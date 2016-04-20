---
layout: post
title: "Slack effects & layoffs"
date: 2016-04-20
categories: slack, humane software
description: "Side effects in Slack."
---

Last month, [I was laid off](https://twitter.com/dotsara/status/710157222391615489) ([more info](http://recode.net/2016/03/16/livingsocial-is-laying-off-more-than-50-percent-of-its-staff/)). 2 days after my 5-year anniversary, no less! :persevere:

But what I'm interested in today is what happened _before_ I was laid off. Or…&nbsp;_while_ I was being laid off? Ugh, whichever.

My last team made heavy, heavy use of [Slack](https://slack.com/)'s [integrations](https://slack.com/apps); in fact, we had a channel (`#flex-team-bots`!) just for Github and CI-related (continuous integration) messages. New pull request? _Message!_ Build failed on `x` server? _Message!_ 

All of that would have been 150% overwhelming in our regular channel, but siloed this way they were easy to consume as needed. 

The morning of the layoffs, right as DM conversations about layoffs fired up, I noticed a bunch of integrations in multiple channels disappearing. _So-and-so deleted an integration in this channel: Github_

After a handful of these, I @-messaged the person whose name paired with the delete messages, asking if he was auditing integrations or what. 

Right about then, [Mike Evans](https://twitter.com/m_evans10) DM'd me to point out that when a Slack account is deleted…&nbsp;any integrations that account setup are deleted as well. 

Oh. _Ooooh._ Oh, fuck.

So, **tl;dr**: the Slack account responsible for deleting is the account used in automated messages to the channels/people specified by a given integration.

## A few thoughts…

1. I don't imagine anyone expected automated messages to act as a coal mine canary, my goal here isn't to wag a finger at Slack, I just wanted to point this out.   <br /><br />
   _Knowing is half the battle…?_
2. In this situation, the person responsible for deleting might not _enjoy_ having to do it but the way Slack seems to be set up, that person ends up _the face_ of it (who knows how many DMs and @'s he got that day…&nbsp; :confused: ).   <br /><br />
	_Maybe **slackbot** could "send" these messages?_
3. Because the automated messages don't provide any detail beyond their app (Github, New Relic, etc.) there's no way to know _which_ integration was deleted. It might have been really important and useful, but once the dust settles and people realize it's missing, it's a guessing game about how to get it back.   <br /><br />
   _An integration archive might be useful here?_   
   `[integration app] [channel destination] [settings] [dates]`

[Anil Dash](https://twitter.com/anildash) talks about [humane tech](https://medium.com/humane-tech/toward-humane-tech-23a20405681a#.l11omvdii) and my friend (and former coworker!) [Ernie Miller](https://twitter.com/erniemiller) talks about [humane _development_](https://ernie.io/2016/03/15/talk-humane-development-empathy-unpacked/) and these layoffs functioned, for me, as a practical demonstration of how and why humane tech & development are important.

:wave:   
-Sara