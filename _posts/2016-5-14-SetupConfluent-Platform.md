---
layout: post
title: Setup Confluent Platform Locally on Mac
description: ""
modified: 2016-05-14
tags: [confluent, setup]
image:
  feature: journalism-for-blogging.jpg
  credit: Fotolia
  creditlink: https://www.fotolia.com/id/1505473

---

How to setup confluent platform locally (without using docker containers):

Download the package:
http://docs.confluent.io/2.0.1/installation.html



I use "confluent-2.0.1-2.11.7.tar.gz".

Before following steps in quick start guide, update ./etc/kafka/server.properties


{% highlight html %}
{% raw %}
host.name=localhost
advertised.host.name=localhost
{% endraw %}
{% endhighlight %}

(Otherwise, you will encounter "LeaderNotFound" or other strange Kafka communication errors.)

Follow quick start:
http://docs.confluent.io/2.0.1/quickstart.html
