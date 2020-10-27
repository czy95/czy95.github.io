---
layout: post
title: Start to use Graphviz
date:  2018-10-19 15:10:16 +0800
categories: [Visualization]
comments: true
---

**Contents**
* TOC
{:toc}
## Random words
Graphviz is hosted on gitlab, It's the first serious projects I've ever met on
Gitlab. I think there are many immature projects hosted on gitlab for which has
a quite short history.

## Code example
```dot
digraph G {  
label = "My way to become a astrophysicist";  
node [shape = record];  

A  [label = "Data scientist", color = red];

B1 [label = "Statistics", color = green];  
B2 [label = "Astronomy", color = green];
B3 [label = "Reasonable Life", color = green];
B4 [label = "Composing", color = green];
B5 [label = "Programming", color = green];
B6 [label = "Presentation", color = green];

B1C1 [label = "Foundation"];
B1C2 [label = "Algorithm"];
B2C1 [label = "Arxiv"];
B2C2 [label = "Classical Books"];
B3C1 [label = "Speaking fluently"];
B3C2 [label = "Exercise"];
B3C3 [label = "Travel"];
B3C4 [label = "Read a lot of books"];
B3C5 [label = "Just keep \nin \ntouch with family"];
B4C1 [label = "Daily writting"];
B4C2 [label = "Pick a right \nproblem"];
B5C1 [label = "I got this"];
B2C1D1 [label = "Think hard"];

A->{B1;B2;B3;B4;B5;B6}[color="#FFFF00"]
B1->{B1C1;B1C2}[color="blue"]
B2->{B2C1;B2C2}[color="#00F5FF"]
B3->{B3C1;B3C2;B3C3;B3C4;B3C5}[color="#0000CD"]
B4->{B4C1;B4C2}
B5->B5C1;
B2C1->B2C1D1;
B1C1->B1C2;
B2C1->B2C2;
}
```
## Rusulat and effects
Graphviz own several modes of layout.

`dot -Tpng a.dot -o a.png` generates:

![png]({{ site.url }}/assets/graphviz.png)


`circo -Tpng a.dot -o a.png` gernerates:

![png]({{ site.url }}/assets/circo.png)

## Reference
* [使用graphviz绘制流程图](http://icodeit.org/2015/11/using-graphviz-drawing/)
* [Official documentation](http://graphviz.org/doc/info/shapes.html)
