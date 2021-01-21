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
  
  These two mantras above are central to the cathedral vs bazaar debate. From a cathedral point of view, bugs are complex and insidious problems. It takes months of scruitiniy and a few dedicated developers, thus the long intervals and inevitable disappointment when something isn't perfect. The bazaar on the other hand assume that bugs are shallow phenomena or at least the turn shallow pretty quickly once ecposed to a thousand eager co developers. Accordingly, when you release often you get more corrections. 
