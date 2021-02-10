--- 
layout: post
title: IEEE Software 
subtitle: What's Happening?
---

For today's blog, I read an article from the IEEE Software Magazine titled **Right Code** which you can find linked [here](https://www-computer-org.nuncio.cofc.edu/csdl/magazine/so/2021/01/09305891/1pNkxcsDIoU). 

The authors discuss the need for more reliable software systems and discusses plausible solutions. Boeing is used an example for what can go drastically wrong when systems aren't reliable. The Boeing 737 Max incidents were found to be caused by multiple errors all culminating. Their Starliner which was Boeing's attempt at a reuseable spacecraft, failed miserably and a NASA panel found it was due to multiple software bugs. So how can we avoid these issues in the future? 

## System Reliability

In most other systems, redundancy has made systems more reliable. For example, having multiple eingines in case one fails. But in software this isn't as easily replicated. If you have a bug in your software and install it on two different computers, the same bug could crash both systems. This is what led to the demise of the maiden flight of Ariane in 1996. Another method for increasing redundancy is N-version programming. In this method, two development teams would start working on the same project in parallel and would consistently compare to eradicate any bugs. This method also has its faults. It pitted teams against one another and did not deliver any form of reliability increase. It is also worth noting that if both teams are working in parallel, they still start at the same point and are thus more likely to make similar mistakes with the same initial requirements. 

So if these methods have failed, how can we include redundancy to increase reliability of our software? We can create self checking code. By including assertions at key points in your code (similar to how we test) it has been proven that there are less faults in the code. So what about when it comes ot testing? A function with a lower cyclomatic complexity does not necessarily require fewer tests to vet thoroughly. All code is written to satisfy some set of requirements and provide a desired functionality. We can spread that functionality across multiple modules and functions to create a large assembly of interconnected and mutually dependent small functions, but that will rarely be the right way to structure the code, and neither will it be able to simplify testing.

In conclusion, the sobering news is that more tests leads to less bugs. This redundancy can help developers avoid a catastrouphic failure down the line. When creating tests it is important to derive these suite of tests from your requirements rather than the structure of a control-flow graph since there are multiple ways to navigate it. 
