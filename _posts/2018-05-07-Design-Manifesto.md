---
layout: page
title: Design Manifesto
subtitle: Sous Shopper
---

# Overview

I’ve learned a lot of lessons about design this semester, both in class and through the course of working on this project. Some of them came through satisfying successes in implementing the concepts from our readings, but many more came from making mistakes and correcting my assumptions. While I feel it is a bit early in my design career to write a manifesto on human-computer interaction, there are five main points I think are worth writing down that I will continue to keep in mind as continue to better understand UX design.

Software engineering is a skill that can be used to create great evil, therefore software design must be grounded in ethics.
Accessibility is key in all design. You aren’t really thinking about user experience unless you’re considering the experience of *every* user.
Don’t decide what’s best for your users until you’ve actually asked them. You might be surprised how often you’re wrong. 
When prototyping you should cut yourself some slack on aesthetics so you don’t cheat yourself (and eventually your customers) on design features.
Iterate, Iterate, Iterate, Iterate, Iterate, Iterate, Iterate, Iterate, Iterate,...


# Ethics 

At the time of writing this post, the news cycle is just starting to get past the Cambridge Analytica scandal at Facebook. If someone happens to dig this post up in the future, then barring the complete collapse of society there will probably be some other recent scandal involving software which does something that isn’t illegal, but isn’t entirely ethical either. The law is generally slow in catching up with modern technological advances, and lawmakers usually do not even turn their attention to these new avenues for wrongdoing or tragic accidents until something very bad happens. Therefore it is our jobs as designers and engineers to focus on building ethical products and to be proactive in sniffing out any exploitable errors.

In Sous Shopper, our team was thankfully working on a fairly low-stakes project. Due to the nature of our app, we were not handling much sensitive data from our users that one might collect in a social app. However, we are committed to finding any potential for abuse in our creation. For an app based on nutritional education, [there is potential to mislead users in a way that can be seriously harmful.](https://ac.els-cdn.com/S0271531716302081/1-s2.0-S0271531716302081-main.pdf?_tid=c47a3700-b8d4-42a8-ac7b-512cb2fd6a47&acdnat=1525663144_c01894833d02272a1e61d54ac2668ec2 “Nutrition: ethical issues and challenges”) Thus, we have strived to be as objective as possible in relaying information about produce without sending users into unproved diet crazes or biasing users toward any particular food industry.

# Accessibility

One thing I’ve learned through the design process of Sous Shopper is that accessibility is an area in which design can almost always be improved. As a designer it’s very easy to think “I know what ableism is, and I know that it’s bad. I would never build something that was inaccessible!” No matter how considerate or socially conscious someone is, there is always room to overlook the obvious if you do not take the time to assess your design from perspectives of every group that might be affected by it. This kind of hubris is what leads you to make a big deal about accessibility during the in-class discussion, and then create a loading splash for your app which is virtually invisible to colorblind users.

![Sous Shopper loading splash next to a copy of itself with a grayscale filter applied. The grayscale version is barely legible.](/jsmilan.github.io/img/SousShopperLoadingScreenColorblind.png)

Yeah, that was embarrassing. Sous Shopper has also been struggling with how we can make better use of alt-text to help with that fact that most of our information about judging ripeness is conveyed visually. In our defense, most of the information we could find online about judging ripeness is based on visual cues such as color, but that just means more research is required to learn how best to discern ripeness without relying on sight, and then how best to convert that information into language. An important takeaway is that information such as this is valuable to all users. We do not harm any users by paying attention to accessibility, we simply remove our own ability to cut corners.

# Listening to Users

Before we can begin to understand human-computer interaction, we must strive to understand how humans interact with the problems we want our computers to solve. For this reason I am eternally grateful to this class for teaching me how to conduct interviews and contextual inquiries. So many ideas in Sous Shopper came from test users who had no idea how much they were contributing to the design process. 

One notable idea was the concept of a ripeness slider. Prior to our contextual inquiry we thought of ripeness as a binary, but after observing various people’s grocery shopping habits we realized that many shoppers have different preferences or intentionally buy under-ripe produce to let it ripen between grocery shopping trips. This is a fundamental part of grocery shopping, but our whole team missed it because our heads were already filled with big-picture concepts that were easier to imagine. Only by observing an outsider were we able to gain insight into this sub-problem.

It is hubris to assume that a lone designer could figure every constituent task associated with their problem in a vacuum. By observing users familiar with the problem you want to solve, you gain access to new perspectives and years of experience. 

# Low-Fi Prototyping

It’s good to have pride in one’s work. I sometimes wonder if anyone would ever get any creative work done if not for our egos. When we finish a project, we want to look down our creations with the satisfaction of having made something that looks good. But pride is also a sin (the deadliest one if we are to believe Dante), and it can hinder design much more than it can inspire designers to do good work.

The paper prototyping stage of this project is one of my few sources of regret in this project. We wanted our prototype to be interesting and unique, and spent too much time on its implementation. The result: a reasonably fluid scrolling system and many hideously underdeveloped features which we were not able to test by the time we had to put out a hi-fi prototype. 

![GIF of the scrolling system in our paper prototype](/sousshopper/img/PaperPrototype/list_swipe.gif)

That might be a satisfying GIF, but at what cost? We were so focused on making our paper prototype feel like a phone app that we built a design that made it incredibly difficult to add additional features. Our cardboard phone fit nicely in the hand, but our commitment to that superficial design goal hindered us in swapping out pages to effectively simulate using our app. There was no reason for us to try to create a high quality experience out of this prototype whose purpose was to ignore aesthetics. 

Paper prototypes require enough work to draw every necessary page by hand, you’ll do best if you avoid further complicating the means by which you convey your design. Besides, you will regret having put in the extra effort when the time comes to modify your design. Which brings me to my next point…

# Iteration

As a computer science major, when I hear the word “iteration,” I usually think of for-loops. Simply put, execute the code inside the loop for a specified number of times. But I think the iteration in design is more akin to the structure of a while loop. As long as a condition is met continue to iterate, each time changing something to get us closer to exiting the loop. 

The point of my clunky metaphor is that there is no set number of tries that will fix a design. The best thing that can be done is to modify and test your design as much as you possibly can during the development period. No idea is born fully formed from its author’s head, it needs time and experience to be molded into something useable. And iteration is the steel that sharpens innovation. 

One purpose of iteration is to point out simple mistakes that are easily glossed over. In our original paper prototype, we carelessly omitted back arrows and favorite icons because we were too focused on our main features. This was a common mistake throughout the class, and most systems are large enough that small errors like this are inevitable on the first try. Even before testing our designs on users, we must give our designs heuristic tests and continue to iterate until we have eliminated all obvious flaws.

Another reason to iterate frequently is to help oneself avoid the sunken cost fallacy. For example, when we began designing Sous Shopper’s UI, we quickly grew attached to the idea of using “pantries” as a metaphor for categories. If this section has taught you anything, you should know metaphors are not exactly my forte. This design choice confused many users, and rapid iteration allowed us to nix pantries before extended the metaphor any further. While changing and presenting your work repeatedly can be exhausting, it can save much work in the future and open you to many more opportunities for improvement.
