---
template: blog-post
title: How to combat FOIT and FOUT
slug: /combat-FOIT-FOUT
date: 2020-09-26 16:01
description: How to combat FOIT and FOUT
---
For the uninitiated, FOIT stands for Flash Of Invisible Text and FOUT stands for Flash of Unstyled Text. Both are the result of the text loading before the font on your site and can be rather jarring and unpleasant to the user. FOIT prevents the user from reading until the font has loaded(or a set amount of time has passed) while FOUT displays the unappealing default font and then changes it to the desired font after loading.

Out of the two, which option is superior? As always with web design, the answer isn’t clear cut. FOIT prioritizes typeface aesthetics while FOUT prioritizes text functionality and accessibility to those with slow connections where the font may never load. So while web developers may cringe at the thought of some users viewing their site with unstyled text, it is my opinion that an accessible site is better than a pretty site that the user cannot read.

But surely we don’t have to choose? How do web developers fight back against them? One solution is to preload the font. This seems like a great idea at first, as it stops both FOIT and FOUT, but it delays the initial render of the web site. Preloading too many things will diminish the performance of your site. Another possible solution is using the “font-display” CSS. It lets you have more control over FOIT and FOUT. The “Fallback” value is a good middle ground that will use FOIT for a short period of time before switching to FOUT. A third option is to use a trick called FOFT, Flash of Faux Text, this relies on loading a custom font variant first, forcing the browser to create “faux” bold and italic, then switching to the real versions when everything has loaded.