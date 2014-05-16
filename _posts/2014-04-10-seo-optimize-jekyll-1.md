---
layout: post
title:  "SEO Optimize Jekyll - Part 1"
date:   2014-04-10 12:12:00
categories: jekyll,seo optimize,sitemap
description: Adding a sitemap to jekyll is simple all you have to do is create a file named sitemap.xml in the root of your jekyll site with the following contents.
keywords: jekyll,seo optimize,sitemap
---
###Adding A Sitemap
Adding a sitemap to jekyll is simple all you have to do is create a file named sitemap.xml in the root of your jekyll site with the following contents.
<pre><code>
&#45;&#45;&#45;<br/>&#45;&#45;&#45;<br/>&#60;?xml version="1.0" encoding="UTF-8"?&#62;<br/>&#60;urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9"&#62;<br/>&#123;% for post in site.posts %&#125;<br/>&#60;url&#62;<br/>&#60;loc&#62;http://anandu.info &#123;&#123; post.url | remove: 'index.html' &#125;&#125;&#60;/loc&#62;<br/>&#60;/url&#62;<br/>&#123;% endfor %&#125;<br/>&#123;% for page in site.pages %&#125;<br/>&#123;% if page.layout != nil %&#125;<br/>&#123;% if page.layout != 'feed' %&#125;<br/>&#60;url&#62;<br/>&#60;loc&#62;http://anandu.info &#123;&#123; page.url | remove: 'index.html' &#125;&#125;&#60;/loc&#62;<br/>&#60;/url&#62;<br/>&#123;% endif %&#125;<br/>&#123;% endif %&#125;<br/>&#123;% endfor %&#125;<br/>&#60;/urlset&#62;
</code></pre>
###Submit Sitemap To Google
Once you have added your sitemap its time to submit it to google.For that you need to have a google account setup with webmaster tools,and have your site verified with webmaster tools.Instruction on how to do that [here](https://support.google.com/webmasters/answer/183669?hl=en#183669)
