---
layout: post
title:  "Setting MacVim as the default editor in OSX"
date:   2014-09-20 14:26:45
categories: vim macvim osx
---

In OSX, TextEdit is the default editor for plain text files. TextEdit is not great for coding snippets because it doesn't play well with some characters. Therefore, I wanted to change the default text editor to something else, in my case: MacVim

You can try the method of selecting a .txt file, Get Info, Open with, select MacVim and then use "Change All".

Another way is just running the following command:

{% highlight bash %}

defaults write com.apple.LaunchServices LSHandlers -array-add '{LSHandlerContentType=public.plain-text;LSHandlerRoleAll=org.vim.MacVim;}'

{% endhighlight %}

