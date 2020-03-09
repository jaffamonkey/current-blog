---
title: "Testing journey in BDD"
date: 2020-02-01T12:35:11-05:00
showDate: true
draft: false
tags: ["bdd","testautomation"]
images:
    - /posts/bdd.gif
---
_[View this article on Medium](https://link.medium.com/Giz5jBjrb4)_

> The sooner we stop applying pass/fail criteria to software development approaches, the better.

Firstly, this is all from my real experience - not from other articles (apart from some paraphrasing of BDD definitions), social media or formal texts on the subjects. I learn in different ways, but most concrete learning is in real situations.

I do take exception to generalisations, and damnit there are hard to avoid. But here goes …
Yes, we all know how things should be done, but when it comes to the crunch (real work), then you always have to be adaptable. Compromises always have to be made, processes needs some pushing (and challenging), people need supporting. Or you could be the project bore, which helps no-one ("that's not real [blank], just don't ask me to fix the problem").

This article is relating to the contracting experience, from contractor perspective. It's an important first idea to process, as a contractors remit and view, is vastly different from a permanent work. Office culture more directly affects permanent workers and by default it is always on lists of employee concerns. But I am hired to work on projects(s), not to "fix" office culture issues. But I can improve the project processes, and be an optimistic positive force within teams.

Office culture, hierarchy, senior management can all be hurdles. But hurdles can be navigated, or even removed - a lot easier when you are a contractor, as you don't have to pander to office politics so much (though you can't just ignore it). Contracting means working in many different company environments, so I am adaptable and less inclined to be a follower. When I am hired, I assume it is for my skills and experience, not my ability to blend into the office.

## Test Automation

I have coded test frameworks from scratch, migrated tools midway through projects, used a variety of tools and helpers. My longer background was in QA and Test management, so I am definitely not a standard tester geek. I start test automation as lean as possible, then add tools/helpers, as/when needed. This was learned through some bitter experience. Once you start dipping into opensource world of test tools, there is a "first time in a sweetshop" feeling.

My experience in test automation goes back to 1998, but will keep it brief, as the real interesting stuff didn't happen until 10 years ago. In 1998, I was given task of testing using a unit test tool created by Unisys (creatively named "Unittool". The next (horrendous) experience was WinRunner, test automation tool for desktop software. And then monstrosity that was/is LoadRunner. This partly drove me down the Test Manager route, as the experience was off-putting.

Then in 2006 I happened upon FitNesse (the wiki front-end for Fit, a test framework by Ward Cunningham), and Selenium soon after. It crucially led me into world of opensource test tools and also introduced me to DSL (domain specific language). A few years later, I was using the Fitnesse/Selenium framework in more earnest, at a company trying to move away from Visual Studio IDE test tools. It was by using this combination, and exploring developer web communities that finally led me into "BDD world" which was gaining popularity in dev communities and more mentions on social media.

Test automation has always been involved in my testing work to varying degrees, but it took me a few years of dabbling before I really threw myself into it. The real inspiration for not only test atuomation, but how it fitted into the larger picture of the build and deployment pipeline, came from BDD world. However it was about direction and journey, not actual BDD itself.

## What is BDD?

BDD (Behavior-Driven Development) is an extension of TDD (Test-Driven Development) that uses a domain-specific scripting language. Most commonly, Gherkin is used down to the pure natural language syntax, and therefore more appealing/accessible. Gherkin is plain language parser originally stemming from Cucumber project, but now a commonly supported package by other frameworks (such as Behat), and relatively easy to implement yourself on any framework. This specification format can result in better acceptance criteria for a feature, as the spec IS the test. I do say "can", because as with any approach, it's possible to completely balls it up.

An area that is over-debated too many times with BDD is does it matter how the "Behaviour" is fed into the development process. Some would say there is a strict process of creating feature files with examples (scenarios), then automating them . Then there is always multiple distractions with tedious cry of "that's not all the testing though!". Yes, we know, we were talking about BDD specifically. The approach of specifying by example as the focus was on writing of requirements illustrating with examples, i.e. thinking a user story through more thoroughly, to fully convey needs. We have (more or less) evolved slowly from a business analysis style of use cases with alternate flows.

## My role on BDD projects

Although I have been on 9 "BDD" projects, my actual remit was more diverse as I had the advantage of many years in test/QA management. In testing, we were always concerned with user behaviours so it was not a big leap in that sense - it was a matter of factoring in an extra "layer", and getting more integrated into development/devops territories. This was understandably a big leap for too many testers. I will outline that more in the case studies articles I am writing, to follow this article.

So as well as technical tasks I was generally expected to contribute to overall Quality Assurance. I was most acutely aware of the question "what is the purpose of this task I am doing". Over the last 10 years my Quality engineering remit on BDD projects has been (in whole or in part):
* Steering the tool selection (usually with the developers)
* Building test frameworks (for functional and non-functional testing)
* Writing Test strategy (a constantly evolving document)
* Devising/improving bug reporting
* Defining the way requirements are devised and managed
* Creating tests before development starts (sometimes too challenging)
* Adding further tests to cover exploratory testing
* Integrating tests into build and deployment pipeline
* Non-functional testing (whether asked-for or not)
* Mentoring, of PO's (Specifying by Example), developers (on BDD), and other testers.

It looks like a long list, which is why being optimal in anything you do is critical. It's an OCD of mine - I hate wasted time. In my work capacity, this proves to be a positive bonus.

## The Business and BDD

Regardless of what the business think is happening in the way of development, they only really have windows, as they are largely interested only in what goes in, and what comes out. Or (toxic-style) they are treated as "not welcome" - not in a deliberately unfriendly way, just people minimising what they perceive as their "interference". Still goes on. Any situation client-side can be accommodated. It's easy to bleat about dealing with office culture issues, but as long as the reliable core team is intact, office culture does not needlessly have to impact the day-to-day development.

Business latched onto BDD marketing, mainly down to the appeal of Gherkin of course, the format for writing specifications. Gherkin is a Domain Specific Language (DSL). DSL has longer history than BDD, and dictionary definition is a computer language specialized to a particular application domain. In BDD, this is applied using natural language (to describe behaviour and expected outcomes). Tools such as Cucumber and Behat enable the Gherkin to be executable, i.e. you can map code to Gherkin step. Simple stuff on the face of it, and to management it looks clear and straightforward from their (Gherkin) side. Until they start writing it.

The DSL doesn't solve problems and business quickly realised it demanded more skills than simply something that could fit on a post-it. The business needed to learn how to convey requirements clearly by means of using examples. And this is where some get lazy, some will struggle, but some will get it. Usually Business analysts and UX people get it quickly, as their work already involves identifying/defining alternate flows/possibilities.

There are rarely 100% dedicated PO's/Business Analysts, as they are usually stretched across projects (sometimes related, sometimes not). Sometimes not even vaguely qualified, but could still represent a good standard user viewpoint. If you have a PO with not even basic stakeholder knowledge at all, you can flag this up as you need someone qualified to say when something is Done.

Client availability can be a problem with interruption to flow, purely down to late sign-offs, or problems flagged up late. This of problem should most definitely be mentioned, as it can have serious impact on a project. Conversely, don't get caught in trap of hammering away at office culture problems.

The idea of having something like Gherkin as the DSL, is the whole team is capable of developing the language of project communication, the language of the business domain. The PO writes the feature, and reviewed as a team. The DSL will not evolve if only one person is working on it. This is where people can get lazy, because in order for the language to grow, all must have an opinion/contribution.

These are the kind of questions (not an exclusive list) for people to consider, when reviewing the DSL:
* Does the over-lying user story make sense?
* Do the scenarios make sense?
* Do the steps themselves make sense?
* Are the steps too granular?
* Are less/more scenarios necessary

From my perspective, it is down to me to directly deal with the business side of the project, as it is quality work that ultimately gives the business confidence in the software development process. These days, they are interested in the actual process

## The Team and BDD

The reliable core of the team that doesn't change is Scrummaster, developers, and if you are lucky dedicated UX/UD people. This group can easily work towards working in a close-knit way, experimenting/improving as development progresses. The business provides delays, and I don't mean that in spiteful way. But they do. They are the clients, the people who will get worried/anxious, the ones who will change their minds. And we are there to help them, not demonise. It's their concept and budget, and we deliver what they need (key word there, "need").

I am more than happy to help the POs and business analysts to integrate more into daily development process, but a life truth is that some can't or won't be helped. There is an old phrase never help people, who don't help themselves. It's a mindset thing, some people are happy to be looked after the whole of their lives. You get all sorts of personalities in offices. I have little time for people like this, regards work. I have a few friends like that - no-one is perfect, but in working context, it's needlessly distracting.

This brings me neatly to another thorny point - when do you vocally complain and/or escalate. This is where the daily standup is useful, and you have two minutes to highlight what you consider blocking issues (which is sometimes people). Be open, be vocal, but if you start following an company escalation process (basically going outside of "the team") you may end up embroiled in company politics and even some resentments. There is little value in a contractor doing this, for the contractor or client. The value we bring is leading by example, our experience, our opinions and mentoring others if necessary. A good Scrummaster and half-decent PO should be able to deal with most problems.

## BDD Buzz

The BDD buzz brought an interesting angle to testing work, as by default testers are a good conduit between business and the techies, the holy grail of specs that mean something to both business and technical people. Developers became highly suspicious of BDD (as it was sold, with the pretty Gherkin) as they knew there was high-risk they would have to maintain these feature tests as well. It can be done, but this is where a tester who can code is a real asset on the team (effectively, they are another developer).

For a few years it was a messy business in most companies that tried it. Commonly dropped with reasons such as high administration or total lack of business engagement. Both are lazy reasons, and a common reaction from someone who not only doesn't understand basic BDD principles, but also disinterested in finding out more. This is where your employee has just cost you one of those Agile consultants, to bounce around your office and sing about it. BDD was sold as snake oil, in common with Agile, Scrum, Lean, Kanban etc.

The "Definition of Done"(DoD) and the usual meetings circus around the topic usually will inlcude "green" feature test(s) as part of the DoD. This will be on environment seperate to build environment (one that business users have access to).

BDD approach involves more than a 3-liner user story. That helps development in the long term, as it means they get clearer directives in the examples. But you know what, it doesn't matter that it's BDD. Noone goes around every day talking about BDD. It's generally part of the sell, but in the working course of a project, it's about "tests first". One of my first investigations when I join a project, is if that BDD layer is any use, but generally people seem to like to have it around once it is introduced. I started referring to "Specification by Example", because a lot of the problem was managers had been sold the BDD tools as BDD, rather than focus on what was relevant to them about the development approach.

## The Gherkin

Tediously on social media, the first thing most latch onto when blowing steam about BDD (based on little or no experience, as far as I can gather) is the Gherkin, thereby completely missing the point. Gherkin is never is the problem, it's just a format. Skills in writing requirements is still woefully underestimated. People with business domain knowledge are vital, but no point if the person writing requirements ignore or misunderstand that input. Sometimes the app doesn't warrant much imgaination from a PO, a less custom app. But mostly you need a PO that not only can specify a feature, but who manages expectations of stakeholders. They also need to be confident in what they consider "Done" to be.

People focus on the popular BDD Gherkin format, because it is both easy to champion and easy to criticise. We have all seen badly written Cherkin, just as often as we see badly written requirements. Underneath every Gherkin step, there is always code. Remove the Gherkin, and the tests still run and still make sense because the natural language step is in the function names. I try to focus of specification by example, when taking business people through it. Even business analysts can get tied in knots with Gherkin, even though I point out their methods are not that far off already. User cases/alternate flows fit very neatly into the Gherkin way.

## Conclusion

I started in period (late 1990's) where business analysts were still standard on projects. Their style of using use cases to illustrate core requirements more fully, came close to what BDD was trying to achieve, which is clearly defined test criteria, which drive development. A lot in software development has not actually changed, it's been mostly a juggling act. Throwing all the balls up in the air, and see how they land. That didn't work how we expected? Let's throw them up again. And so on.

The success of BDD-labelled projects success comes from bringing the team closer together. It also seems to attract certain kind of developers, usually ones who are fans of TDD, at the very least developers obsessed with keeping their own unit tests in order. And usually more vocal with opinions. After all, if you are selling up to an approach which demands more is done, before actual coding starts, developers need to be confident to voice concerns at any stage and be transparent with their work progress. That is not all developers.

Actual BDD might fail early or never properly start, but you can be sure requirements will be clearer, and there will be good automation at all levels of that dull-looking testing pyramid. When people think about whats needs to be tested, or thinks about what test would warrant accepting a feature as done, it broadens their minds. A simple user story can become more complex but also more valuable. And more importantly more correctly implemented sooner.

For BDD to "work" at all, the business need to be proactive with writing BDD features/scenarios, and secondly developers need to be able to converse with PO's, during development of a feature. Oh, and you need someone dedicated to quality and testing, because having a dedicated person for this is the perfect way to provide support for the whole team in the BDD way of thing, not just developers.

