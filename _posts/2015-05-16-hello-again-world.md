---
layout: post
title: "Hello again, World!"
date: 2015-05-16
categories: learning
description: "Back to bloggin' and stuff."
---

Aloha!

So, check it out: it took me _almost_ 10 attempts to grok how to make a Jekyll-Github pages site again. I'd done it once before, but went 18 months never updating it, so, y'know: clean slate! (_I know, I know:_ dead links.) Fool that I can sometimes be, I totally thought this time it would be easier. Jekyll gem, all this extra experience under my belt, blah blah blah…&nbsp;

I can hear you laughing from here.

I tried 4 times to start over again using [Jekyll's own documentation](http://jekyllrb.com/docs/home/) and for reasons I don't fully understand myself, I'd hit a brick wall after running `jekyll new name-of-my-new-site`.

Instead of boring you with how spectacularly stumped I can get, I'll tell you what finally worked for me.

Before doing anything at [github.com](https://github.com) or at the command line, I opened up a bunch of Github Pages tutorials and read through them. (I can, fairly, be accused of sometimes jumping too soon and trying to start a thing before reading all the instructions. _ahem_)

I had tried (and failed) so many times to start from scratch, so the first step in [this Smashing Magazine tutorial](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/) where you fork a ready-made Jekyll repo and just edit the `_config.yml` is what really helped everything fall into place for me.

[Heather](http://jxnblk.com/Heather) is the theme I wanted to use and now that I got the whole fork-then-edit thing, starting over with Heather was a snap. Hooray!

If you have a [peek at the repo for this site](https://github.com/dotsara/dotsara.github.io), you'll notice that it doesn't say it's forked from the Heather repo, anymore. And that's because in the spirit of "I don't know, try it out!" I wanted to learn how to kill the commit history on a forked repo. (There's no real need for me to keep it in this instance.)

Stack Overflow to the rescue! [How do I remove the old history from a git repository?](http://stackoverflow.com/questions/4515580/how-do-i-remove-the-old-history-from-a-git-repository) Way down at the bottom, [I found what I was after](http://stackoverflow.com/a/28081807).

Here's what I did locally:

* Fork the Heather theme to my repo
* Rename the newly-forked repo to `dotsara.github.io` (Settings > Repository name)
* Clone the repo (via SSH because I don't want to have to enter my user/pass every. single. time) to my machine: `git clone git@github.com:dotsara/dotsara.github.io.git`
* `cd` into my new folder: `cd dotsara.github.io`
* Delete the `.git` directory, re-initialize the folder as a git folder, add a remote server back   
   `sudo rm -r .git && git init && git remote add origin git@github.com:dotsara/dotsara.github.io.git`
* Edit this blog post, make a new commit (which will show all the Jekyll & theme files as new/untracked) and push!

:tada:

And that's…&nbsp;that. See you soon!