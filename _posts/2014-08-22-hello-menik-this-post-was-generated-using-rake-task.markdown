---
layout: post
title: "Hello Menik ! This post was generated using rake task"
date: 2014-08-22 00:00:35 +0700
comments: true
categories: 
tags: 
---

how to use

open your terminal and type :

{% highlight ruby %}
rake post:create
{% endhighlight %}

then enter your desired title

you are free to edit the template. just go to lib/tasks/post.rake and change whatever you want in :

{% highlight ruby%}
File.open(filename, 'w') do |post|
  post.puts "---"
  post.puts "layout: post"
  post.puts "title: \"#{title.gsub(/&/,'&amp;')}\""
  post.puts "date: #{Time.now.strftime('%Y-%m-%d %H:%M:%S %z')}"
  post.puts "comments: true"
  post.puts "categories: "
  post.puts "tags: "
  post.puts "---"
end
{% endhighlight %}


