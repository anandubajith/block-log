---
layout: post
title:  "SEO Optimize Jekyll - Part 2"
date:   2014-04-11 12:12:00
categories: jekyll,seo optimize,sitemap
description: Meta tags are required for better seo.Twitter cards and Facebook opengraph tags are required for better shares in social media.This will help you in adding those to your jekyll powered blog.
keywords: jekyll,seo optimize,sitemap
excrept: Meta tags are required for better seo.Twitter cards and Facebook opengraph tags are required for better shares in social media.This will help you in adding those to your jekyll powered blog.
---
Meta tags are required for better seo.Twitter cards and Facebook opengraph tags are required for better shares in social media.This will help you in adding those to your jekyll powered blog.
###Add Meta Tags
Edit your default template located in <code>_layouts/default.html</code> and add the following code just above the <code>&lt;/head&gt;</code>
<pre><code>&lt;meta name=&quot;twitter:title&quot; content=&quot;&#123;&#123; page.title &#125;&#125;&quot;&gt;
&lt;meta property=&quot;og:title&quot; content=&quot;&#123;&#123; page.title &#125;&#125;&quot; /&gt;
&lt;meta property=&quot;og:site_name&quot; content=&quot;&#123;&#123; page.title &#125;&#125;&quot; /&gt;
&lt;meta itemprop=&quot;name&quot; content=&quot;&#123;&#123; page.title &#125;&#125;&quot;&gt;
&#123;% if page.description %&#125;
&lt;meta name=&quot;twitter:description&quot; content=&quot;&#123;&#123; page.description &#125;&#125;&quot;&gt;
&lt;meta property=&quot;og:description&quot; content=&quot;&#123;&#123; page.description &#125;&#125;&quot; /&gt;
&lt;meta itemprop=&quot;description&quot; content=&quot;&#123;&#123; page.description &#125;&#125;&quot;&gt;
&lt;meta name=&quot;description&quot; content=&quot;&#123;&#123; page.description &#125;&#125;&quot; /&gt;
&#123;% else %&#125;
&lt;meta name=&quot;twitter:description&quot; content=&quot;<span style="background:#f39c12;color:#fff;">default description</span>&quot;&gt;
&lt;meta property=&quot;og:description&quot; content=&quot;<span style="background:#f39c12;color:#fff;">default description</span>&quot; /&gt;
&lt;meta itemprop=&quot;description&quot; content=&quot;<span style="background:#f39c12;color:#fff;">default description</span>&quot;&gt;
&lt;meta name=&quot;description&quot; content=&quot;<span style="background:#f39c12;color:#fff;">default description</span>&quot; /&gt;
&#123;% endif %&#125;
&lt;meta name=&quot;twitter:creator&quot; content=&quot;<span style="background:#3498db;color:#fff;">@twitter-username</span>&quot;&gt;
&lt;meta name=&quot;twitter:domain&quot; content=&quot;<span style="background:#e74c3c;color:#fff;">domain.com</span>&#123;&#123; page.url &#125;&#125;&quot;&gt;
&lt;meta property=&quot;og:type&quot; content=&quot;article&quot; /&gt;
&lt;meta property=&quot;og:url&quot; content=&quot;<span style="background:#e74c3c;color:#fff;">http://domain.com</span>&#123;&#123; page.url &#125;&#125;&quot; /&gt;
&lt;meta property=&quot;og:image&quot; content=&quot;<span style="background:#7f8c8d;color:#fff;">http://domain.com/opengraph-image.png</span>&quot; /&gt;
&lt;meta name=&quot;twitter:image:src&quot; content=&quot;<span style="background:#16a085;color:#fff;">http://domain.com/twitter-image.png</span>&quot;&gt;
&lt;meta name=&quot;twitter:card&quot; content=&quot;summary&quot;&gt;
&lt;meta name=&quot;twitter:site&quot; content=&quot;<span style="background:#3498db;color:#fff;">@twitter-username</span>&quot;&gt;
&lt;link rel=&quot;author&quot; href=&quot;https://plus.google.com/<span style="background:#8e44ad;color:#fff;">google-plus-profile-id</span>/posts&quot;/&gt;
&#123;% if page.keywords %&#125;
&lt;meta name=&quot;keywords&quot; content=&quot;&#123;&#123; page.keywords &#125;&#125;&quot;&gt;
&#123;% else %&#125;
&lt;meta name=&quot;keywords&quot; content=&quot;<span style="background:#2c3e50;color:#fff;">default-keywords</span>&quot;&gt;
&#123;% endif %&#125;
</code></pre>
###Installation
Change the following values accordingly <br><br>
<span style="background:#3498db;color:#fff;">@twitter-username</span> - with your twitter username.<br>
<span style="background:#2c3e50;color:#fff;">default-keywords</span> - with your default keywords.<br>
<span style="background:#8e44ad;color:#fff;">google-plus-profile-id</span> - with your google plus profile ID.<br>
<span style="background:#e74c3c;color:#fff;">domain.com</span> - with your url.<br>
<span style="background:#16a085;color:#fff;">http://domain.com/twitter-image.png</span> - with image to be shown on Twitter.<br>
<span style="background:#7f8c8d;color:#fff;">http://domain.com/opengraph-image.png</span> - with image to be shown on Facebook. <br>
<span style="background:#f39c12;color:#fff;">default description</span> - with the description of your page.<br>

###Usage
Once you have completed the above steps, In your YAML front matter you can you two new tags <code>description</code> and <code>keywords</code>.
Like this for an example
<pre><code>
&#45;&#45;&#45;
layout: post
title:  "SEO Optimize Jekyll - Part 2"
date:   2014-04-11 12:12:00
categories: jekyll,seo optimize,meta tags,opengraph
description: a small tutorial on how to optimize jekyll for search engines. 
keywords: jekyll,seo optimize,sitemap
&#45;&#45;&#45;
</code></pre>
