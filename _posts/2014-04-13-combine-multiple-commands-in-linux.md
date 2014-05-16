---
layout: post
title: "Combine Multiple Commands In Ubuntu"
date: 2014-04-13 12:12:12
categories: ubuntu,linux,commands
description: In a developers workflow he may need to use the termial a lot also he might want to repeat a set of commands one after the other continuously, But what if we can combine these long commands into a single small command.Yes it's Possible with the help of a simple bash script!.
keywords: combine,ubuntu,terminal,linux,bash
---

In a developers workflow he may need to use the termial a lot also he might want to repeat a set of commands one after the other continuously, But what if we can combine these long commands into a single small command.Yes it's Possible with the help of a simple bash script!.

###Steps
There are two versions of this script, the first one is to execute the next command only if the previous one suceeds(_conditonal execution_).The second one will not check if the previous one suceeded or not(_unconditonal execution_).Before that run these commands and replace <span style="background:#e74c3c;color:#fff">smallcommand</span> with your small command.
<pre>
cd /usr/local/bin
sudo gedit <span style="background:#e74c3c;color:#fff">smallcommand</span>
</pre><br><br>
After running the last command you will get a gedit window, copy and paste the desired script from below and save the file. Remember <b>conditonal execution</b> is to execute the next command only if the previous one suceeds and <b>unconditonal execution</b> will not check if the previous one suceeded or not.<br><br>

<h3>Conditonal execution</h3>
<pre>
#! /bin/sh
command 1 \
&& command 2 \
&& command 3 \
&& command 4 \
</pre>
<br>

###Uconditonal execution
<pre>
&#35;! /bin/sh
command 1
command 2
command 3
command 4
</pre><br><br>
Now you can use <span style="background:#e74c3c;color:#fff">smallcommand</span> instead of the long commands.
