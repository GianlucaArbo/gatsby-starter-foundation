---
template: blog-post
title: What the Font!? A Guide to Web Safe Fonts.
slug: /what-the-font
date: 2020-09-19 19:32
description: web safe fonts
---
Fonts are a great way to make your website stand out from the pack, they add extra flair to your site while maintaining simplicity, but they can also cause a number of problems. You can spend however much time you want picking the perfect font for your blog, but if it doesn’t display for the end user then all of that time will be wasted, and they will be greeted by a bland default font picked by their browser. 

The simplest solution to this problem is to use a “web safe” font. This is a font that is installed on the majority of computers and thus has the highest chances of being displayed on the user’s browser. If your site uses one of these fonts, then it will rarely ever have the issue of not being displayed properly. Unfortunately, this list is quite small, mainly due to mac and windows featuring a very different list of default fonts, with only five fonts being considered universal. This is abysmally small for any aesthetically oriented web developer. You can set your favorite fonts as the first option, with other more universal web safe fonts as a fallback, but this isn’t ideal. 

The @font-face CSS technique is a rather simple solution, requiring only a few lines of code to implement. It loads the desired font onto the user’s browser so they can see your carefully picked font in all of its glory. But @font-face comes with its own share of problems, not all web browsers support the same file extensions, forcing you to have fallbacks. Another problem is the increased loading caused by having more fonts. 

As with most things in web development, you have to weigh the pros and cons, universal accessibility or aesthetics, and choose what is right for you.