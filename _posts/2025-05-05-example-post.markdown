---
layout: post
title:  "Adding a post to this site"
date:   2025-05-05 14:35:52 +0100
categories: jekyll update
---

### Making a post 
First of all you'll need to make a new file in the `_posts/` directory with a name in the format `YYYY-MM-DD-POSTNAME.markdown`

### How to write Markdown
Thankfully the majority of writing Markdown is the same as writing plain English - you just need to tell Jekyll what you'd like it to do with certain bits of text. The title just above this, for example. Go and check out this fantastic guide to see all the wacky and wonderful stuff you can do in Markdown: [https://www.ihsantopaloglu.com/Jekyll-Markdown-Cheat-Sheet/](https://www.ihsantopaloglu.com/Jekyll-Markdown-Cheat-Sheet/)

### Adding a video to your post 
To do this, you'll need to use a little HTML, but YouTube will give you a hand and generate it for you! First of all, go to the video you'd like to add to your post, and click "Share", and then "Embed". You should see something like this:  

{% highlight html %}
```
<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=ZbBBfRSoe3b_dfsF" 
    title="YouTube video player" frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
</iframe>
```
{% endhighlight %}

Simply add that to your post, and voila! Rick Astley at his finest!

<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=ZbBBfRSoe3b_dfsF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
