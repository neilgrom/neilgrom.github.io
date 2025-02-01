---
title: "Organization and Automation for Working - Tips and Tricks"
date: 2025-01-31
tags: ["anecdotes", "travel"]
---
Hey everybody! I'm back, and for the first time in a while, seems like my life has settled down for a few days. Was in Baltimore Monday/Tuesday for my project which is nice that's over, I was definitely feeling bummed out over my couple days I'd spent there coming off the back of the choatic travel with the month long trip before.

I'm sure I'll make some posts about my trip from this last month (he says, naively, making another post not talking about that one), but here's a quick summary of why I was so exhuasted. I spent Christmas visiting my family in North Carolina, which was great to see everyone. 
After that I went back to Indy for a few days, then started my month long adventure consisting of
-1 week in California visiting my girlfriend (Santa Cruz, San Franciso
-2 weeks in the UK (mostly work, running around Eastern England)
-1 week in Austria visiting a friend (Vienna, Graz)

So to top all that off with a trip to Baltimore upon my return after being gone for a month was exhasting, but it's over. When I got back yesterday, I started thinking about organization, optimization, and work flow from my desktop out of my home office.

Obviously with my month on the road, it wasn't an optimal working setup, but I travel with my portable monitor so it was nice to have that for my trip (until I broke it sleepwalking.... different story). The efficiency you get out of a second screen is unmatched and I highly recommend it for anyone who doesn't work out of the same desk all the time. Even if it's just for your home setup.

I wanted to take this post to talk about how I set myself up efficiently with how I structure my computer and my workflow and the tools I use to make everything go as efficiently as possible. Maybe I'll turn this into a better organized post or guide one day. Maybe I can title this post "How To Organize Your Computer to be More Efficient" for extra clicks...

So here's a summary of the different tools I use on a daily basis and what my recent restructuring has told me about my workflow, along with tips and continued improvements I'm making. For some background, as a consultant, I need to be easily able to pull documents, information, and web pages within a moment's notice once my brain fires on what I need to do, so let's dive in! 

1.) Google Chrome Bookmarks
If you're not using these already, you really need to start. Not only does bookmarking a link give you one-click access to your most utilized pages, but if you clear your history, you can type in the bookmark name up top in a pinch, which is handy for my brain a lot of the time. I have my work computer structured by my different projects/base/essential sites in different folders so I use that at least everyday.
Personal Computer Bookmarks Bar Layout: ![image](https://github.com/user-attachments/assets/bb4e7f94-5aa7-4b73-a2e7-9c533c504f0d)

I'm also interested in diving more into utilizing tab groups in Chrome, which are pretty much the ability to pull up multiple tabs at once with one click. Cool right? This also allows you to keep them organized and you can close the entire tab group and re-open it with a single click. My previous execution of this failed because I opened a bunch of client sites at once and they all used the same authentication and errored out over each other... So tbd on this one's effectiveness for me.

2.) Remote Desktop Manager
Holy god this one is literally a miracle for me. We have soo many different clients to connect to and keeping track of all of those as different IP's and passwords and locations is a pain in the butt. While other people while probably use this tool _actually_ effectively, I use it just to dump the IP and location and access instructions for each site which greatly streamlines the process of accessing multiple sites at once.
![image](https://github.com/user-attachments/assets/f3455863-a598-4b28-9ede-0b2a03667289)

3.) Outlook Efficiency
I think I could do a whole post on how I manage my outlook. The big thing I've started doing recently is filtering emails as soon as they hit my inbox. This has made a massive improvement for me, because although it takes a bit of work up front, I can take some time to review the open items I still need to do based on what's in that folder. If I don't have an email for a specific task, I will forward the email to myself so it shows up where I can see it, which is nice.

I also have my folders filtered by project, which is great for easy acccess to project information in a pinch. I am realizing I have some cross-over so some items aren't in the folders I'd expect them to be, so that needs to be ironed out. I've also got a couple other folders, such as "Helpful Emails", "Template Emails to Send", and some automatic filters that take certain things out of my inbox so I don't have to manually move them.

> Looking at you, all of the sales emails I get for projects I will never be involved in

The auto-filter rules also have a lot of potential in terms of optimizing important emails you don't have to read right this instance, like filtering product release notes, or non-essential email alerts to different folders where you can review them later if needed.

4.) To-Do List: Sticky Notes/OneNote
As I began my consulting career, I found myself taking numerous notes about every single little detail, which overall may have enhanced my learning, but I've never actually revisited. I do revisit code snippets, old project setup, and functionality, but none of that is really done through OneNote. I use it as a sort of initial thought dump/landing page, and keep a centralized "To Do" list of everything that I can think of to do. 

I keep a more (wow I just learned how you can insert emojis on accident 🐤) daily sort of list on my Stick Notes App on my desktop to monitor. When I'm at home, I dump, similar to my sticky notes app, everything I need to get done, then organize it by importance and finish what I need to do. I think I've found a structure that works well for me here.

5.) Basic Windows File Structure/Folder Organization
While I feel as though my work file paths and locations are fairly structured behind different folders, I realized my desktop is extremely poorly optimized. I can still get exactly what I need when I need it from where, but it often takes clicking through several folders to get there. Because I'm always plugging/unplugging my computer, working on a portable monitor, and never on the same setup in terms of screen orientation, I don't really use my desktop, like EVER.

Which is crazy to admit. I have pretty much everything I need either on my task bar, on the search bar, bookmarked in Chrome, or in a folder somewhere. So I've revamped my home screen this past week to actually have specific shortcut folder I always use pinned to quick access and present on my home screen, so we'll see how it helps. I feel as though I'm always working with probably like 10 different apps open, so my homescreen is never visible hence the problem.

6.) Shortcuts/Automation
![image](https://github.com/user-attachments/assets/d2d6aef0-1c2e-40c0-afd4-9094490ae104)

Now, the real reason for this post is what I spent several hours today working on, automation and efficient improvements. I realized I've been slowly modifying my systems to work for me and I came to the conclusion that there are a ton of different commands that I'm using ALL the time. For example, a basic SQL select statement where I always join the same two tables together, like as follows.

`select * from table1 t1
LEFT JOIN table t2 on t1.ordernum = t2.ordernum
LEFT JOIN table t3 on t11.productcode = t3.productcode`

I originally thought, "What if I could type a customer name and have my computer default me to that customer's splash page in a chrome tab?" So I got curious, got exploring, and realized how easy it would be to setup a bunch of shortcuts to do that AND shorthand automation for pulling important code/information in flash.

I am totally someone who will spend 2 hours learning how to automate a 1min task, but this really has some potential. I probably type that query in (or some form of it) at least once a day, which takes at least a minute to type. Using the software I'm trailing called TextBlaze, you can create your own shortcuts that automatically resolve into text. Meaning, I can create an sql bank of all my favorite queries and immediately pull them.

It's exciting/fun in a way because I feel as though I'm writing my own shorthand language at the moment. Like to get that above query snippet, I can simply type t123j, which would default into the standard join statement you see above. That's part of the automation I have unlocked and oh boy, the potential is crazy. I also have some email templates setup that look like this when I type in SchedCall which allow for filling in text.

/SchedCall
![image](https://github.com/user-attachments/assets/6fd4ed09-12b3-49e8-9900-c8d5809e65fc)

As a consultant I do a ton of check-ups/check-ins so I wrote up a few template emails today and I will slowly be adding to this bank as I go. Here's what we've got right now as some different shorthand/functionality and I'm very excited to see the power I can pull from this.
![image](https://github.com/user-attachments/assets/3bbc1604-8e49-41a1-baff-6f5bc6bdd71e)

The next step is to look into some software that I can go directly to certain browser links on, and build that out so that I can type %Customer1 and immediately get sent to a splash page of theirs. I'm still exploring the best fit for that software.

That's everything I've got in terms of how I enable myself to do my job better/faster. I'm excited to see the gain I'm going to get from TextBlaze from shorthand to text inserts to pulling up formatting for different sql queries as I get started.

Here's to working less and getting paid the same amount! (Hopefully)
-nhg


