+++
description = ""
tags = ["blog",""]
date = "2017-04-23T00:07:00-05:00"
title = "newsbeuter"
categories = ["blog"]
draft = false

+++

i found something i'm absolutely delighted with the other day -- it's called [newsbeuter](http://newsbeuter.org/), and it's a cli ncurses rss reader -- "the mutt of rss readers". [documentation](http://newsbeuter.org/doc/newsbeuter.html), [archwiki article](https://wiki.archlinux.org/index.php/Newsbeuter), [github](https://github.com/akrennmair/newsbeuter).

after i left most social media a few years ago, i started assembling a new mode of internet use. i spent a lot of time cruising blogs and finding interesting people and began posting on a forum, for the most part. i had been using [feedly](https://feedly.com/) as an rss reader -- i never had a chance to try google reader, and i kept crashing and burning trying to host rss software like [tiny tiny rss](https://tt-rss.org/fox/tt-rss/wikis/home) on my vps. feedly works reasonably well, but it's bloated and ugly so i've been keeping my eyes open. enter newsbeuter

[![](/img/ncurses.jpg#thumb-right)](/img/ncurses.jpg)i've come to really enjoy being able to read and compute on a dark screen cramped with terminals. [ncurses](http://www.etcwiki.org/wiki/Best_ncurses_linux_console_programs) is a cross-platform library meant to create terminal-based gui's, and i've developed a lot of aesthetic attachement to having newsbeuter, vim, [ncmpcpp](https://rybczak.net/ncmpcpp/), and [finch](https://coderstalk.blogspot.com/2008/09/finch-howto-use-pidgin-via-terminal.html) filling my peripheral vision with nice mono terminal text and dark color schemes. it beats flashing browsers and memory-intensive gui frameworks imo, at least. 

the only real disappointment i've had with newsbeuter is that there doesnt seem to be any way to have a single linear timelines one can simply scroll through or paginate -- only individual posts, manually reloaded (autoreload is an option but blasting 60 urls every time i want to open it was a bit of a pain), paged through with `n`. 

anyway -- i'm so excited about having a terminal based rss reader that i wanted to share, even if i'm just talking into the void of this blog. i hope someone else might find it as exciting as i do. and [here](https://github.com/yapishu/dotfiles/blob/master/newsbeuter) is my config dotfile -- i think it's relatively sane to copy/paste.
