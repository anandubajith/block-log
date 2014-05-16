---
layout: post
title:  "Squared - A Minimalistic Jekyll Theme"
date:   2014-06-09 14:19:00
categories: jekyll, themes
---
<img src="/img/squared.png" title="Squared - A Minimalistic Jekyll Theme" alt="Squared - A Minimalistic Jekyll Theme">
I have designed a new theme for my blog , its based on the colors of Flat UI and it is minimalistic.Today I share it with the world!!!.

[Live Demo](http://anandu.info/squared)

[Download](https://github.com/anandubajith/squared/archive/master.zip)

[Github Repo](https://github.com/anandubajith/squared)


Setting up
====================
To start you own blog, simply git clone the repository on github. You could also press the "fork" button on github.
<pre><code>git clone https://github.com/anandubajith/squared.git</code></pre>
Then you will need to edit the _config.yml file at the root of repository.

To add your own posts, add a file to the _posts directory which has the name year-month-day-title.md. 
<br>Note - the file does not have to be markdown.

To publish the post, just <code>git push</code> it to your own github repo and your set!

Things to change on `_config.yml`
====================
There is a config file at the root called `_config.yml`. By Default it looks like:

    name: Squared Theme
    markdown: redcarpet
    permalink: /:title
    disqus-id: anandu
    url: http%3A%2F%2Fanandu.info 
    twitter-username: anandubajith
    author: Anandu

You will need to change <code>name</code> , <code>url</code> , <code>twitter-username</code> and <code>author</code>. All others are optional, Here is what the variables mean.<br>

<code>name</code> - The name of your jekyll site.<br>
<code>markdown</code> - The preferred markdown to use. <br>
<code>permalink</code> - the permalink to use for your posts.<br>
<code>disqus-id</code> - the disqus id, if not set comments will not be shown.<br>
<code>url</code> - The parsed URL of your site.<br>
<code>twitter-username</code> - Your Twitter username , used while sharing.<br>
<code>author</code> - Your Name!!.<br><br>

For more information on Jekyll, visit their [wiki on github](https://github.com/mojombo/jekyll/wiki).

For more information on github pages: [http://pages.github.com](http://pages.github.com).

License
====================
The MIT License (MIT)

Copyright (c) 2014 Anandu B Ajith

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

