---
layout: post
title: Blogging Like a Neuboie
---

This is the first post and I'm just testing. Check this kewl snippet:

{% highlight scala %}
def handleEvents(uid: String) = for {
  id  <- uid.as[Int]
  _   <- authorize(id, Admin)
  res <- handleEventsGet(id) | handleEventsPost(id)
} yield res
{% endhighlight %}
