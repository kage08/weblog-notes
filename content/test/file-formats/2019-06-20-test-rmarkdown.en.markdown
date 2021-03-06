---
title: Test Links in .Rmarkdown file format
author: Peter Baumgartner
date: '2019-06-20'
slug: test-links-in-rmarkdown
categories: []
tags: []
lastmod: ~
description: 'How to link from a file in <code>.Rmarkdown</code> format to other pages.'
disable_comments: yes
draft: yes
---

TEST, TESTEN and again TESTING!

## Using markdown link format in .Rmarkdown file

### From md to all other directories and formats

These links work always as they URL in paranthesis refers directly to the URL taken from the browser.

+ **Markdown link from post into same directory:** Text before link [This is the LinkText](/2019/06/05/physik-libre-a-bookdown-project/) and Text after link
+ **Markdown link from post, into another post directory:**Text before link [This is the LinkText](/2018/07/19/blogdown-using-themes/) and Text after link
+ **Markdown link from post, into tutorial directory:**Text before link [This is the LinkText](/tutorial/how-to-produce-bibliographic-metadata-for-you-web-page/) and Text after link
+ **Markdown link from post, into tutorial directory with other format:**Text before link [This is the LinkText](/test/test-citation/) and Text after link

## Using shortcode link format in .Rmarkdown file is the same as in .md files

The reason is that _`.RMarkdown` is internally converted to `.markdown`._

### From md to all other directories and formats


+ **Markdown link from post into same directory:** Text before link [This is the LinkText]({{< ref "2019-06-20-test-rmd" >}}) and Text after link
+ **Markdown link from post into another directory:** Text before link [This is the LinkText]({{< ref "/post/2019/2019-06-18-DS-coursera" >}}) and Text after link
+ **Markdown link from post into another directory:** Text before link [This is the LinkText]({{< relref "2019-06-18-DS-coursera" >}}) and Text after link
