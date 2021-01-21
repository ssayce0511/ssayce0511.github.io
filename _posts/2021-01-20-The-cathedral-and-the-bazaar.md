---
layout: post
title: The Cathedral & The Bazaar
subtitle: Reflections on FOSS
cover-img: /assets/img/cover2.jpg
thumbnail-img: /assets/img/cathe.jpg
share-img: /assets/img/path.jpg
tags: [reading, reflection]
---

The Cathedral & the Bazaar compares the two methods of software development. The author initially believed that the most important software was to be built like a cathedral. Crafted carefully by a group of individuyal wizards working in isolation, with no beta released before it is time. The Lunix community on the other hand was compared to a bazaar of differing agendas and approaches out of which a coherent and stable system emerged only by a sucession of miracles. 

Raymond continues, citing his need for a POP3 client. Through this personal ancedote the author relates important mantras. 

1. Every good work of software starts by scratching a developers personal itch. 
  Raymond needed a new client, so he decided to make one.
2. Good programmers know what to write. Great ones know what to rewrite (and reuse). 

  Instead of writing something from scratch, Raymond gathered a couple of candidates that were most similar to his desired client. Picking and choosing features and rewriting existing open source code saved him time and effort. 
  
3. "Plan to throw one away; you will, anyhow." - Fred Brooks 

  The author relates to this because he made the choice to switch to a different code because he noticed some critical errors in his current project. Raymond also states that you really don't understand a problem until after the first time you impliment a solution. Once the author got in contact with the project's owner, he quickly took over control which demonstrates the next two mantras: 
  
  4. If you have the right attitude, interesting problems will find ypu. 
  5. When you lose interest in a pgoram, your last duty to it is to hand it off to a competent successor. 
  The author also learned that many contributors to OSS are also the users of the software. 
  6. Treating your users as co-developers is your least hassle route to rapid code imporvement and effective debugging. 
  
  Early and frequent releases are a critical part of the Linux development model. Most developers don't like this because on larger more trivial projects, the early versions were always bugggy and you don't want to lose users because of this. This reinfoced the belief that the cathedral method was the only way. If the overriding objective was for your users to encounter as few bugs as possible, you would only be releasing every 6 months and debugging like crazy between releases. Linux proved this wrong and had a healthy development evironment. Linux knew that: 
  7. Release early and release often. Listen to your customers. 
  8. Given a large enough beta-tester and co-developer base, almost every problem will be characterized quickly and the fix obvious to someone. 
  
  These two mantras above are central to the cathedral vs bazaar debate. From a cathedral point of view, bugs are complex and insidious problems. It takes months of scruitiniy and a few dedicated developers, thus the long intervals and inevitable disappointment when something isn't perfect. The bazaar on the other hand assume that bugs are shallow phenomena or at least the turn shallow pretty quickly once ecposed to a thousand eager co developers. Accordingly, when you release often you get more corrections. Going off of this point. 
  
  10. If you treat your beta testers as if theyre youur most valuble resource, they will respond by becoming your most valuable resource. 
  
  11. The next best thing to having good ideas is recognizing good ideas from your users. Sometimes the latter is
better.

12. Often, the most striking and innovative solutions come from realizing that your concept of the problem was
wrong.

The last two mantras ask us to take some reflective thinking. The author encourages developers that have hit a road block to reflect and ask if your asking the right question rather than if you have the correct answer. OFten reframing the problem is the solution. We can also relate this to the idea of feature bloat. Especially in an FOSS environment. This leads us to the next mantra: 

13. "Perfection in design is achieved not when there is nothing more to add, but rather when there is nothng more to take away." 

You should also be open to letting a project grow in new wasys. 

14. Any tool should be userful in the expected way, but a truly great tool lends itself to uses you never expected. 
15. When writing gateway software of any kind, take pains to disturb the data stream as little as possible – and
*never* throw away information unless the recipient forces you to!

Moving on lets discuss some necessary preconditions for the bazaar style of development. 

Its clear that you cannot start from the ground up in bazaar style. Its fine to test and debug and improve in this style, but to origonate is another thing. When you start community-building you need a plausible promise. The program doesn't have to work well it must only not fail and run, and convince potential co developers that it can evolve into something better. It is absolutley critical that the coordinator of a project be able to recognize the good ideas of others. 
  
