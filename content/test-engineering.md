---
title: Test Engineering
date: 2018-02-13T13:42:49-05:00
---

> Less is more

Sometimes investing is a feature-rich test framework is a good idea, but starting small is always the best place to start. Tests run as part of CI/CD should be as lean (fast) as possible. Conversely, don't waste too much time on native coding - packages are there too help you, just be selective and conscious of potential overheads created on the Build server. 
Scope of automation

Did you really think it's just about verifying feature for you web or mobile app? That is just the window on the testing input from business viewpoint, but the scope is more dynamic than this. Or should be. 

I do often repeat the same mantras: exploratory testing is a mindset that can be applied to automation, you don't need to run a heavy load test to get useful feedback, web accessibility should be covered by default (any excuses are poor excuses), security testing is an essential not an option, device/browser compatibility testing should be approached with scope caution.

Importantly, all tests of all kinds should evolve constantly, or they are most likely useless.

> DevOps is our friend

Test engineering can help beleaguered DevOps in several ways: Dockerizing your test framework (better portability), keep package-count low (and specify versions so pointless updates do not occur on every install), use cloud service to store reports and other test artifacts (like screenshots)