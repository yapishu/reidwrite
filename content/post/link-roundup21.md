+++
categories = ["blog"]
draft = false
description = ""
date = "2017-10-20T00:00:13-05:00"
title = "link roundup 21"
tags = ["blog","links"]

+++

### reading

the list is a bit skimpy this week (and unusually heavy on a single source), but i'm trying to push out an update for the sake of regularity.

  - [Origins and History of Unix, 1969-1995](http://www.catb.org/esr/writings/taoup/html/ch02s01.html) -- catb.org

> [![](/img/thompson.jpg#thumb-right)](/img/thompson.jpg)A 1974 paper in Communications of the ACM [Ritchie-Thompson] gave Unix its first public exposure. In that paper, its authors described the unprecedentedly simple design of Unix, and reported over 600 Unix installations. All were on machines underpowered even by the standards of that day, but (as Ritchie and Thompson wrote) “constraint has encouraged not only economy, but also a certain elegance of design”.

> After the CACM paper, research labs and universities all over the world clamored for the chance to try out Unix themselves. Under a 1958 consent decree in settlement of an antitrust case, AT&T (the parent organization of Bell Labs) had been forbidden from entering the computer business. Unix could not, therefore, be turned into a product; indeed, under the terms of the consent decree, Bell Labs was required to license its nontelephone technology to anyone who asked. Ken Thompson quietly began answering requests by shipping out tapes and disk packs — each, according to legend, with a note signed “love, ken”.

> This was years before personal computers. Not only was the hardware needed to run Unix too expensive to be within an individual's reach, but nobody imagined that would change in the foreseeable future. So Unix machines were only available by the grace of big organizations with big budgets: corporations, universities, government agencies. But use of these minicomputers was less regulated than the even-bigger mainframes, and Unix development rapidly took on a countercultural air. It was the early 1970s; the pioneering Unix programmers were shaggy hippies and hippie-wannabes. They delighted in playing with an operating system that not only offered them fascinating challenges at the leading edge of computer science, but also subverted all the technical assumptions and business practices that went with Big Computing. Card punches, COBOL, business suits, and batch IBM mainframes were the despised old wave; Unix hackers reveled in the sense that they were simultaneously building the future and flipping a finger at the system.

  - [How Israel Caught Russian Hackers Scouring the World for U.S. Secrets](https://www.nytimes.com/2017/10/10/technology/kaspersky-lab-israel-russia-hacking.html) -- nytimes.com

> Kaspersky’s researchers noted that attackers had managed to burrow deep into the company’s computers and evade detection for months. Investigators later discovered that the Israeli hackers had implanted multiple back doors into Kaspersky’s systems, employing sophisticated tools to steal passwords, take screenshots, and vacuum up emails and documents.

> In its June 2015 report, Kaspersky noted that its attackers seemed primarily interested in the company’s work on nation-state attacks, particularly Kaspersky’s work on the “Equation Group” — its private industry term for the N.S.A. — and the “Regin” campaign, another industry term for a hacking unit inside the United Kingdom’s intelligence agency, the Government Communications Headquarters, or GCHQ.

> Israeli intelligence officers informed the N.S.A. that in the course of their Kaspersky hack, they uncovered evidence that Russian government hackers were using Kaspersky’s access to aggressively scan for American government classified programs, and pulling any findings back to Russian intelligence systems. They provided their N.S.A. counterparts with solid evidence of the Kremlin campaign in the form of screenshots and other documentation, according to the people briefed on the events.

  - [The World Once Laughed at North Korean Cyberpower. No More.](https://www.nytimes.com/2017/10/15/world/asia/north-korea-hacking-cyber-sony.html) -- nytimes.com

> [![](/img/nkinterview.jpg#thumb-right)](/img/nkinterview.jpg)More recently, North Koreans seemed to have changed tack once again. North Korean hackers’ fingerprints showed up in a series of attempted attacks on so-called cryptocurrency exchanges in South Korea, and were successful in at least one case, according to researchers at FireEye.

> The attacks on Bitcoin exchanges, which see hundreds of millions of dollars worth of Bitcoin exchanged a day, offered Pyongyang a potentially very lucrative source of new funds. And, researchers say, there is evidence they have been exchanging Bitcoin gathered from their heists for Monero, a highly anonymous version of cryptocurrency that is far harder for global authorities to trace.

> The most widespread hack was WannaCry, a global ransomware attack that used a program that cripples a computer and demands a ransom payment in exchange for unlocking the computer, or its data. In a twist the North Koreans surely enjoyed, their hackers based the attack on a secret tool, called “Eternal Blue,” stolen from the National Security Agency.

it's astonishing how quickly our cyberpunk future has manifested in the last five years.

  - [Elliptic Curve Cryptography for Beginners](http://blog.wesleyac.com/posts/elliptic-curves) -- blog.wesleyac.com

> I find cryptography fascinating, and have recently become interested in elliptic curve cryptography (ECC) in particular. However, it's not easy to find an introduction to elliptic curve cryptography that doesn't assume an advanced math background. This post is an attempt to explain how ECC works using only high school level math. Because of this, I purposely simplify some aspects of this, particularly around terms that have specific mathematical meaning. However, you should still get a good intuitive understanding of elliptic curves from this post.

  - [A low-level explanation of the mechanics of Monero vs Bitcoin in plain English](https://www.monero.how/how-does-monero-work-details-in-plain-english) -- monero.how

> We don't want the sender of a transaction to notice when the recipient of the transaction then spends the funds in a new transaction. Monero solves this problem through the use of ‘ring signatures’.

> Ring signatures enable ‘transaction mixing’ to occur. Transaction mixing means that when funds are sent, the sender randomly chooses several other users’ funds to also appear in the transaction as a possible source of the funds being sent. The cryptographical nature of the ring signature means that no one can tell which of the funds were really the source of the transaction – not even the person that gave the funds to the sender in the first place. A system of ‘key images’ associated with each ring signature ensures that although no one can tell the true source of the funds, it can be easily detected if the sender attempts to anonymously send their funds twice.

  - [What Did the C.I.A. Do to His Father?](http://www.nytimes.com/2001/04/01/magazine/cia-what-did-the-cia-do-to-his-father.html) (2001) -- nytimes.com

> A week or so later, Eric, Lisa, Nils and two lawyers met the C.I.A.'s director, William Colby, at the agency's headquarters in Langley, Va. In his memoirs, Colby remembered the lunch as ''one of the most difficult assignments I have ever had.'' At the end of the lunch, Colby handed the family an inch-thick sheaf of declassified documents relating to Frank Olson's death. What Colby did not tell them -- did not reveal until he published his memoirs just three years later -- was that Frank Olson had not been a civilian employee of the Department of the Army. He had been a C.I.A. employee working at Fort Detrick.

> The Colby documents were photocopies of the agency's own in-house investigation of Olson's death and like Eric's collages: a redacted jumble of fragments, full of unexplained terms like the ''Artichoke'' and ''Bluebird'' projects. These turned out to be the precursors of what became known as MK-ULTRA, a C.I.A. project, beginning in the Korean War, to explore the use of drugs like LSD as truth serums, as well as botulism and anthrax, for use in covert assassination.

> The documents claimed that during a meeting between the C.I.A. and Fort Detrick scientists at Deep Creek Lodge in rural Maryland on Nov. 19,1953, Sidney Gottlieb of the C.I.A. slipped LSD into Olson's glass of Cointreau. After 20 minutes, Olson developed mild symptoms of disorientation. He was then told the drink had been spiked. The next day, Olson returned home early and spent the weekend in a mood that Alice remembered as withdrawn but not remotely psychotic. He kept saying he had made a terrible mistake, but she couldn't get him to say what it was.

  - [Why Arabs Lose Wars](http://www.meforum.org/441/why-arabs-lose-wars) (1999) -- meforum.org

> [![](/img/schwarzkopf.jpg#thumb-right)](/img/schwarzkopf.jpg)Second, the complex mosaic system of peoples creates additional problems for training, as rulers in the Middle East make use of the sectarian and tribal loyalties to maintain power. The 'Alawi minority controls Syria, East Bankers control Jordan, Sunnis control Iraq, and Nejdis control Saudi Arabia. This has direct implications for the military, where sectarian considerations affect assignments and promotions. Some minorities (such the Circassians in Jordan or the Druze in Syria) tie their well-being to the ruling elite and perform critical protection roles; others (such as the Shi'a of Iraq) are excluded from the officer corps. In any case, the assignment of officers based on sectarian considerations works against assignments based on merit.

> The same lack of trust operates at the interstate level, where Arab armies exhibit very little trust of each other, and with good reason. The blatant lie Gamal Abdel Nasser told King Husayn in June 1967 to get him into the war against Israel—that the Egyptian air force was over Tel Aviv (when most of its planes had been destroyed)—was a classic example of deceit.27 Sadat's disingenuous approach to the Syrians to entice them to enter the war in October 1973 was another (he told them that the Egyptians were planning total war, a deception which included using a second set of operational plans intended only for Syrian eyes).28 With this sort of history, it is no wonder that there is very little cross or joint training among Arab armies and very few command exercises. During the 1967 war, for example, not a single Jordanian liaison officer was stationed in Egypt, nor were the Jordanians forthcoming with the Egyptian command.29

  - [Digital Fascism: Anti-PC Idol Smashing Isn't Just a Joke](http://www.tabletmag.com/jewish-news-and-politics/247110/internet-alt-right-fascists) -- tabletmag.com

> In recent years two powerful currents in trolling came together to produce the digital vanguard of the alt-right. One was opposition to political correctness and the increasingly censorious culture of mainstream liberalism. The other was a creeping despair. Where the anti-PC sentiment had a fairly broad appeal, this was a more pointed sentiment. It was associated in its political dimensions with increasingly maligned and alienated young white men who saw their career and social prospects narrowing at the same time as interpersonal relations seemed to fracture and grow more mercenary. Feminism, immigration and demographic shifts changed both the labor and cultural environments. Naturally, white men who had the most status to lose, reacted with the greatest vehemence. Some became embittered and joined together in subcultural communities of resentment. They saw themselves not just as victims of circumstance but came to believe they had been cheated out of their rightful power and influence by a conspiracy of interlopers: women, minorities, Jews.

> The hacker scholar Gabriella Coleman has compared 4chan’s trolls to the dadaists and in a particular unintended way there was truth in this comparison. Egging each other on under the cloak of anonymity, free to voice their fears and desires, the young men of 4Chan unleashed tremendous creative energies that still influence and redound in mainstream popular culture. If the 4Chan hive could sometimes behave like an art collective, it is also the case that Dadaists, in common with other modernist movements, were drawn to totalitarian temptations. Dadaism was dedicated to aesthetics above all and politically incoherent, but it evinced a belief “that the style and the beautiful gesture was all that mattered” as the historian Walter Laqueur wrote in his cultural history of the Weimar Republic, “and for that reason sympathized with the bomb throwers rather than their victims.”

nagle has been making quite a name for herself since her book was released. her book is stellar, imo -- i've really enjoyed most of what i've read by her, but [this interview](http://zero-books.net/blogs/zero/zero-squared-127-nagle-answers-her-critics-such-as-they-are/) is a great introduction to her as well.

  - [These Giant Printers Are Meant to Make Rockets](https://www.bloomberg.com/news/articles/2017-10-18/these-giant-printers-are-meant-to-make-rockets) -- bloomberg.com

> [![](/img/3dp.jpg#thumb-right)](/img/3dp.jpg)Near the back of the factory, Relativity is tinkering with alloys to make its metals better suited for 3D printing and to be able to combine more of a rocket’s hull and inner workings. “The space shuttle had 2.5 million moving parts,” Ellis says. “We think SpaceX and Blue Origin have gotten that down to maybe 100,000 moving parts per rocket. We want to get to 1,000 moving parts, fewer than a car.”

> Relativity is running lean, with just 14 full-time employees and $10 million in funding from the likes of Dallas Mavericks owner Mark Cuban, venture firm Social Capital, and startup accelerator Y Combinator. In June it successfully test-fired its printed engine at a NASA facility in Mississippi. By mid-2020 the company plans to print a 90-foot-tall, 7-foot-wide rocket that can carry 2,000 pounds to orbit; the founders say it’ll fly in 2021. At that size and the $10 million launch price, the rocket could take smallish corporate satellites into orbit for far less than what government-run space agencies charge.

>Four years, however, is a long time. Both Blue Origin and SpaceX are run by billionaires with a knack for making things cheaper; over the past decade, Musk’s team has used advances in consumer electronics, software, and manufacturing to cut launch costs to $60 million, from the typical $100 million to $300 million. Both companies have also started to perfect reusable rockets and can take more cargo to orbit on their much larger craft.

### misc

  - [Colony](https://colony.io/) -- colony.io

a decentralized platform for organizations built on ethereum

  - [Urbyte 1: Atoms, auras, types](https://urbit.org/docs/byte/1/) -- urbit.org

educational documents for urbit -- i still find the whole thing kind of mind-bending and like i don't grasp enough of it to really understand what it makes possible, but it's still fun to learn and think about.
