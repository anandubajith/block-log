<img src="http://anandu.info/img/block-log.png">
Jekyll is pretty rad and figured releasing a cleaned up version of my site as a theme for others to hack and build on would be fun. So here be that theme — I call it Block-log, a responsive Jekyll theme focused on minimalism for personal blogs.

[Live Demo](http://anandu.info/block-log)

[Download](https://github.com/anandubajith/block-log/archive/master.zip)

[Github Repo](https://github.com/anandubajith/block-log)


Setting up
====================
To start you own blog, simply git clone the repository on github. You could also press the "fork" button on github.
<pre><code>git clone https://github.com/anandubajith/block-log.git</code></pre>
Then you will need to edit the _config.yml file at the root of repository.

To add your own posts, add a file to the _posts directory which has the name year-month-day-title.md. 
<br>Note - the file does not have to be markdown.

To publish the post, just <code>git push</code> it to your own github repo and your set!
> #After Cloning make sure to delete the <code>gh-pages</code> branch, Because it contains a lot of junk used for the demo site.

Things to change on `_config.yml`
====================
There is a config file at the root called `_config.yml`. By Default it looks like:

    name: block-log
    description: Hi, This is <b>block-log</b>.<br>A Jekyll theme build with minimalist blocks
    markdown: redcarpet
    pygments: true
    disqus-id: anandu
    email: me@example.com
    twitter: twitterusername
    github: gitusername
    
You will need to change <code>name</code> , <code>url</code> , <code>twitter-username</code> and <code>github</code>. All others are optional, Here is what the variables mean.<br>

<code>name</code> - The name of your jekyll site.<br>
<code>description</code> - A description for your site<br>
<code>markdown</code> - The preferred markdown to use. <br>
<code>disqus-id</code> - the disqus id, if not set comments will not be shown.<br>
<code>twitter-username</code> - Your Twitter username , used while sharing.<br>
<code>email</code> - your email,if unset willnot be shown<br>
<code>github</code> - Your github username<br><br>

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

