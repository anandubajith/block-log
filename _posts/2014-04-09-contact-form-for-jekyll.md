---
layout: post
title:  "How To Add Contact Form To Jekyll"
date:   2014-04-09 12:12:00
categories: personal
description: Jekyll is a simple, blog-aware, static site generator build with ruby.if you are hosting Jekyll on a host that supports php you can have a contact form build with php, but when you are hosting on a host that does not support php, like github..
keywords: jekyll,contact,page

---
<div class="cover">
</div>
Jekyll is a simple, blog-aware, static site generator build with ruby.if you are hosting Jekyll on a host that supports php you can have a contact form build with php, but when you are hosting on a host that does not support php, like github pages you can't do that.This is the time you may start to rely on third party services but most of these services does not support customization, recently i found a service that supports customization of everything.The service is called [Simple Form](http://getsimpleform.com/).

### Using It With Jekyll
* Go to [Simple Form homepage](http://getsimpleform.com/) and sign up, scroll down to the bottom of the page and copy your form api token.
* Create a new page in jekyll and add the following contents in to it
<pre><code>
&lt;form action=&quot;http://getsimpleform.com/messages?form_api_token=<span style="color:#e74c3c"><b>apikey</b></span>&quot; method=&quot;post&quot;&gt;<br/>  &lt;input type='hidden' name='redirect_to' value='<b><span style="color:#3498db">redirect-to</span></b>' /&gt;<br/>  &lt;input type='text' name='Name' placeholder=&quot;Your Name&quot; /&gt;<br/>  &lt;input type='text' name='email' placeholder=&quot;Your Email&quot; /&gt;<br/>  &lt;textarea name=&quot;message&quot; placeholder=&quot;Your Message&quot;&gt;&lt;/textarea&gt;<br/>  &lt;input type='submit' value='Submit' /&gt;<br/>&lt;/form&gt;
</code></pre>
* Replace <span style="color:#e74c3c"><b>apikey</b></span> with your form api token then replace <b><span style="color:#3498db">redirect-to</span></b> with the page you want to redirect to after the user submits the form.

If you want a live demo check out [http://anandu.info/contact/](http://anandu.info/contact/).

