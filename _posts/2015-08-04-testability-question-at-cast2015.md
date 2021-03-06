---
layout: post
title: Testability Question at CAST2015
date: '2015-08-04T21:31:00.000+01:00'
author: Richard Bradshaw
categories:
- Community
- Conferences
- Automation in Testing
- Testability
- Automation Design
tags: 
- Testability
- Automation
modified_time: '2015-08-04T21:31:00.433+01:00'
blogger_id: tag:blogger.com,1999:blog-8318661666872903125.post-3229094255686374755
blogger_orig_url: http://www.thefriendlytester.co.uk/2015/08/testability-question-at-cast2015.html
permalink: /2015/08/testability-question-at-cast2015.html
comments: true
---

I was watching the live stream of CAST2015 earlier, in particular I was listening to Maria Kedemo talking about "Visualising Testability". Having done her's and Ben Kellys workshop at LetsTest, I was interested to hear Maria talk about this topic again, and also to see if anything from the workshop was in the talk.  

Wanting to get involved more, I posted a question to the twitter printer, which on a side note, is an awesome idea.  

<blockquote><a href="https://twitter.com/AST_News">@AST_News</a> Testers with programming skills, do you feel more should use them for increasing <a href="https://twitter.com/hashtag/testability?src=hash">#testability</a> when writing auto-checks. <a href="https://twitter.com/hashtag/CAST2015?src=hash">#CAST2015</a>
<footer>— Richard Bradshaw <a href="https://twitter.com/FriendlyTester/status/628650593507217408">@FriendlyTester</a> August 4, 2015</footer></blockquote>

If I could rewrite it, I would write. "Should testers with coding skills focus some of their time on increasing testability of the product/testing, instead of focusing on creating automated checks, which I believe is where the majority spend their time" sadly, that doesn't fit in 140 char.  

I believe they should, as I believe automation is just a tool. The most common use being reducing testers time spent checking, by automating those checks. Which I also believe is where most focus their efforts. However some testers skills are on par with some developers now, especially those occupying the role of SDET and such. So surely we could use those skills to increase some aspects of testability. For example, referencing [James Bach model](http://www.satisfice.com/tools/testable.pdf), someone with those skills could spend time improving intrinsic testability, altering the product itself. This could be adding in some logging they require, it could be writing some hooks to make accessing the system easier and much more.  

But for me, I want to see more testers focus on what James titled "Project-Related Testability". I encourage people with coding skills, testers or developers, to create tools that really support the testing efforts. For example, they could write tools for reading logs files, creating data, state manipulation, data manipulation and much more.  

Of course with any automation pursuit, it should be clear what is trying to be achieved and be aware of falling into the automation trap. If something it taking to long, will the value be returned by continuing or should you just accept defeat.  

Anyhow, I encourage all to watch Marie's talk once its published on the [AST YouTube page](https://www.youtube.com/user/TheAstVideos) and think about what tools could you create, or someone in your team create, to increase an aspect of testability.