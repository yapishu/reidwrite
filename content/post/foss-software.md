+++
date = "2017-03-01T21:04:27-06:00"
title = "foss software"
tags = ["blog",""]
categories = ["blog"]
draft = false
description = ""

+++

_i switched to linux_ about 2.5 years ago, after using windows my entire life, starting with 3.1 on a desktop in my room that i got in 1997. i have to say i am absolutely delighted with the state of desktop linux. i tried using linux on my computers a few times over the years without having it stick -- first with suse on a laptop in 2002 using cd's i picked up at a used bookstore, then with ubuntu in about 2010. both times i got fed up with minor annoyances that required much more work to fix than i was used to, inside an unfamiliar paradigm that frustrated me.

what changed this time? well, i put openwrt on a router, and had to use vi to edit the configuration. i finally sat down to learn basic cli functions beyond simply copying commands verbatim from tutorials, and found that it had a relatively straightforward logic to it. i wanted to try unix-like operating systems again and see if i could hack it. this time around, my computers worked flawlessly out of the box, and i didn't have to fix any fundamental issues. i did one online tutorial in particular -- [learn the command line, by codecademy](https://www.codecademy.com/learn/learn-the-command-line) -- which left me feeling genuinely _excited_ about understanding how computers worked for the first time since i was a kid.

i've since switched to linux on every pc i own, and i've become one of 'those guys' when i talk about computers with friends now. but i can't help it, i think this stuff is genuinely really fun.

currently i use [xubuntu](http://xubuntu.org/) (ubuntu with xfce) on my desktop, an [asus vivopc](https://www.amazon.com/Asus-VIVOPC-VM40B-04-ASUS-Desktop/dp/B01AUG1V9C/) -- nothing very special, but a cute little box -- and [galliumos](https://galliumos.org/) on my [toshiba chromebook 2](https://www.amazon.com/Toshiba-Chromebook-CB35-C3300-Backlit-Keyboard/dp/B015806LMM), which is an xubuntu derivative distro meant for chromebooks.

galliumos is a real treasure -- it's very lightweight, _very_ fast, and all of my hardware works perfectly. my toshiba was chosen almost arbitrarily, just trying to balance between reviews and pricepoint, but i made a really good choice with it on one particular point: it comes with a 16gb ssd, which i swapped out for a 128gb. that was the main constraint on it in its stock configuration, but with the 128 i don't have to worry about a crowded disk. even with full disk encryption (via [luks](https://guardianproject.info/code/luks/), which is selected during install), it goes from boot to logged in in under ten seconds.

i intend to dive in a little deeper at some point, and will probably try installing arch on a machine once i'm comfortable restoring from backups, but for now i'm very pleased with my software configurations and workflows.

anyway, the reason i wanted to make this particular post was to share some of the software i've found that i'm excited about -- the stuff that justifies switching to linux, in my opinion. so are some of my favorite examples:

1. [sshuttle](https://github.com/apenwarr/sshuttle)
   * this was the first piece of linux software that got me seriously excited: if you have a user account on a remote server you can ssh into, you can tunnel your whole connection through it -- a poor man's vpn. vpn's aren't expensive to begin with, but i pay $15/year for one with [ramnode](http://ramnode.com/vps.php). it's also **much** simpler than configuring openvpn or similar on your server, and requires much less overhead (somewhat necessary when your vps has 128mb of memory!). one small issue: on every computer i've tried running the sshuttle client on, on the first attempt after a boot, it will give an error message and drop the connection immediately. not to worry though, because it will work on second attempt with no hitches. if you have rsa key auth set up on ssh, you don't even need to enter a password. simply alias ```sudo sshuttle -r user@server 0/0``` to 'proxy' or something. voila! you have transparently forwarded your connection. a friend uses it with a vps in the uk to watch geolocked content.

2. [vimwiki](https://github.com/vimwiki/vimwiki)
  * a personal wiki inside of vim, which uses markdown, and autoindexes entries. i use this to take notes for school, and keep my working directory in a folder in spideroak to sync between my computers. it also has an excellent export to html function. mostly, i'm using this to work on my vim abilities.

3. [atom](https://atom.io/)
  * cross-platform, extensible, and beautiful text editor developed by github. i use this for editing the markdown files for this blog, primarily, though i intend to use it if/when i force myself to learn some programming. it's a real pleasure to use, especially with a dark theme.

4. [borg](https://borgbackup.readthedocs.io/en/stable/)/[borgmatic](https://github.com/witten/borgmatic)
  * cli backup software, which deduplicates and supports encryption. backup to anywhere you can ssh into, and encrypt it if you don't trust whoever controls it. borgmatic is a script to automatic the backups, and enforce rules -- eg pruning old backups.

5. [pass](https://www.passwordstore.org/)
  * cli keepass/lastpass alternative. saves each entry into an individual gpg-encrypted file, making it similarly portable (and combine well with) borg. to be honest, i don't use this because i'm stuck on lastpass's convenience, but i'm glad it exists. if i (or you) ever decide to switch, there is fortunately a script to export [lastpass-to-pass](https://git.zx2c4.com/password-store/tree/contrib/importers/lastpass2pass.rb). if lastpass ever has a security breach that shakes my faith in them, this is what i intend to fall back onto.

6. [redshift](http://jonls.dk/redshift/)
  * this is simply an open source clone of [f.lux](https://justgetflux.com/) -- if you're unfamiliar with it, it shifts the light temperature of your monitor towards warm/orange tint as the sun goes down. the idea is that blue light disrupts your internal clock and can hurt your sleep. instead, your monitor has a warm cfl-like glow as the night goes on. i find it much easier to look at, in any case.
