---
layout: post
title: Running ELMAG Code
date:  2018-10-28 21:57:54 +0800
categories: [Fortran]
comments: true
---

**Contents**
* TOC
{:toc}
## [Standard tutorial](https://sourceforge.net/projects/elmag/files/)
Download the file [elmag203.tar.gz](http://elmag.sourceforge.net/docs.html); unpacking the files
```
$ tar -xvf elmag203.tar.gz
```
will create the files inside the subdirectory Elmag203.

Using MPI it may be necessary to load libraries,
```
$ module load openmpi-x86_64
```
before compiling and running the executable
```
$ make mpi
$ mpirun -np X a.out &
```
on X processors.

If MPI is not available, a single processor version can be compiled,
```
$ make single
$ ./a.out &
```

>  elmag_py203.tar.gz contains a python wrapper contributed by M. Meyer.
   copy elmag_py203.tar.gz in a subdirectory, unpack and look at README.md
   for instructions. No support for the installation of these files is
   provided.

## Code structure of Elmag
![png]({{ site.url }}/assets/elmag.svg)

Download [source code]({{ site.url }}/assets/elmag.dot)

Tip: Reduce node as much as possible, or the display will be a mess.

## Employ it in your task
Confront a complex software which contains many subprograms, we are required to figure out how the pieces is structured together, then we can employ it to our task. Conclude my way as follow.
* Find Main program

  program Elmagcasc
* Track the Workflow
  1. call MPI_*
  2. call call init
  3. call user_main
  4. call MPI_*
  5. call user_output
  6. call banner
  7. call MPI_*
* The purpose for each node.
  1. call user_main: Customize the condition for your work.

    To specify the EBL model (model), the number of injected particles (nmax), the jet opening angle of the source in degrees (th_jet), edit user_variables.
  2. call user_output: Put the result to somewhere.
  3. call banner: Make an easy interface for user who is watching the executing process.

## Some modification on MacOS
### Install openmpi on MacOS through `brew`

Inspired from a [answer](http://linuxdesktops.soton.ac.uk/openmpi.html) to install openmpi on other os. [Furthermore](https://unix.stackexchange.com/questions/80711/how-to-install-apt-get-or-yum-on-mac-os-x), `brew` is the equivalent to `apt-get` or `yum` on Mac OS X. Then the solution is clear.
```sh
$ brew install openmpi
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> Updated Formulae
crowdin                    gmime                      nsd

==> Installing dependencies for open-mpi: libevent
==> Installing open-mpi dependency: libevent
==> Downloading https://homebrew.bintray.com/bottles/libevent-2.1.8.mojave.bottl
######################################################################## 100.0%
==> Pouring libevent-2.1.8.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libevent/2.1.8: 846 files, 2.2MB
==> Installing open-mpi
==> Downloading https://homebrew.bintray.com/bottles/open-mpi-3.1.2.mojave.bottl
######################################################################## 100.0%
==> Pouring open-mpi-3.1.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/open-mpi/3.1.2: 736 files, 10.5MB
$ export PATH=$PATH:/usr/local/Cellar/open-mpi/3.1.2/bin/
$ ompi_info
                 Package: Open MPI brew@Mojave.local Distribution
                Open MPI: 3.1.2
  Open MPI repo revision: v3.1.2
   Open MPI release date: Aug 22, 2018
                Open RTE: 3.1.2
  Open RTE repo revision: v3.1.2
   Open RTE release date: Aug 22, 2018
                    OPAL: 3.1.2
...
$ mpirun -np 2 a.out &
```
This time I do it fluently without digging in attachment knowledge on `module`.

## Modify [Elmag ](https://github.com/marcomuzio/Elmag) template
```sh
$ bash run_basic_fill.sh
```

* [sed: 1: "user202.f90": invalid command code u](https://markhneedham.com/blog/2011/01/14/sed-sed-1-invalid-command-code-r-on-mac-os-x/)
