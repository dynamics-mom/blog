---
layout: post
title:  "Let's change a mood for a moment..."
date:   2022-12-27 16:00:00 +0100
categories: general
---

Let’s change the mood for a moment. My first blog posts might have been sad. I have talked about sickness, equity etc. However, life of a mother isn’t only about the problems! I can’t write like that all the time because other consultants won’t decide to have a kid. The idea of the blog was born while I had motherhood issues, but it isn’t always like that. Don’t worry!

Franek, my son is incredibly positive kid, happy all the time. When I ask him about something he always replies ‘YES’ (probably he doesn’t know how to pronounce ‘no’ yet, but it’s better for us 😊). I try to finish my work at the same time every day, we pick him up from school and spend the whole evening together. I love to watch him doing puzzles. Like all mothers, I believe my son is the smartest kid (why he wouldn’t be with the parents like us). I think that’s normal that we want to be proud of our babies and we should be, whatever they do. First steps, first words, first argue, etc. All those moments are worth to remember. As a working mother sometimes, I am afraid of skipping something when he is at pre-school, but honestly, he needs this time without parents to learn how to be independent. Women needs this time for themselves as well. They need to grow as an employee, doing something with other adults, making they own career. Kids are growing so fast and one day they will start do their own stuff. I can work during the week, but weekends are always for my son. He should see mother take care of him and love him the most, even if she sent him to pre-school in such young age (my kid was 11 months). If you find this work-life balance and will accept it – sky is the limit for you.

If we talk about changes, in Feature Management you can already see the change Customer / Vendor Posting Group functionality – Allow using of multiple posting groups for customer and vendor.

![image](https://user-images.githubusercontent.com/118689671/209685661-6514cecb-f71b-456a-9b93-ab8e9ffedec9.png)

There are some features that you need to enable before:
- Enable use of new extensible exchange rate adjustment, including posting review
Then when you try to post the Purchase Order, Purchase Invoice, Sales Order, Sales Invoice you will be able to change the default Posting Group into the substitutions. Note: there is no info that the functionality will work on journals. 
In the documentation from Microsoft, it is written that when the posting of the payment for the document will be done, the amounts will be re-posted between accounts to match the posting. 
Looks quite promising because lot of clients ask for this functionality. Unfortunately, we must be patient and wait till Q2023 for PROD. There will be test version on Sandbox in BC22. I will update you!
