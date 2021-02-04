---
layout: post
title: Teaching Open Source Exercises
subtitle: This Bugs Me
tags: [reading, reflection, zulip, open-source, bugs]
---
After reading chapter 6 of [Teaching Open Source](https://quaid.fedorapeople.org/TOS/Practical_Open_Source_Software_Exploration/html/sn-Debugging_the_Code-Exercise_-_Find_the_Oldest_Bug.html) I applied some of the exercises related to bug searching on our team's FOSS project, Zulip. The repository for zulip can be found [here](https://github.com/zulip/zulip). 

### EX. 6.4 Find the oldest bug that's still open in your chosen project. Write a blog entry describing the problem, with a theory about why the bug hasn't been resolved yet. (Bonus points if you can actually resolve the bug.)

The oldest open issue (without a pending PR) was from September 26th 2015 titled ***Installation script breaks other sites*** and was issue #39 so it is an easy assumption this has been an ongoing issue since project conception. The issue seems to involve configuration files and some backend programming which I am not very familar with. From what I can gather, this bug arose because on certain setups could override configuration files when zulip was being installed. Initially a README file was updated and this workaround was sufficent until in February of 2016 another user requested the issue be reponed because it was still breaking certain installations. 

For the next couple of years, labels were added and removed which was meant to prompt other members of the zulip community to take notice. The bug has recently gained activity from another user making commits to their own branch of zulip and referenced this old issue. Maybe finally after 7 years the bug will be resolved soon. It has likely taken so long because it seems to involve the larger scope of the project build and installation files, something I don't know how to fix. 

### EX. 6.5 Figure out how to create a new account on the bug tracker of your chosen project. You'll need that account very soon.

I have created an account on Github, and a zulip account while also joining the zulip organization. I have claimed one issue and have been assigned to it. You can find the issue [here](https://github.com/zulip/zulip/issues/2278). The main hurdle will be to recreate this issue because it seems like many other users have had trouble recreating this particular bug in the past. 

### EX. 6.6 Go through your project's bug tracker and find a bug that you think you might be able to reproduce -- and then try to reproduce it in the latest build. Take careful notes. Report your experiences as a comment to the bug. If you can reproduce the bug, great! Give as much information as you can. If you can't reproduce the bug, great! Give as much information as you can, and ask the original reporter if there are other steps you might be able to take to reproduce the bug.

I chose [this](https://github.com/zulip/zulip/pull/16725) bug which actually has a pending review PR. In this bug, in user settings when you would pick a favorite date a calendar widget pops up. If you press the esc button you exit back to the main home page of zulip but the calendar widget still appears. I was able to recreate this bug exactly as they described. The only way to get rid of this widget is by reloding the page or by clicking anywhere else on the screen. You can also select a date and it will be entered into the sytsem and appear in the field when you return to the user settings page. I will decline to leave a comment on this issue because the Pull Request has passed all checks and is only pending review. 

### EX. 6.7 Find five bug reports in the new state, and attempt to triage them according to the rules above. Your goal is to do as much as you possibly can, in a short period of time, to make those bug reports as useful as possible to the developer to whom they are assigned. (Note: be sure to follow any triage rules that your project may have defined. If there are no set triage rules, be sure to announce your intentions on the project's mailing list, so that developers can provide you some guidelines if they choose.)

For my bug triage, I looked at Zulip's issue tracker and sorted to the newest issues. I decided to pick these five: 

* [Can't close message edit form after internet connection is lost](https://github.com/zulip/zulip/issues/17190)
* [Can't search history of shared-history private streams](https://github.com/zulip/zulip/issues/17183)
* [filter: Check if search operand is valid](https://github.com/zulip/zulip/issues/17175)
* [widgets: Prevent edits to /poll and /todo messages.](https://github.com/zulip/zulip/issues/17156)
* [feature request: Add green/orange presence circles to PM/mention autocompletes](https://github.com/zulip/zulip/issues/17138) 

I would rank them from high to low priority as such: 

1. [Can't search history of shared-history private streams](https://github.com/zulip/zulip/issues/17183)
2. [Can't close message edit form after internet connection is lost](https://github.com/zulip/zulip/issues/17190)
3. [filter: Check if search operand is valid](https://github.com/zulip/zulip/issues/17175)
4. [widgets: Prevent edits to /poll and /todo messages.](https://github.com/zulip/zulip/issues/17156)
5. [feature request: Add green/orange presence circles to PM/mention autocompletes](https://github.com/zulip/zulip/issues/17138) 

I rank them in this order because 5. is simply a feature request, this doesn't affect the overall functioning of the project. 4. is also a simple edit to prevent edits to certain widgets with an error message. 3. Is of medium priority since it seemed to be fixed quickly, but searching with an invalid operand leads to a 400 error which is not desireable. 1. and 2. directly affect how the users interact with Zulip and the 1st regarding search history seems to cause a lot of confusion with users while 2. is also a high priority because in the issue thread, there are problems trying to re create this issue again. 


