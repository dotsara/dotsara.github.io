---
layout: post
title: "A developer&#8217;s work is never done…"
date: 2015-08-06
categories: learning
description: "There's no glamour, but there *is* satisfaction."
---

"[The Tedium of Managing Code](http://alistapart.com/column/the-tedium-of-managing-code)" by [Lyza Danger Gardner](https://twitter.com/lyzadanger) is excellent (h/t [@scriberty](https://twitter.com/scriberty)).

From the lede: "There’s a place motivation goes to die for web developers. It’s when something we have to do is simultaneously very, very hard and very, very uninteresting. You know, the corner of Hard and Boring Streets in downtown Must-Ship-to-Clientsville."

To which I must add: _word_. 

Our code base isn't old by software standards, but in Internet years, it's practically middle-aged. We used to be a monorail, but [now we rock SOA](https://techblog.livingsocial.com/blog/categories/soa/), which is great! :dancer: 

However, we obviously have what any (every?) large-scale site has: cruft, dead code, junk drawer files. All those "ugh, I'll clean this up later" helper methods, all that horrendously nested and specific CSS, so much clunky, janky javascript. We have it all. (You can be jealous, it's all right.)

A few months back I found myself on a new team and with the luxury (yes) of very few proper projects. I'd occasionally worked on a clean-up task here and there (encouraged by one of my excellent coworkers: [Tom Copeland](https://twitter.com/tcopeland)) and I thought, "hey self, why not _just_ work on clean-up? You know that junk drawer file you hate deep down in your bones? Now's your chance!"

And so I took it!

What does it take to focus on clean-up work for 3 months? What I learned is:

* clean-up work is a non-destructive way to indulge in [yak shaving](http://sethgodin.typepad.com/seths_blog/2005/03/dont_shave_that.html); oh sure, you start all high-minded, ready to whip `this-terrible-stylesheet.css` into shape and a week later you've produced 6 pull requests, deleted a thousand lines of code, and feel pretty awesome. But you still haven't deleted the file. (Yet.)
* you need to schedule non-clean-up work for yourself. Classes, tutorials, [rubber ducking](https://en.wikipedia.org/wiki/Rubber_duck_debugging) for a coworker, _something_. _Anything_. The breaks will keep you from climbing the walls and/or spending a lot of money on new keyboards…
* you absolutely need the support of your team and your team lead/manager/boss. We are a pull request kind of organization and it was not uncommon for me to open 5 in a week. If your team doesn't respond well to a steady flow of pull requests: you in danger, girl.


I'm a frontend dev and that means clean-up work happens in several arenas. Searching projects in my text editor, [`ack`-ing](http://beyondgrep.com/) in a shell (_and_ in my text editor), running test suites (over and over and over), running our entire site locally and kicking the tires (over and over and over). It's a lot (see above: tedious).

So why do it?

It is _so_ satisfying. _Hell yeah_ I kept a brag sheet of my deletions (nearly 10,000 LOC!) and it was pretty fun watching the numbers change week-to-week.

It is also _so_ important. Reducing overhead when coworkers need to edit, add, or delete a feature? Reducing my own team’s confusion when we’re bug-hunting or troubleshooting? That is incredibly valuable. All the time you don’t spend wondering what a block of code means or does is time you get to spend solving problems.

While I wouldn't want to _live_ on the corner of Hard and Boring Streets, it's a useful place to visit and leave better than you found it. :punch:

-Sara