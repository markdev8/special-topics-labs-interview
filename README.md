# Interview time with Jeremy

## Overview
To give you a better idea of "real" GitHub workflows, I want you to fill out the below interview.  Many open source projects have their source repositories available publicly on GitHub.  They want to accept contributions from anyone, but they also have a few requirements:
1. They don't want to allow direct push access to their repository, because they want to choose whether or not to accept the patch (perhaps they need to require a license agreement, or they want to make sure all tests pass before taking the patch)
1. They want to be able to give feedback on the patch before accepting it (perhaps it violates coding standards, or is missing tests, etc.)

For git repositories with these types of requirements, GitHub has the [pull request](https://help.github.com/en/articles/about-pull-requests) process. Pull requests let a third party propopse a patch to the repository, and let reviewers (either human or machine) provide feedback and request additional changes for the patch. 

There are multiple ways to make a pull request.  For open source development, adding everyone who wants to send a pull request as a collaborator to that repository is infeasible (even if there are fine-grained permissions to allow for "pull-request-proposer only").  So their pull request model more generally follows this pattern:
1. User Bob wants to contribute to project `next-best-thing` (which is publicly available on GitHub).  User Nancy is a "maintainer" of `next-best-thing`.  That means that Nancy has the rights to modify the repo (merging commits, rebasing, etc.).
1. Bob starts by [making a fork](https://help.github.com/en/articles/fork-a-repo) of `next-best-thing`.  That means he has a copy of `next-best-thing` in his GitHub account, along with metadata that "remembers" that the original source of this repository was the authority `next-best-thing` maintained by Nancy.
1. Bob clones his `next-best-thing` repo to his local development environment (in your case this would be your Amazon workspace, cloning either through IntelliJ or the command line).
1. Bob makes his modifications on his local copy (either on the default `master` branch or on a branch specific for this change).
1. Bob [pushes his changes](https://help.github.com/en/articles/pushing-to-a-remote) to his fork of the repo.  At this point, Bob can log into GitHub and see his changes.  He is now prepared to create a pull request.
1. Bob [creates a pull request](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork) that is sent _to the original repo_ that Nancy helps to maintain.  Note that this is different than what you will typically do.
1. Nancy reviews Bob's change, providing feedback.  Frequently, Bob will have to [update his pull request](https://stackoverflow.com/questions/9790448/how-to-update-a-pull-request-from-forked-repo) with more commits to address Nancy's concerns.
1. Finally, Nancy is happy with Bob's pull request and [merges](https://help.github.com/en/articles/merging-a-pull-request) it into the authoritative `next-best-thing` repository.  At this point she can decide whether she wants to keep Bob's full commit history, or "squash" it into a single commit.

## Getting Started:
For this lab, you should play the role of Bob in the Overview section above.  Fill out the Interview below, and send me a pull request when you're done!

For each question, please add your response to any other responses already recorded.  Your answer should be formatted similar to the following sample:

Q1: Is this a question?
* _Jeremy_: yes it is

Q2: What is the answer?
* _Jeremy_: Of course, the answer is [42](https://simple.wikipedia.org/wiki/42_(answer)).

## Interview
Hello!  In the rush that is the start of the term, I really haven't had a chance to chat with many of you.  So would you do me the favor of helping me get to know a bit about you by answering the following?  Please avoid one word answers... I want to learn about you!

Q1: So you're finishing up your time in this CSCC program.  Why did you decide to embark on this journey?
* _Mark_: I have always been interested in programming since my first experiences in middle school on TRS-80 machines. My senior year in high school I took a programming class, which was a brand new subject at the time. I wrote a quadratic formula program in Microsoft Extended Color BASIC on my TRS-80 Color Computer for extra credit, and the teacher accused me of plagiarizing. Not that I needed the extra credit, but I did have to defend myself on that.

Q2: I _love_ to travel.  Tell me a bit about your favorite travel destination so far.  What's on your travel bucket list?
* _Mark_ : I'm not that big into travel. I like the feeling of home. As a college student I did live in France for six months - actually turned 21 in France. I would very much like to visit Montreal (again), Belgium, and Brazil.

Q3: Name your favorite member of [The Beatles](https://en.wikipedia.org/wiki/The_Beatles), and your favorite Beatles song.  You do know at least one Beatles song, right?  If you are a Beatles fan, feel free to give me your top 5 or so.
* _Mark_ : I don't have a favorite Beatle. Maybe I'll say Ringo Starr as a nod to Seth MacFarlane's ["I lean" joke](https://youtube.com/watch?v=bkgLVOzJqaM) in Family Guy: Something Something Darkside. My favorite Beatles song might be "I Saw Her Standing There". I have the original "Introducing the Beatles" album and as a kid was more crazy about a friend's record: "The Chipmunks Sing the Beatles". I picked that up cheap on CD years ago, for nostalgia's sake. As an adult, I prefer the Beatles' voices, it turns out.

Q4: Do you have any pets? Species/Name/Details please. [Murray](images/Murray.jpeg?raw) wants to know... (he's not as smart as that picture makes him seem). 
* _Mark_ : I have a couple of aquariums going with freshwater tropical fish. Two months ago I lost my darling Chloe, my little buddy, my little girl. I'm still working on getting over that one. She was a chocolate cocker spaniel with tan eyebrows and highlights at her feet. Even when she was feeling out of whack on our last walks in the park, people would smile at seeing her and tell me how pretty she was.  She was my sense of home.  I also have a small cat, kind of a cross between orange and gray tabby. She only has one eye, but that doesn't stop her from catching mice.

## Submitting Your Work
Once I have merged your pull request into my repo, please submit your repo along with a screenshot of your pull request in Blackboard.

