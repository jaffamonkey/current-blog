---
title: "BDD Project Case Studies"
date: 2018-02-01T12:35:11-05:00
showDate: true
draft: false
tags: ["bdd","testautomation"]
---

# Case studies

#### Always getting it wrong

> If you are contracting for many years at different companies, expect a few embarrassing tweets in your history. That is why I balk at the term “expert”, as every “expert” has the same history.  We all jump to conclusions, make bad assumptions, but hopefully we learn quickly (I try). I still cringe at stuff I posted last year, no amount of experience can stop you making mistakes. With every contract, there is always something I could have done better on the previous one (whatever the success level). I have followed some bad directions, but I never waste too much time down rabbit holes for years now.

The case studies can be loosely categorised as the following.

* Close as damnit
* Not strict BDD but specification by example is followed, and bdd tools used.
* Not strict BDD anspecification by example is followed, and bdd tools used.
* Not even close

## Industry: Finance (2011/2012)

#### wtf was I on?
_Tweet: Oct 20, 2011_
> Just switched from #kanban project to #bdd one -wow it feels so much slower!  Even a Sprint feels too long these days :) 

#### Oh ffs ...
_Tweet: Oct 20, 2011_
> I had recent experience with #BDD - it doesn't seem that far off #TDD though - am I missing something?

I first came across BDD on a C# project for a small Elections and Claims web app (I still have no idea what claims and elections are). Up to that point, I had been working on several projects, using the Visual Studio tools for test automation. Project Management was purist Scrum, but there was room for Agile development practice at least. 

The development team on another project had brought in a BDD tool Specflow, and were very much it’s champions. However on closer inspection I saw, what I have seen several times since with these setups - outdated features and a lot of failing tests. Anyway, back to the project I was one where Specflow was the tool.  

I had already worked with Fitnesse and some DSL plugins, so was aware of concept of natural language driven tests. Less user-friendly than subsequent tools, but I did like the style of writing accetpance tests that more clearly illustrated for eny audience. 

A lot of the BDD tests were backend and at the time my C# skills were enough to code UI tests, but otherwise light. The developer was helpful and enthused on the testing side also, and we worked almost in constant pairing mode, with the business analaysts on hand answer questions or create test data. 

It felt slower than what I was used to, because up to that point, I didn’t work so much with others devising acceptance tests. Or spend as much time on them, Since I started, devising tests based on business (and sometimes system) requirements was the norm. But it was more of a formal mapping process from analysis document to test cases.  

This way felt odd, but good. Odd, because I plain wasn’t used to this way of working. Good, because of course I had more assistance to write the tests, from both business and technical team members. 

Once the first set of BBD tests were written, and because the team was small, it gathered pace faster. It was not Gherkin, the step text was in function title.  Gherkin became popular purely because it provided a route for the business to get involved with BDD. 

After that contract I really made decision to focus more heavily on the tech side, and leave the test manager contracts behind.


## Industry: Creative (2013/2014)

#### I am almost falling out of my pulpit.
_Tweet: Aug 28, 2013_
> #BDD introduced me to a testing world, where tester can be more integral. Not for the faint-hearted, or those not willing to learn MORE.

#### You can tell I love the BDD label
_Tweet: Sep 2, 2013_
> That what makes #BDD so good :) Keeps development on track of what customer expects. i.e. Automated tests driven by requirements.

The good one at OPG
Team contribution to writing features: Good (All)

I had significant career gap after KPMG, as realised a senior technical direction was the best for me at that point. QA/Test Manager roles had always had a degree of hands-on tech tasks, and I found that more satisfying.

What was strange was that I was hired on my newly acquired self-taught skills using Behat. And my wonderful personality, naturally :) I chose Behat as I was already very familiar with php and javscripts also. CucumberJS was a very new product at that stage, so I chose the more stable tool. So I threw myself into self-teaching more in-depth about test engineering,  I learnt using Linux CLI whenever possible, ignored all UI tools and helpers. This way was harder, as I really had to understand the whole damn thing, nothing to make it easier. My choice, and I enjoy the challenge anyway. Would spend whole day with terminal windows open, and little else.

Although well versed with PHP and coding tests, the Behat/Gherkin part was a learn as I went exercise. But we all do that, learning is a skill and commonly that skill is very valuable. So I wrote the Gherkin, with some help initially from POs but they struggled (though did join in a few months in, once they got into the swing of it). So until that point, they contributed by at least adding descriptive scenario heading. This is all part of people communicating and trying to find common ground to make process clearer and easier.

What made this project a total joy to work on, is that after a scrappy few months (and a lot of hard work building up Gherkin library for PO's to encourage them), BDD diriven by Gherkin requirements was working. The PO's fully got on board with adopting this format, and Sprint planning was a series of clear scenarios to which developers could usually provide instant feedback. The developers themselves were a very gregarious and opinionated, transparency was high. There was a Scrummaster who delighted in his role. It was a good mixture of people - the most important key to success on any project.

Admission, I followed that crappy “Then I fill in this with that”, but only in early few months. I added code to test API (outside of the UI test framework), ran all on build server in parallel. I added automated light performance, accessibility and OWASP security checks (dev always appreciate some NFR feedback). The Gherkin matured over time, and at end of 14 months, I had a set of around 70 Gherkin steps with a few comprehensive e2e tests running regularly. I enjoyed the work, and my php coding improved rapidly. I value the CLI learning experience.

On technical side, was a less straight path one. The project started out as a Zend framework, with UI layer yet to be decided. The front-end went Angular over several months, so in fact the tools used were not the best matched. BUT it really did not matter. The only constriction I had with a straight Behat/Selenium setup was it could not tell when a page had fully loaded. I managed to hack this a little, but as the web app got more complex (heavy-duty numerous forms, it got unreliable, so relied on the old favourite of setting max page timeout, which does have added benefit of highlighting slow loading pages.  

In the last few months, did attempt migration to CucumberJS/Protractor, but in 2013 CucumberJS still had some issues of it’s own. Sometimes you will only swap soap for shampoo. The ideal (in hindsight) would have been Jasmine/Protector. Jasmine syntax still has steps, but that detail in all in the code itself.  Old style BDD tools, if you like - the developers had this stuff before the business fell in love with Gherkin. Gherkin is a layer, and it is removable as the functioning code lie underneath. Tools like CucumberJS enable that Gherkin to be executable.  A big lesson after 14 months (one of my longest ever projects) was not to get too wrapped up in Gherkin. There are so many ways to write it really, and so many opinions. But if your team understand purpose, and importantly the business see the value of it, why not use it. 

## Industry: Civil Service (2014/2015)

#### Utter vague bollocks
_Tweet: Jan 5, 2015_
> After mild #BDD comedown last year, following the philosophy of “Begin with the end in mind.” [Stephen R. Covey]

The lean one at HMRC
Team contribution to writing features: Good (Devs, Test)
Room to play, and we had a lean team. The project was a straightforward career management website based on the Symfony framework so still within php.  I had taken time to tidy up framework from last prokect, and was in a good reusable state.  Lesson here is only build frameworks if you are going to reuse. 

From Sprint 1 (can we drop the Sprint 0 bollocks, please), BDD was applied 100% with no feature moving forward in Sprint planning without the clear business acceptance test ready-to-run. A lot more communication involved, but luckily we were all a very communicative group who didn’t mind being interrupted (we all can waffle). 6 sprints of perfection, and a very happy PO. Unfortunately as is the way of business, other factors meant essentially the project was put on hold.

## Industry: Mobile (2015)

#### Horrible realisation idiots had got hold of BDD
_Tweet: May 17, 2015_
> Oh no! Realised sales people have now got hold of #bdd. Just ignore them & they may just go away :) Or could be the beginning of the end.

The BDD tools, but not BDD (Test)
Team contribution to writing features: Good (Devs, Test)

A project fully committed to Behat with webdirverio, though the Gherkin was large and unwieldily and test framework had suffered from too many playing at it. So I felt like a repairman for the first few weeks. Then had a view of their grim build and deploy process which entailed the CTO regular being up at 4am fixing deployment issues. Classic fire-fighting addiction, as it’s easy to be a hero. If sleep is not your thing. The lead dev strided around with undone huge boots, like a construction worker. Big fish in little pond - common delusion in tech.

This was first project I had been on where they had BDD tools, but that was it. Project ran to Scrum, even though they considered themselves Agile. When I suggested I raised issues on Jira tracking, not post-it notes, there was weird resistance.  Until the second day when a developer (the one who grumbled most) suddenly turned round to me and said, "Actually, this does make it easier!". Its not said with pride, as I wanted to respond "And I had to tell you that?".


## Industry: Logisitics (2015)

#### My optimism always wins ... in the end
_Tweet: Aug 22, 2015_
> My 4 #bdd years, out of 20 years of contracting, had more impact on my knowledge and learning, than any of the other 16. Says something.

#### Mock data, don't do it
_Tweet: Sep 14, 2015_
> It’s amazing how much quicker api development can happen, when there is ban of mock data for bdd tests :)  #necessityisthemotherofinvention

#### Yep, I am mildly pissed off.
_Tweet: Sep 28, 2015_
> People resist doing #bdd scenarios, while at same time, illustrating user stories verbally, using scenarios. Is it such a big leap? :)

#### Frustration showing, as I was spoilt with earlier BDD projects
_Tweet: Nov 15, 2015_
> When #BDD scenario writing is delegated (usually QA) & no-one else reviews, different expectations are no surprise. Needs consensus.
> 
Over the Netherlands on a large Agile Transformation project, bloated with Agile consultants but luckily very good developers. This is partly why this case study is longer by far. My thoughts on Agile Transformation projects contain too many swear words, and could fill an article all on it's own.  Dutch office culture is a little ... old fashioned. Maybe that's not the right description, but generally there is informal communication layer, but also a strong hierarchal based layer. And the two shall never mix.

The digital transfomation "work" was an incredibly annoying side to the work, the older senior management layer were clearly enthusiastic with concepts of change and improvments. The consultants clearly followed some kind of agile management guidebook.  One strange one would hang out at the back of random Scrum meeting, pereched like a statue on edge of a desk, like he was eavesdropping (trying to be the chicken).  He knew I didn't like him, as I considered him untrustworthy and self-serving.  I was left alone within the teams, as they worked out early on I was too cynical to be bothered with. 

The Agile test consutlant clearly regardless Specification by Example as his "bible" (always easier life if you just have one), as it was easier for them to grasp, and become quick "experts" in. Yes, it's all about the fucking conversation. And lego. And "fun" bughunts (yes lets all demoralise development by having surprise one too). There are some Agile consutlants I can respect, but as a group full of some real self-serving slime. This was the problem - the projects under the DT umbrella had very self-serving indiviuals, the nature of Agile consultancy. My own theory is an over-inflated sense of power, as senior management suddenly become like children eager for their new toys, and hopefully an army of doers ready to follow any fluffy ideas thrown at them. They are professional (Agile) chickens, dropping their never-ending soundbite eggs (wanted or not), doing silly dances, disrupting working, pointless games/presentations. It's all a game. It's an idiot profession.

it wasn't all  bad ...

Developers were from Xebia (mostly), and an excellent bunch they were to. Ultra professional, their code was fabulous and helpful to.  The developers were not actively involved in the writing of acceptance tests in the required Gherkin, but they were using a nice Jasmine/Protractor setup prior to that. This was my first proer use of CucumberJS/Protractor, and it was ... fiddly to get set up. As I don't believe in wasting time, and wanted to quickly guage developers, at the main weekly development meeting I asked for help as the framework as the code was not behaving asynchronously (i.e. it was not properly waiting for page loads). All developers tried and failed - some being very dismissive about the code then irritated at their own inability to resolve it. I have to say, I enjoyed those moments. Finally when working with a junior developer, I appraoched issue from another direction, as he said quite sensibly maybe CucumberJS is just not very good. In 2015, it still wasn't! Changing the test code to use other functions worked.

I was also lead on two other projects, which had low-skilled testers, many of whom automating tests was very new and they were reliant on developers to write the code. With some basic help, I at least got them started coded some basic steps, to which the developers sighed with relief. 

They were using a CucumberJS/Protractor setup, both these products still releatively new at that point. So the CucumberJS/Projector binding was awkward. On the two other projects the framework was broken.  One had green running tests, though there were in fact failures. Another had butchered the core code, so you couldn’t use “And” anymore. To this day, I still don’t know how he did it, and unfortunately my discovery led to his contract not being extended. Up to point of my arrival, they had been only writing Gherkin, and the developers wrote the code.

One another project they had hired antoher lady, a Protractor expert, which I wasn't, so I asked to pair sometime to share knowledge and hopefully pick up more Protractor info. A look of fear came on her face, and she hurriedly explained she had used it "a little". I wanted to facepalm. After a few tester meeting, I proposed we share my now working stable framework between projects (mine was only working one), and move forward.

After these initial dramas, the process was pedestrian.  I would take user stories in Jira, created by a old-fashioned PO, and devise Gherkin tests. Why was I using Gherkin, when I was the only one writing them? Simple. Because people liked them. You can spin any angle on Gherkin you like, but the use of tools boils down to audience. If it was just me and a bunch of developers, the setup would be leaner. One issue throughout the project is tests never ran on build or deploy pipeline. There were many manual steps in both, and horrendous amount of docker containers.  So running against environments from my machine, and making reports available on the Confluence wiki that noone looked at. Senior management would add stars on things, usually on Sunday night.

One class act a month before I left, was the PO suddenly took it upon himself (without consutling with the teams at all), and decided to use the aha SaaS, for recording requirements. IUtterly laugable that a manager thinks this kind of decision making, looks like strong action from stong manager (exactly why he did it). Development went well, because there were good developers. And a good Scrummaster. And a good test engineer of course :) But the digital transformation layer was utterly pointless.


## Industry: Vouchers (2016)

#### My escapism project
_Tweet: Jan 19, 2016_
> January mission: Create #BDD test framework that works on Mac, Linux and Windows, without need for "fiddling" :) The latter will be awkward!

#### Ooooh, miaow! Obviously read a few articles that pissed me off.
_Tweet: Jan 25, 2016_
> Your failure to persuade business as to the benefit of a well-organised specification language, does not mean bdd is crap. #Gherkin
> 
#### Depressing realisation of the idiocy of development process.
_Tweet: Feb 14, 2016_
> Why many clients appear to want the #bdd style test automation, but not much else ... apart from some kind of magic.


The interview was weird, as they talked like everything was in place and I was part of the plan. What I didn’t realise the plan was: there was no plan. They assumed I would slot in and somehow “do my thing”. 

I used a Cucumber/Protractor set BDD tools, but not BDD, and tests had to be run on my PC. The successful build dashboard was a screenshot green. Team contribution to writing features was zero, the young PO's preferred gazing at spreadsheets and their Inbox. I made it a mission to ensure test framework was portable across Windows, Linux and MacOS (success!). I was forced into using Windows platform, as I had to use machine from their office.  Windows 7 was getting towards better support for Node and support for Linux commands, but a headache of a challenge. 

In scrum meeting I regularly had to wave my hadn’t and say a sarcastic “hello!”, when people referred to me like I was not there. This was the testers they were used to, or no testers any all.  I would get messages from the lovely beleaguered QA manager, saying a dev was complaining I was raising bugs before he finished. I replied that is what I do when I am testing on test environment. No, I should wait until I am told. 

I spent most of four months building CucumberJS based test framework, and executing UI/API tests locally and emailing out reports. Some places are so broken, there is little you can do to fix without some serious ass-kicking. My work was popular with management, who like the fact there was something they could rely on. Though it was always reporting bad news. My daily pin-drop question was “when can I get these tests running as part of the build cycle?”. It was the kind of environment a shit tester could go hog-wild, and cruise through 6 months, just ensuring the bug tickets was closed off.

It was a lesson that sometimes although senior management hire to get help, it does not mean anyone underneath them wants it. It was a firefighting environment, that plain refused to listen to any . They preferred the way of working, even though the demands of their B2C website clearly pointed to change. The Products Owners were young, happy with their job titles, but seemed a little clueless what they were supposed to do. The beleaguered Scrummaster was forced to play silly games around signoffs, as the lead PO always took opportunity to puff out his chest and be difficult for the sake of it. Forget BDD, this place wasn’t even Agile, it was chaotic but mitigated by superb (wasted) devops. 

## Industry: NHS (2016)

#### BDD was a sensitive subject area around this time - too many vying for "expert" status.
_Tweet: Jul 18, 2016_
> I should add that I am not selling #bdd as software development cult. Thought I should add that, given recent testing soap operas!

#### I still believe this 
_Tweet: Jul 1, 2016_
> I don't care for labels, but projects with  certain labels seem to attract good people, at all levels. #bdd #opensource #devops

Worked again with consultancy, who generally followed the same BDD-driven approach, but really it’s about writing Gherkin style features.  A bit more of a pedestrian project, it started out as a Java/Spring project, but the frontend was given to angular. Heavily driven by UX team, via prototyping it worked not least because although the PO’s were not up to doing requirements, gherkin or otherwise, they trusted the team and clearly enjoyed being part of it.

## Industry: Ministry of Justice (2016/2017)

#### One of those tweets referencing something specific that must have pissed me off
_Tweet: Dec 5, 2016_
> An automated acceptance test doesn't care what you label it - #bdd, #tdd, #atdd  ... It's either useful or it isn't.

#### I always positive spin, so this was result of applying some pragmaticsm in more challenging projects
_Tweet: Jan 5, 2017_
> #BDD doesn't have to be pure for good effect. Better specs, better CI tests, better team vibe and better tools.

The most suited and booted consultany I had worked with for a while, but open and honest with their challenges. In those circumstances, I will always give a little bit more.

The BDD tools use, not strict BDD, but was tests first, and these were used by business as acceptance criteria.  Used the now classic combination  of CucumberJS/Protractor.

Team contribution to writing features: Poor (Test).

The BDD tools use, not strict BDD, but was tests first, and these were used by business as acceptance criteria.

Team contribution to writing features: Average (Test, Bus Analyst).  Another civil service, and they seem to expect Gherkin format, as the OPG project was touted as a success based on the approach. No PO as such, a couple of business analysts, though one kept far removed of requirements while the other had a committed attempt at the Gherkin.  I do curse it sometimes, as with business analyst I was want them to basically be themlsves, but they too get lost in common traps which are over or under doing them.

Civil Service like BDD projects, or they are commonly sold of the Gherkin format itself. This leads to varying degrees of collaboration. You can’t fire someone for their inability yo write requirements properly. Your standard Business Analayst will still do a masterful job of giving you all you need to develop tests based on the scenarios they usually outline. But  bizarrely most find translation to wiring in actual Gherkin hard. Not least because the beginner guides are all “When I click button, Then I see confirmation message.”  This quickly falls apart when considering less form-driven tests (the easy ones). This pushes PO’s to think more carefully about their usual write-3-line-user-story-and-run approach.

## Industry: Civil Service (2017/2018)

#### Oooh, look at what I made!
_Tweet: Jun 11, 2018_
> When I did a presentation of Gherkin and BDD for a totally non-tech audience (mainly for the product owners), I realised it's straightforward to avoid terminology, and use simple generic language. There is a tendency to over-complicate things in tech 

#### Uusal resignation to fact, if you don't have the PO that do speicifation by example, you can still use the appraoch and the tools, though no need for Gherkin if no interest (sometime devs like to have this format)
_Tweet: Sep 8, 2017_
> The level of engagement from POs and stakeholders does vary wildly, but I still find BDD approach to acceptance tests useful.

Here I went for a CucumberJS/Webdriverio, which at the time was touted incorrectly as "selenium replacement" (it still needed selenium server to execute tests in browser). It came with whole host of steps, which quickly became apparent most were redundant/useless for the project. Midway through I migrated across to NightwatchJS/Cucumber framework, which only took and day or so.  The Gherkin remained the same, and it did not take too long to adjust the existing javascript code. I ended up with a much leaner framework. The issue with using the helper tools is it's not easy to see the overhead, until you have something to compare it to.


## Industry: Civil Service (2019)

#### I could imagine myself yawning as I typed this.
_Tweet: Aug 15, 2019_
> If you follow any methodology by the letter, you will have a hard time. Adapt, adjust etc. per project/team. BDD has good elements, which other approaches like Specification By Example picked up on. Also inspired some great opensource tools. More than readability 

A diversion skill-wise into Ruby.  As by now, learning as I go became just an assumed part of my work life.  As your skills accrue, learning is rarely from the beginning, as skills always cross into other products/areas. The project was driven by extensive designs and protyping, this does make following BDD path easier, so much can be visible (and operational depending on sophiscation for tool used). Civil service projects tend to be a tad pedestrians as design templates are tightly controlled and applied rigidly. It's like a brand-look. As soon as I see one of "those buttons", I know it's a civil service site.

And now I have lost interest in writing about it, as though projects are different, they are also the same. Life is 99% mundanity, 1% insanity and that goes for work too.


# Conclusion

The conclusion is there is no conclusion! It's clear what BDD is, but there are other positive effects I have seen on projects that I have worked on, when at least applying these principles is it has an effect that no consultant will be able to manufacture.

* It brings a team working closer together
* It attracts a certain kind of developer, a more sociable one.
* The business is drawn deeper into the requirements.

But don't let anyone tell you that it's too hard, and this is where the tester can really be of value - they can help make it happen. Test automation is not tied to any approach really, and I used tools of various kinds for testing since 1997. Test automation stands alone and can be done badly, and done well. Like everything in life. 
