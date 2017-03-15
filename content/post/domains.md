+++
draft = false
date = "2017-03-14T18:03:10-05:00"
title = "domains and virtual hosts"
description = ""
tags = ["blog","writing"]
categories = ["blog"]

+++

i spent the better part of the last day working on getting a second site running on my vps. it's live now -- you can see it at [hyperstition.al](https://hyperstition.al) (get it?). i got lazy about theming and just cloned this blog for the moment. this writeup is mostly for reference in case anything breaks in the future.

first step was registering .al, as cheaply as possible, which i ended up doing for 13/yr with a registrar called istanco (no points for guessing the nationality). it took surprisingly long for the domain to propagate -- at least six hours, i went to bed eventually. i thought that kind of latency was relegated to the old days, but i suppose that is to be expected with an albanian domain.

the next step was configuring a second virtual host on apache. this part was especially confusing because the official documentation appeared to tell me to place the edits in `/etc/hosts`, when they actually went in `httpd.conf` (`apache2.conf` on ubuntu). this was followed by it seeing the document root as `/var/www/html` instead of `/var/www/hyperstition.al/public_html`, which i couldn't figure out how to fix, so i sighed and just tried to move on to configuring ssl.

[lets-encrypt](https://letsencrypt.org/) is some seriously magical software. i went through the motions of following a [DO tutorial](https://www.digitalocean.com/community/tutorials/how-to-set-up-let-s-encrypt-certificates-for-multiple-apache-virtual-hosts-on-ubuntu-14-04) for configuring virtual hosts on ubuntu, and in the most baffling step in this process, running the setup script somehow managed to *crash my vps*. as in, i had to log into the vm cp and turn it back on. i don't have the faintest fucking clue how this happened.

i double checked my config files, remembered to strip out the stuff i had put into my `hosts` file, and ran it again -- voila, not only did it work without a hitch, it began serving the new domain out of the proper document root.

so, now i have a cute albanian [domain hack](https://en.wikipedia.org/wiki/Domain_hack), and it's got forced ssl.

the next bit took an embarrassingly long time to figure out. to update this blog, i run a relatively straightforward command:

  `rsync -av public/ reid@artorias.pw:/var/www/artorias.pw/public_html/`

however, with the new domain's folder i kept getting error messages along the lines of

  `rsync: recv_generator: mkdir "/var/www/hyperstition.al/public_html/categories" failed: Permission denied (13)`

i spent a good hour and a half trying to figure out what the fuck was going on, eventually figuring it had something to do with folder permissions, and trying to learn how to parse `ls -l` output. *eventually* i guessed that using chown on `/var/www/hyperstition.al` to change the owner ought to work, and some time after that realized that changing `public_html` in that folder was the real key. and, finally, all is as it should be -- rsync copies everything over without a hitch.

i'm probably going to change the theme to [code-editor](http://themes.gohugo.io/hugo-code-editor-theme/) once i get around to writing something worth posting, but for now, i'm happy that everything is still humming along. and to celebrate: indian food tonight.

---
