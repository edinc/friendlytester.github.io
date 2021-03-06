---
layout: post
title: How Often Do You Really Fix A "Failing" Automated Check
date: '2015-06-13T18:24:00.000+01:00'
author: Richard Bradshaw
categories:
- Automated Checking
- Automation Design
- Automation in Testing
tags:
- Automation
modified_time: '2015-06-13T20:07:44.589+01:00'
blogger_id: tag:blogger.com,1999:blog-8318661666872903125.post-8431215467083733803
blogger_orig_url: http://www.thefriendlytester.co.uk/2015/06/how-often-do-you-really-fix-failing.html
permalink: /2015/06/how-often-do-you-really-fix-failing.html
comments: true
---

Do we really fix a failing automated check? Or do we simply defunct one and create a new one.  

I saw a tweet the other day from an old colleague of mine.  

> Fixing failing [#selenium](https://twitter.com/hashtag/selenium?src=hash) tests is like playing "Whack A Mole" !  
> — Paul Marshall (@P_Marshall_) [April 28, 2015](https://twitter.com/P_Marshall_/status/592966723986452480)

It got me thinking, how often do we really fix a failing automated check? By fix in this instance, my thoughts started with getting it passing again, getting it green. Even though I prefer not to talk about passing and failing, for the context of this post, passing means satisfying the algorithm and failing means didn't satisfy the algorithm.  

Lots of discussion followed on Twitter after I tweeted, ["You very rarely 'fix' a 'failing' automated check"](https://twitter.com/FriendlyTester/status/592972631705559040), but going to try and summarise the thoughts.  

So lets run through an example, I have a sign up form that has 10 fields on, I also have many checks that are all passing on this form. A new field has been introduced to the form, a mandatory field, this has caused 5 of the checks to now fail. In order to get those checks passing again, then need to be instructed to populate the mandatory field. Does this class as fixing the check?  

I don't believe so, for me this is a new check, it just so happens to reuse 95% of code from a now defunct check. So we haven't fixed it, we have created a new one. Semantic argument some of you may be thinking, but I don't think so. For me, its a very important distinction.  

How often have you been in this situation, the build goes red, someone investigates, 5 checks are failing, then you hear "fix those checks!". If you haven't, replace check with test, and try again. It's certainly something I have experienced multiple times.  

Someone then runs the checks locally and immediately sees that the new field isn't being populated, "oh look it's not populating the mandatory field, I will make it do that", they do it, run them, they all pass! Job done......  

Here lays the problem, how do they know that mandatory field is even meant to be there. Well likelihood is they did know, which then leads to the question, why weren't they "fixed" as part of the initial development work? One problem could be the separation of coding the feature and creating automated checks, happens in a lot of places, especially where 'testing' is a separate activity. It could be they run them after and then fix where required. But I feel it's because teams don't stop to think about the impact changes will have on the checks upfront. Once the work is done, the checks are ran like a safety net, failures investigated and 'fixed'.  

So what's my gripe here? Well I feel more people need to give their use of automated checks more focus, you could write the cleanest automation possible, but if you don't know what they are checking, if anything at all, what use is that to you? It's like the building the wrong product right. We should be thinking at the time of developing new features, what new checks are going to be needed here, and importantly what checks are not. Are existing checks now checking enough, what else should they be looking at.  

Checking can be an important part of an approach to testing, evidently very important at companies where there have created hundreds or thousands of automated checks. If you are going to rely on automated checks so much, then you need to apply a lot of critical thinking to what checks you create and continue to maintain. As repeated many times, your automated checks will only check what they are instructed to, they are completely blind to everything else.  

Designing effective checks, by effective I mean adds value to your testing, supports you in tackling your testing problem can be a difficult process and requires a lot of skill, some are more obvious. It isn't something someone who doesn't understand testing should be doing. Now, turning those into automated checks, sure, I could see that being done by someone who doesn't understand testing, it would be far form ideal though in my opinion.  

The reason I say it's far from ideal relates to this tweet from the start of the year.  

<blockquote class="twitter-tweet tw-align-center" data-lang="en-gb"><p lang="en" dir="ltr">You can not create an automated check without doing some testing first. <a href="https://twitter.com/hashtag/Testing?src=hash">#Testing</a> <a href="https://twitter.com/hashtag/Automation?src=hash">#Automation</a></p>&mdash; Richard Bradshaw (@FriendlyTester) <a href="https://twitter.com/FriendlyTester/status/556407117041893376">17 January 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

Now of course this depends on your framework of choice and the architecture you are building on, but the creation of automated checks can be one of much exploration. It can also be the case of adding some keywords to a spreadsheet, but even in that scenario much exploration would have already been done.  

The application needs to be explored at a level you may have not yet done. In the example of the web, the html needs to be explored for testability, is this a site I can easy automate? At the API level we may discover json elements that we have no idea what they do, or where they come from, we need to work these things out, we need to test.  Also as we are automating a check we may become aware of other attributes/values that we should be checking, and adjust the check accordingly, again though, this requires thought, requires skill. There is also the process of testing the automated check, something I have previously written about [here](http://www.thefriendlytester.co.uk/2014/03/who-tests-checks.html).  

Feel myself going slightly of topic, so lets try to wrap this up. Testing encompasses checking (James Bach & Michael Bolton, http://www.satisfice.com/blog/archives/856), your automated checks should be supporting your testing, helping you tackle your testing problem. Regularly review your automated checks, don't be afraid to delete them, always be evaluating there effectiveness. If you find yourself 'fixing' lots of automated checks, take the time to stop and think about what you are really doing.  

1.  How could the situation have been avoided?
2.  Could it have been done earlier?
3.  What is this check even checking?
4.  I have "fixed" this many time already, is this an effective check?
5.  What information is this checking giving me?

Don't chase green, chase automated checks that support your testing problem. Don't blindly "fix" automated checks. Also for another post, something that we discussed in my automation workshop at LetsTest and Nordic Testing Days recently, do you checks clearly indicate their intention? Sure we can read the code and see what it does, see what it is checking, but what about its original intention, where is that? Be writing about this soon, your "fix" may actually break the algorithm, and therefore mis direct testing effort.  

Remember the code isn't the check, the check is the algorithm. The code is the implementation of it. They may not always align, especially over time and with lots of fixes. Focus on both.  

P.s thanks to [Maaret](https://twitter.com/maaretp) and [Toby](https://twitter.com/TobyTheTester) for their posts, [here](http://visible-quality.blogspot.co.uk/2015/06/checking-how-to-feel-like-idiot-while.html?utm_source=twitterfeed&utm_medium=twitter&utm_term=software+testing) and [here](https://tobythetesterblog.wordpress.com/2015/06/11/how-does-it-feel-the-difference-between-checking-and-testing/) respectively. I intended to think about this more back at the original tweet time, their blogging gave me the nudge needed.  

p.p.s I should add, that I believe its OK to say you are fixing check if you are changing the implementation of the algorithm, as long as those changes don't alter the original algorithm. Such as changing the data or updating some locators. Or even the url's. Things along those lines.