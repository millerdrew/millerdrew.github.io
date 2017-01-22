---
layout: post
title:  "Wrangling Vim"
date:   2017-01-22
comments: true
categories: jekyll update
---

![Vim](/assets/vim.png)

If you are looking for code editors that are beginner friendly, I would suggest [Atom](https://atom.io/) or [Sublime](https://www.sublimetext.com/).  Both are excellent, modern editing tools that any web developer should be comfortable with.

But if you're like me, and want to get a little crazy with an editor that has a steep learning curve but pays dividends down the road, it's hard to find something to match [Vim](http://www.vim.org/).  Do yourself a favor though and don't start with vanilla Vim... Instead get a nice starter pack such as this one created by Square called [Maximum Awesome](https://medium.com/square-corner-blog/fly-vim-first-class-610f1a39b572#.qexo773dp).

It doesn't look like much until you realize it gives you complete control without ever having to resort to a mouse.  That's right:  With magical combinations of keystrokes you are able to zip around your files making changes at a much faster rate than you would otherwise.  The flipside is that you spend a lot of time in the beginning stumbling through those commands as you learn them.

Now I don't recommend jumping into Vim while cutting off all help... Make life a little easier on yourself by using MacVim.  It allows you to use the mouse when you need to and makes for a much smoother transition into the world of Vim.

Normal Vim is started on the command line like this:
```
vi
```
While for MacVim
```
mvim
```

An example of some shortcuts:

* Jumping around files with ,t (similar to cmd-p in sublime)
* Accessing directory through Nerdtree with ,d or ,f
* Creating/deleting/renaming files within Nerdtree with m
* Searching within a file with /
* Moving around with hjkl

There's many many more, and I plan on including a reference of the ones I use the most.

Here are some settings that I changed with my home directory in the .vimrc.local file:

```
colorscheme solarized
set background=dark
set lines=100 columns=200
set guifont=Menlo\ Regular:h24
```

Before I changed those settings I found the MacVim started in a tiny window with a tiny font... And the colorscheme is just for fun :smile:.  

Give it a shot.  You might find Vim not so crazy after all :wink:.

{% if page.comments %}
<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = "{{ page.url }}";  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = 'joyfulcoding-com'; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
var disqus_developer = 1;
};
*/

(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = '//joyfulcoding-com.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
{% endif %}

