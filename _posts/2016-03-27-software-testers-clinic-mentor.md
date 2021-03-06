---
layout: post
title: Software Testers Clinic - A Mentor Experience Report
date: '2016-03-27T23:32:00.001+01:00'
author: Richard Bradshaw
categories:
- Community
- Software Testing Clinic
tags:
- Coaching
- Mentoring
- Community
modified_time: '2016-03-27T23:47:04.733+01:00'
blogger_id: tag:blogger.com,1999:blog-8318661666872903125.post-6131949948090939326
blogger_orig_url: http://www.thefriendlytester.co.uk/2016/03/software-testers-clinic-mentor.html
permalink: /2016/03/software-testers-clinic-mentor.html
comments: true
---

I recently attended the first [Software Testers Clinic](http://www.softwaretestingclinic.com/), an initiative created by [Mark Winteringham](https://twitter.com/2bittester) and [Dan Ashby](https://twitter.com/DanAshby04). You can read more about the idea on their website.  

I thoroughly enjoyed the evening, especially the second half of the evening, where attendees were encouraged to actually do some testing. Now, as the sessions are aimed at people new to testing as well as people looking to expand their testing knowledge, the attendees are a combination of students and mentors. I was attending as a mentor. So the testing exercise was arranged so that 3 students were paired with a mentor. My first student was [Demetra Cucueanu](https://twitter.com/DemetraCucueanu), a budding new tester, proving to all that it's never to late to try a new career. Demetra is actively seeking a junior testing position. The second was [Bhagya Mudiyanselage](https://twitter.com/bhagyagdm) and the third was Joe McGuinness.  

The reason for this post is in response to the experience report created by Bhagya, you can read that [here](https://bhagyagdm.wordpress.com/2016/03/26/swtcwhat-is-testing/). An attempt to explain the approach I took with the students, as a mentor.  

The challenge set to us was simply to test [http://www.drawastickman.com](http://www.drawastickman.com/). We immediately asked them how long we had, and were told about 30 minutes.  

So before we got started, I asked them a simple question. Why are we testing this? Neither of us knew so we asked, the response was to learn more about testing. Drawastickman was simple a vehicle to aid that. We then briefly discussed the importance of knowing why we are testing something.  

So we got going by me asking "What do you know about drawastickman.com?". Turns out we/they knew very little, the obvious is all we knew, "it's a website". So I introduced them to the concept of a Scouting/Recon session. I was first introduced to the concept in the book Explore It! by Elizabeth Hendrickson, fantastic testing book if you haven't read it yet. The session is intended to help us set the context a little, specifically around the application. Ideally you would spend a full session doing this, so about 90 minutes to 2 hours.  

I believe it's very hard to testing something you know nothing about, and I mean nothing, all we had was a url. So I encouraged the students to spend 5 minutes, just exploring the application. Looking for things they can identify with. For example, immediately after looking at the url they realised it's a game. Joe immediately saw a link for a native mobile version of the game, could be an interesting avenue to explore. Bhagya went straight into the game, to see if she could get a basic understanding of how it worked. Demetra explored the sites navigation and discovered numerous forms that she thought could be interesting to test. Plus a whole lot more.  

After 5 minutes, I asked them to explain to each other what they have discovered about drawastickman.com, and I collated the list on a nearby whiteboard, I loves me a whiteboard. I then recapped with them about how quickly we were able to get a better understanding of this application. We went from a url, to a 10-15 item list of things we actually knew about the website.  

I then suggested to them, they pick something from their list or the main list to explore further. Something that was of interest to them. Explaining to them how this approach now sets the focus of their testing, it frames it. I introduced the idea of charters to them, again repeated my encouragement for them to read Explore it! We could have continued to explore and just shallowly tested things as we came across them, however I was keen to see them attempt to test an area deeply. So they all selected an area to explore further. The reason I was keen for this, was I attempt to relate it to testing in their jobs, where I assumed they would need to test deeply.  

I shadowed them for about 5 minutes, watching them all test, and a pattern emerged. No notes, or very little. So after another 5 more minutes of testing, I stopped them to discuss what they had learnt after just 15 minutes of testing now. They had all learnt a lot, however my earlier observation had come to fruition, they were eagerly telling me about what they have found, but the majority of it was from memory. There was even a few confirmations of this, such as "there was this one thing, but I've forgot".  So we had a brief discussion about the importance of taking notes whilst testing, and how they can help guide future testing, but also aid you in telling the story of the testing you have done thus far.  

They continued to test, a which point I decided to take the approach of chatting to them individually, to see how they were finding the approach of using charters. This gave me the opportunity to offer some one to one feedback and directly suggest some resources to them based on what they had done or were doing. Also giving them the opportunity to quiz me.  

One of the topics that came up was, when do we move on to the next charter? Time was short, so we had a brief discussion about it. We discussed the idea of feeling like you've found enough information, or that you've exhausted all the ideas you had. This allowed us a brief moment to discuss the relationship between charters, test ideas and actual tests. We then very briefly hit on the idea of heuristics and some popular mnemonics, I suggested some resources for them to explore, including [Karen Johnson's card deck](http://karennicolejohnson.com/2012/07/testing-mnemonics-as-a-card-deck-v2/) and [Test Insane's MindMaps](http://apps.testinsane.com/mindmaps/). Also with drawastickman being a public application I suggested exploring social media for comments on the game, as well as reviews in the app stores. These can be a fantastic source of test ideas for public facing applications.  

The final discussion we had was specifically related to testing drawastickman.com. If you're not familiar with it, you can draw a character with the touchpad or mouse, and the site will bring it to live, depending on what you draw. The discussion was about reproducing bugs, how could we reproduce issues we observe, seeing as re-drawing the exact same stickman would be tricky. So we discussed some ideas, such as recording the screen and using a mouse cursor recorder. Highlighting the use of tools.  

That's pretty much that. I feel in this instance that my mentoring/coaching went rather well. I could have perhaps let them test a bit longer than I did, however all the students seem really engaged on learning more about charters and sessions. I had a lengthly discussion with Joe specifically about using sessions in the workplace and encouraged him to google Session Based Test Management.  

I tried my best to be the facilitator of discussions, instead of telling them what to do. Allowing them to ask me why I was suggesting X. Such approach also allows me to collate more information from them, which my highlight a different approach I could take. Without the discussion though, it isn't really mentoring/coaching, it's telling.  

As a sole tester at the moment, it was great to be able to mentor and coach some testers, while they actually tested something. I really enjoyed the event.  

I would encourage anyone in the London area to check out a future Testers Clinic, regardless of your testing level, as you can participate as a student or mentor, both full of potential learnings. The link to their site is at the start of the post and details of the next meetup are on their home page.