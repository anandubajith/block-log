block-log
=========

![A screenshot of block-log theme.](/images/block-log.png)

| [Live demo](https://anandu.net/demo/block-log/) | [Github Repo](https://github.com/anandubajith/block-log) | [Download zip](https://github.com/anandubajith/block-log/archive/master.zip) |
|-----------|-------------|---------------|

Setting up
====================
To start you own blog, simply git clone the repository on github. You could also press the "fork" button on github.
```
git clone https://github.com/anandubajith/block-logs.git
```
Then you will need to edit the `_config.yml` file at the root of repository.

To add your own posts, add a file to the `_posts` directory which has the name `year-month-day-title.md`.
*Note - the file does not have to be markdown.*

To publish the post, just `git push` it to your own github repo and your set!

Things to change on `_config.yml`
====================
There is a config file at the root called `_config.yml`. By Default it looks like:
```
title:        "Block-Log"
description:  "Write an awesome description for your blog."
baseurl:      "" # the subpath of your site, e.g. /blog/
url:          "http://yourdomain.com" # the base hostname & protocol for your site
permalink:    /:year/:title
github:       "yourusername"
twitter:      "yourusername"
email:        "mail@example.com"
disqus-id:    "example" #leave blank if you dont want comments.
markdown:     kramdown
sass:
    style: :compressed
```

For more information on Jekyll, visit their [wiki on github](https://github.com/mojombo/jekyll/wiki).
For more information on github pages: [http://pages.github.com](http://pages.github.com).

License
====================
### The MIT License (MIT)

Copyright (c) 2015 Anandu B Ajith

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
