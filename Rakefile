require 'date'

currentTime = Time.now
desc 'create a new draft post'
task :post do
  title = ENV['TITLE']
  slug = "#{Date.today}-#{title.downcase.gsub(/[^\w]+/, '-')}"

  file = File.join(
    File.dirname(__FILE__),
    '_posts',
    slug + '.markdown'
  )

  File.open(file, "w") do |f|
    f << <<-EOS.gsub(/^    /, '')
    ---
    layout: post
    title: #{title}
    date:  #{currentTime}
    categories: []
    comments: true
    mathjax: true
    toc: true
    ---
    **Contents**
    * TOC
    {:toc}


    EOS
  end

  system ("#{ENV['EDITOR']} #{file}")
end
