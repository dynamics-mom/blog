---
layout: post
title:  "First story & how to create development tasks"
date:   2022-12-02 21:30:00 +0100
categories: general
---

That will be a story why I have decided to start a blog. The second part of the story gives the conclusion on why a proper development task description provided by the consultant matters. I have collected the tips and suggestions from my developer’s friends to help other write proper documentation. 
It was a lovely evening until the little one (my son, Franek) woke up with 38 degrees. It was 10 PM, so I knew that finding a nanny for the next day will be impossible! 2 hours earlier I finished the general concepts of the development task for the training for junior developers the next day. I did it as general as possible because I knew I will be at the meeting with them to answer the questions. We made a deal with a daddy that he will cover the first part of the day so I will attend to the workshop. Then I will be back and cover the second part of the day. On my way to the office, I was talking to a friend who was running the training (that’s coincidence that he is my neighbor). The first thing when I came to the office, I informed my colleagues that I need to run to home in the middle of the day. In this kind of situations, I always feel so unprofessional knowing that I should be in the office, but I simply can’t… but then I realized people understand this. I’m not the only one whose kid is sick on an important day (or the first day of holidays :)). 

Dear ladies - don’t worry, these situations happen all the time. Just do the rest of your job the best you can, and people will fully support you. I think the pandemic period changed minds of a lot of people. 

Recently, I had a situation that my sick child didn’t want to go for a nap with nanny. I took him on my hands and started swinging but I was on the familiarization meeting with another team. Suddenly my manager said that now Magda will introduce herself, but please switch the camera on. First thing that came to my mind – “oh no”. I did it as he said, but in the beginning, I said that I’m a mother and then I started talking about myself. Nobody reacted, everyone was super chilled about the whole situation. It doesn’t mean that now I will go with Franek for all my meetings, but I want to say that such stories happen, and we shouldn’t cry about it. 

Let’s go back to story. During our way to the office, we have discussed that I would like to do something more to create my own consultant brand. The friend of my suggested the blog, so my first answer was… yeah with Franek I can write about mother’s live mostly. That’s how the Dynamics Mom was created. As a kid I wanted to be a journalist (the sports one, but let’s do some compromises). In the middle of the day, I took taxi back home and, on that way, I have written my first post! Action = reaction! 

What about the workshop and development task description? Why this topic is so important? Nowadays we mostly work from home, cooperating with people across the word, different time zones, different mother language. The time when we were at the office every day and we could discuss face to face all programming changes have passed. The proper description of task was important as well to keep the history of the features. Now we must write it properly because sometimes we are not online all the time. We walk our dog during the day, make doctor appointments, dentists, some of us like to start work at 12 AM. and some at 7 AM. (crazy ones). 

The consultant job (sometimes even considered a business analyst) is to take all the requirements from the client and put it as a story to the developers. Once during the interview, the headhunter asked me what the consultant work is. I like to say that we are kind of translators, we talk with the clients using financial and functional language and translate it into developer’s language to create the features. As I mentioned already, we can’t always join the call, ask additional questions, and wait for the answers - so to do not stop the and try to describe the requirement as good as in possible from the beginning (even if it means redoing some of the work you already did or spending another hour on analysis).

A couple of tips:
1.	The most important one in my opinion – write anything. Better or worse but try to write down all the requirements you know. I’ve asked my fiancée (BC developer & architect) what a good specification in his opinion is. The first answer was - any documentation, since very often they do need to work on guesses or unfinished documents from the customer. Let’s make our job simpler 😊
2.	Try to understand the client’s requirement by yourself. I’ve done the postgraduate studies of IT Project Management and one of the courses was about facilitating the meeting. The lector repeated over and over our sentences but starting with “did I understand it correctly “, ‘did you mean that…”, etc. At the beginning I was quite frustrated, but then I tried this method with client. That’s worked like a charm! If I correctly understand the needs of my customer, I can better explain it to others. The consultant cannot be afraid to go back to the client and ask more and more. We work for them to make their lives easier. I’m not talking about sending the same questions several times because it puts as in a bad situation. I am talking about clarifying the questions which helps build the better features. 
3.	Trye to put in the exact numbers of the tables and pages or at least their names, where or which the functionality that should be created is based on. I do it like: “To the Sales Header Table (36) add new flied type = Boolean”. All should know Ctrl+Alt+F1 so you know when you write down the requirement. It costs consultant 1 minute more but helps to understand what needs to be done.

<img alt="Picture1" src="https://user-images.githubusercontent.com/118689671/205382859-a9ad168e-d04f-483e-95a7-f69cd661d82d.png">

4.	As I mentioned in previous point, write down the type of the new field if this is Boolean, Decimal, Text. If this is the list put the information to which dictionary table, it should refer to. If there is a possibility you can draw a picture how it’ll look like (see example below).

<img width="482" alt="Picture2" src="https://user-images.githubusercontent.com/118689671/205383381-161aa3a1-4203-4b89-a31f-dce2f2e6ffab.png">

5.	For all the new fields, try to put the relation to the other tables, e.g., “the new field should be copied to the field to Posted Sales Header (112)”. Remember if that the field doesn’t exist on the second table, add it there as well. See the screens below, if I add something on the Sales Header, I should add it into Sales Invoice Header as well. Of course, not all new fields need to be copied, but always think of it.

<img width="482" alt="Picture3" src="https://user-images.githubusercontent.com/118689671/205383440-41b45bee-42ae-4f3f-aead-b08af1f80f10.png">

<img width="482" alt="Picture4" src="https://user-images.githubusercontent.com/118689671/205383469-8bca3775-5bb3-490d-8019-10540e8ae830.png">

6.	If it will be a new table/field, always put the name in English. It doesn’t matter which language the project is in. All the names need to be created in English. Then in cooperation with developers, the consultant should fill the translation file in. If it’s possible, ask your client for the translation.

<img width="482" alt="Picture5" src="https://user-images.githubusercontent.com/118689671/205383763-5e491a35-e465-4a26-8576-9c150a77ce32.png">

7.	If there will be any calculations, explain exactly what to add, multiply, divide, etc. The best way is to provide all the names of fields that must be used, e.g., Quantity * Unit Price Excl. VAT * 10% and fill the results into new field called Transport Cost.
8.	Think about all possible scenarios. Let’s say we need to update some data by filling the field A. What should be done with the field B? Should it be changed? Should it stay the same? If it needs to be changed, so under which conditions. Trust me, developers ask all these questions while programming. 
9.	If you ask for the report correction, because it’s too complex to do it yourself in Word (yes, some reports consultants can correct by themselves), mark exactly which fields should be placed where. Explain what caption should be used and what data should be visible on the printout.

<img width="414" alt="Picture6" src="https://user-images.githubusercontent.com/118689671/205383830-6920abf3-71e3-4a20-a944-107aecb1ee86.png">

<img width="482" alt="Picture7" src="https://user-images.githubusercontent.com/118689671/205383857-fa20f612-cdec-4c90-870d-0434c1817082.png">

10.	Don’t hardcode anything. If you need to filter by any name, code, value ask to add it to the setup instead of putting the exact value in the code. 
11.	If this is possible put the pictures (no, not of yourself) 😊

In the beginning of my consultant’s career, I have sent the description of the development task to be developed. My friend did it exactly as I explained as a joke – it was completely not what I expected (even though I knew what the task was about). It was a lesson to always think twice. Communication is important. Let’s make our work simpler for the sake of all of us! 
