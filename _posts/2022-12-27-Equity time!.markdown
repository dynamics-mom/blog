---
layout: post
title:  "Equity time! "
date:   2022-12-27 16:30:00 +0100
categories: general
---

Let’s write some words about equity. It’s time to talk about new features in Financial Reporting (calculating the equity) and comparison of man and women at work. I’m proud of being a mom. I think it’s the best what happened in my life. When I wake up in the morning and see the smile of my kid my heart just melts. When I came back from maternity leave, I felt like I lost a year in my career, but it wasn’t like that. When you become a mother, you start the most important project in your live. That’s probably the only one which will never reach GoLive, but you will love it the most. I was off for a year and a half so it’s quite a lot. First thing I’ve done when I came back to work, was passing MB-800 certificate. Then I took over the project form the other Senior Consultant. I was full of positive energy to work, and I shared it with the others. Basically, I share the knowledge which I like the most. I would like to say that hiring young moms don’t stop the work because the baby is sick often. They are usually full of energy and head of dreams. Employers shouldn’t look who is better man or women, but sometimes we lose because people think that moms always take sick leave. 

We girls work, take care of babies, cook, do the laundry, look pretty (that also a hard job to do). Do you ever hear the story about the sick mom? Even if, when the woman is sick, they do the list above like every day. When the man is sick, he barely can move his hand with 37 degrees (after this comment I won’t be the most liked blogger by men). That’s not the story of my life. That’s the story of almost all my girlfriends. Maybe that’s why the women are giving the birth and taking the months off. We are stronger to fight with the work inequity, like me! 

What about equity in Business Central. There is a standard functionality to build the Financial Reports (replaced the Account Schedules) based on correct setup on Chart of Account. In the version Business Central 21 there are new features into it:

1.	You can import / export Financial Reports into files so you can simply manage them between companies.  

![image](https://user-images.githubusercontent.com/118689671/209688351-dcbd8482-016a-4cc5-b62d-d9d84e3eb195.png)

2.	User can do Totaling by Totaling Type = Account Category 

![image](https://user-images.githubusercontent.com/118689671/209688410-e7d73023-37ec-4406-8f90-9b77b138c6d0.png)

3.	You can decide if the lines should be printed if the balance = 0. 

![image](https://user-images.githubusercontent.com/118689671/209688470-fbae9d37-77aa-4339-aa52-834935216f0b.png)

4.	You can view Account Schedules Overview as 15 columns so that you can see budgets for 12 months and a total.

If you need to remember how to generate the Financial Reports in Business Central, please see the reminder below 😊
Create the P&L and Balance Sheet template:

![image](https://user-images.githubusercontent.com/118689671/209688613-b694c661-596e-4220-9386-b5a85a3db5ab.png)

![image](https://user-images.githubusercontent.com/118689671/209688633-22fd741d-f8a5-4fd3-abcf-73a7ce33bc82.png)

Please be advised the Account Categories cannot be added but the default names can be change by clicking Edit

![image](https://user-images.githubusercontent.com/118689671/209688677-d9a4bd9d-0278-4b69-88ad-6dd314dc3443.png)

Fill the Description under each Category based on the P&L and BS template. The Subcategories can be added/deleted, or the user can adjust the existing ones. User can create the indentation line in the report. 

![image](https://user-images.githubusercontent.com/118689671/209688734-d6ade901-1536-4c3d-b3d4-a7d337090b59.png)

Please remember that all subcategories must be assigned to the proper Account Category, such as Assets, Liabilities, Equity, Income, Cost of Goods Sold, Expense. 

![image](https://user-images.githubusercontent.com/118689671/209688774-c8e5494a-7449-45cb-b5ac-7faaf721c97d.png)

For the cash flow statement proposes user can add the Additional Report Definition e.g., Operating Activities, Investing Activities, Financial Activities, Cash Accounts, Retained Earnings, Distribution to Shareholders. 

![image](https://user-images.githubusercontent.com/118689671/209688825-1255afad-ed5d-47f0-8c73-2f91a07215e8.png)

The standard setup already covers the existing Account Schedules. At the end of the G/L Account Categories setup, please adjust it. 

![image](https://user-images.githubusercontent.com/118689671/209688864-f7574e22-34df-45d0-8152-f42e8b784440.png)

Then the user needs to decide if the reports should be created as a new one or adjust the existing one. 

![image](https://user-images.githubusercontent.com/118689671/209688892-117f8bc2-b8a3-4e42-9ffd-bad5772212dd.png)

Then to each G/L Account with Direct Posting Type the one of the created Account Subcategories needs to be added. 

![image](https://user-images.githubusercontent.com/118689671/209688921-f419eb07-8ed3-44aa-9f30-1ab4e08bb970.png)

The Account Subcategory can be updated by Configuration Package. The User can export the table G/L Account (15) and G/L Account Category (570) to the Excel Sheet, then fill it in and import back. 

![image](https://user-images.githubusercontent.com/118689671/209688966-6ea45437-14b4-467c-9de8-4156ead5575a.png)

![image](https://user-images.githubusercontent.com/118689671/209688983-cbc8ef2c-6100-4cd7-a829-257c937e67f9.png)

Update the Accounting Schedules again. 

![image](https://user-images.githubusercontent.com/118689671/209689015-e83fe1be-6839-44c3-9564-677b88d0cf88.png)

At the G/L Accounts Categories the accounts were updated. 

![image](https://user-images.githubusercontent.com/118689671/209689044-12fcf68f-1aec-41c5-90d4-69163ebf6937.png)

Check if the Finance Reports are properly assigned in the General Ledger Setup 

![image](https://user-images.githubusercontent.com/118689671/209689089-8a459e00-841f-4e17-9f55-64ba4629518c.png)

Print the report in the Financial Report Page. 

![image](https://user-images.githubusercontent.com/118689671/209689113-4d0e1b66-cb1c-4e0b-95c0-8b37aa18ea43.png)

Done. 
