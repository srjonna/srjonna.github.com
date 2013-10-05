---
layout: post
title: "code example"
description: ""
category: "Pyments"
tags: []
author: "Kalona"
---
{% include JB/setup %}

### Java Pygments Example

{% highlight java %}
public static void main(String[] arg) {
    List<String> awesome = Arrays.asList("ObjectOriented")
                          .stream()
                          .map(s -> "FunctionalProgramming-" + s)
                          .collect(Collectors.toList());
}
{% endhighlight %}

<!--end excerpt-->

### Scala Pygments Example

{% highlight java %}
object HelloWorld {
    def main(args: Array[String]) {
      println("Hello, world!")
    }
  }
{% endhighlight %}

###With line numbers

{% highlight java linenos=table %}
public static void main(String[] arg) {
    List<String> awesome = Arrays.asList("ObjectOriented")
                          .stream()
                          .map(s -> "FunctionalProgramming-" + s)
                          .collect(Collectors.toList());
}
{% endhighlight %}

