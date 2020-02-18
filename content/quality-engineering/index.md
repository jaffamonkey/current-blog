---
title: Quality Engineering
date: 2018-02-13T13:42:49-05:00
images:
    - /clients/clients.png
---

Quality engineering combines quality assurance and test engineering

## Test engineering

> Less is more

Sometimes investing is a feature-rich test framework is a good idea, but starting small is always the best place to start. Tests run as part of CI/CD should be as lean (fast) as possible. Conversely, don't waste too much time on native coding - packages are there too help you, just be selective and conscious of potential overheads created on the Build server. 
Scope of automation

Did you really think it's just about verifying feature for you web or mobile app? That is just the window on the testing input from business viewpoint, but the scope is more dynamic than this. Or should be. 

I do often repeat the same mantras: exploratory testing is a mindset that can be applied to automation, you don't need to run a heavy load test to get useful feedback, web accessibility should be covered by default (any excuses are poor excuses), security testing is an essential not an option, device/browser compatibility testing should be approached with scope caution.

Importantly, all tests of all kinds should evolve constantly, or they are most likely useless.

> DevOps is our friend

Test engineering can help beleaguered DevOps in several ways: Dockerizing your test framework (better portability), keep package-count low (and specify versions so pointless updates do not occur on every install), use cloud service to store reports and other test artifacts (like screenshots)

## Quality assurance

What an Agile coach/consultant does, was always covered in Quality assurance remit (without the Lego, and bug-hunt fun days).

Major challenge when talking about quality in software, without sending the audience into deep coma. As with describing your dreams to others, it never seems quite as exciting when put into words. 

So why do we need Quality assurance? Because we are all the same in one respect: even when we are sure, we can be 100% wrong. 

I focus on interactions (the weakness in humans is the same as code - at points of integration). But keeping on top of this, we can ensure quality in all areas of a project and here are a few ways Quality assurance can help. 

### Transparency

We have all heard this before, but these will never happen unless people can feel free to be themselves. Keep momentum on a project, with a group of individuals with complete freedom to express themselves. It's a challenge, and a worthwhile one.

### CI/CD pipelines

Vital, but should be serving all needs and it is easy to fall into the trap of just celebrating they exist.

### Definition of Done

Everyone has a common idea of what sensibly indicates when a Feature is "Done". However, everyone has also subtle variations on what they consider to be "Done". Is it worth dissecting the DoD to a granular level to please everyone? No - keep it pragmatic.

### Requirements

In order to do effective criteria such as the DoD, the user story has to be clear, and it is worth chasing this process down. What helps is thinking beyond a 3-liner user story, and thinking about examples to illustrate meaning more clearly. This gives the developers more direction, a better basis for creating acceptance tests, and a clearer shot of fulfilling expectations.

*Quality at all stages in project pipeline needs regular reivew, and importantly, the team should feel they can be honest.*
