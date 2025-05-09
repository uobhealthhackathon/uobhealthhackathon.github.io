---
layout: post
title:  "Adding a post to this site"
---

### How does the website work?
The website itself is hosted using something called [GitHub Pages](https://pages.github.com/), which GitHub offers for free to everyone! We're using something called [Jekyll](https://jekyllrb.com/) which helps us to take markdown files (you'll learn about this in a sec) and turn it ✨ magically ✨ into the HTML (and CSS and JavaScript) that you're seeing right now. How cool is that!

### Making a post 
First of all you'll need to make a new file in the `_posts/` directory with a name in the format `YYYY-MM-DD-POSTNAME.markdown`. The top of that file contains something called [front matter](https://jekyllrb.com/docs/front-matter/) which tells Jekyll what it contains. The front matter for this post looks like this,
```
---
layout: post
title: "Adding a post to this site"
---
``` 

To create a file, on the [GitHub repository](https://github.com/uobhealthhackathon/uobhealthhackathon.github.io), go to "Code", click the `_posts/` directory, then click "Add file", and then "Create new file"

<img src="{{site.baseurl}}/assets/add_file.png">

From there, give your post the `YYYY-MM-DD-POSTNAME.markdown` name, and click "Commit changes"

<img src="{{site.baseurl}}/assets/create_post.png">

You can do the same for images, but instead of the `_posts/` directory, we should store them in `assets/` instead to keep the repository nice and tidy!

### How to write Markdown
Thankfully the majority of writing Markdown is the same as writing plain English - you just need to tell Jekyll what you'd like it to do with certain bits of text. The title just above this, for example. Go and check out this fantastic guide to see all the wacky and wonderful stuff you can do in Markdown: [https://www.ihsantopaloglu.com/Jekyll-Markdown-Cheat-Sheet/](https://www.ihsantopaloglu.com/Jekyll-Markdown-Cheat-Sheet/)

### Adding an image to your post
This is a little more complicated than adding text, but let's do this. You'll need to use a little HTML, which you can add into your post just like anything else. As with making a post, you'll need to add a new file to GitHub again - this time in the `assets/` directory. This is where we store all of our images, and instead of making a new file, this time you can upload one instead. 

Once `YOUR_IMAGE` is in `assets/`, you can add it to your post like this,
{% highlight html %}
{% raw %}
<img src="{{site.baseurl}}/assets/YOUR_IMAGE.png">
{% endraw %}
{% endhighlight %}

### Adding a video to your post 
To do this, you'll need to use a little HTML, but YouTube will give you a hand and generate it for you! First of all, go to the video you'd like to add to your post, and click "Share", and then "Embed". You should see something like this:  

{% highlight html %}
<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=ZbBBfRSoe3b_dfsF" 
    title="YouTube video player" frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
</iframe>
{% endhighlight %}

Simply add that to your post, and voila! Rick Astley at his finest!

<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=ZbBBfRSoe3b_dfsF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
