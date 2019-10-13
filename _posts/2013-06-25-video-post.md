---
layout: post
title:  "A Post with a Video"
date:   2016-03-15
excerpt: "Custom written post descriptions are the way to go... if you're not lazy."
tag:
- sample
- post
- video
comments: true
---
<iframe width="560" height="315" src="//www.youtube.com/embed/SU3kYxJmWuQ" frameborder="0"> </iframe>
<iframe width="500" height="300" src="http://cld2099web.audiovideoweb.com/va90web25003/companions/Foundations%20of%20Rock/13.01.mp3" id="audio"></iframe>


<audio controls="controls">
  <source type="audio/mp3" src="http://cld2099web.audiovideoweb.com/va90web25003/companions/Foundations%20of%20Rock/13.01.mp3"></source>
  <p>Your browser does not support the audio element.</p>
</audio>
![](13.01.mp3)
Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).

Not sure if this only effects Kramdown or if it's an issue with Markdown in general. But adding YouTube video embeds causes errors when building your Jekyll site. To fix add a space between the `<iframe>` tags and remove `allowfullscreen`. Example below:

{% highlight html %}
<iframe width="560" height="315" src="//www.youtube.com/embed/SU3kYxJmWuQ" frameborder="0"> </iframe>
{% endhighlight %}
