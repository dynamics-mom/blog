It’s quite difficult to write a blog with 2 y.o., but more difficult is to do this when you are sick yourself.  After weeks of getting better, I finally find the time to write some words about Business Central. When I have started my blog, all people tell me I must create new article on regular basis. It is difficult I can agree… after the work you only dream about the bad and some sleep instead of sitting next to the table and write. After weeks of sickness, I have finally put myself together and create some manual about Intercompany. Hope you will like it!
At first create the IC company in the system. You can create one from the beginning or use the one of the existing companies as a template. 
Go to Companies -> New or Copy

![image](https://user-images.githubusercontent.com/118689671/220185735-7778e502-ab24-4f6f-906b-513b36c7c304.png)

It can take a while…

![image](https://user-images.githubusercontent.com/118689671/220185775-079a2f88-0250-4944-8a10-7845ae37512c.png)

Then do the Mapping between the Chart of Accounts. We must remember that sales transactions in one company will the purchase for another. That mean on one side there will be a revenue and on the other side it will be a cost. Go to Intercompany Chart of Accounts

![image](https://user-images.githubusercontent.com/118689671/220185803-dc8d1d34-45cd-4774-823d-f277961d8109.png)

There is possibility to use the existing CoA by Home -> Copy from Chart of Account. 

![image](https://user-images.githubusercontent.com/118689671/220185826-09bec8b1-118e-4084-b948-5ce4716d1161.png)

Then do the mapping in the Map-to G/L Acc. No.

![image](https://user-images.githubusercontent.com/118689671/220185850-a72a5db2-f584-488d-915e-304ba615b546.png)

If some of the accounts should be populated as the same, you can use the function Home -> Map to Acc. With Same No. (it can be done for multiple account by Select more function on the line). 

![image](https://user-images.githubusercontent.com/118689671/220185879-c1883957-a19c-40ab-9ea2-fbdacd181757.png)

If any of the accounts shouldn’t be used it can be Blocked.

![image](https://user-images.githubusercontent.com/118689671/220185903-131cef68-95be-44a6-a814-b5a75b5c6518.png)

The setup can be also Import/Export between the IC companies.

![image](https://user-images.githubusercontent.com/118689671/220185944-672a400c-6fc2-4e2d-9691-cad3099c5d52.png)

Then do the mapping between the dimensions. Go to Tell me -> Intercompany Dimensions

![image](https://user-images.githubusercontent.com/118689671/220185978-8785f1ce-ec4c-4e04-8fa2-146daf7fd279.png)

Similarly, to CoA the Dimensions can be copy from company setup. Go to Dimension -> Copy from Dimensions. 

![image](https://user-images.githubusercontent.com/118689671/220186020-9450ff7c-c73b-4ab9-95bb-52a004c7f667.png)

Then do the mapping manually or map the same. To copy the mapping go to Dimensions -> Map to Dim. with Same Code. 

![image](https://user-images.githubusercontent.com/118689671/220186051-03ff062f-4572-4227-83f7-45aec2e40748.png)

The Dimension Values was copied as well so you must adjust them if necessary.

![image](https://user-images.githubusercontent.com/118689671/220186085-a6385103-98c6-41c7-9ed7-2bb0824bacda.png)

Note: Intercompany Purchase Transactions are not handled Resources, Fixed Assets, Item Charges. If you have one of this type it will be send blank, so the user needs to adjust it later. 

Then create the Intercompany Vendor and Customer. 

![image](https://user-images.githubusercontent.com/118689671/220186116-b1ddbab3-5f67-4d43-a572-a6d20be66717.png)

![image](https://user-images.githubusercontent.com/118689671/220186130-18f7a472-1729-4fd8-8f92-97f52331ca3a.png)

In the newest version of Business Central you must run the feature from the Management Feature -> Feature Update: Automatically accept intercompany general journal transactions. In the release 2022 wave 1 the Microsoft have added new function related the Auto-accept the transactions. 

![image](https://user-images.githubusercontent.com/118689671/220186182-08d5038c-c41f-4d3a-bb59-19867f1e7ba3.png)

Go to Intercompany Setup

![image](https://user-images.githubusercontent.com/118689671/220186234-4a0e8090-c5bf-49e3-850a-50876b8534fe.png)

Fill the Intercompany Partner Code for the current company and decide if the transactions should be sent automatically. Then go to Open new Intercompany Setup page

![image](https://user-images.githubusercontent.com/118689671/220186284-68ce5729-143f-4ec9-90fd-5d16b28f89d7.png)

Setup the Default IC Gen. Jnl. Template and Default IC Gen. Jnl. Batch. New feature I have mentioned above – Auto. Send Transactions. 

![image](https://user-images.githubusercontent.com/118689671/220186332-8e12aa79-38df-4bc2-bb9c-ca7826f899f3.png)

Go to Intercompany Partner and add the Code:

![image](https://user-images.githubusercontent.com/118689671/220186376-5cc9e3e4-199c-43c1-82a5-83cb05813600.png)

Fill the Sales Transaction Tab:
Customer No. – select the one from the list
Receivables Accounts – select the account from CoA for posting the IC Receivables
Outbound Sales Item No. Type - what type of item number is entered in the IC Partner Reference field for items on purchase lines that you send to this IC partner (Order, Common Item Number, Item Reference)
Fill the Purchase Transaction Tab:
Vendor No. – select the Vendor from the list
Payables Account - select the account from CoA for posting the IC Payables
Outbound Purch. Item No. Type – what type of item number is entered in the IC Partner Reference field for items on purchase lines that you send to this IC partner (Order, Common Item Number, Item Reference)
Cost Distribution in LCY – if you will be splitting the costs between the companies, decide if the value will be sent in LCY or the origin currency

![image](https://user-images.githubusercontent.com/118689671/220186426-4e92af7a-7c71-4c70-ae13-b51ffce433ba.png)

Do the same setup on the second company – IC
* use the same code as main company

Documents Handling
Create Sales Order for IC Customer 

![image](https://user-images.githubusercontent.com/118689671/220186530-c544be70-eb42-4789-8d1f-3c1540f9b770.png)

Press Send IC Sales Order  

![image](https://user-images.githubusercontent.com/118689671/220186561-1bb7a1d4-0a75-4710-ba9c-f415daef221c.png)

In Handled Intercompany Outbox Transactions, you can see the Order was transfer. If you do not approve auto creation of the document, you will need to open Intercompany Outbox Transaction and send it manually

![image](https://user-images.githubusercontent.com/118689671/220186617-bafd4fbd-aa99-427a-b9b5-da51b374cca7.png)

In Handled Intercompany Inbox Transactions, you can see the Order was received. If the auto-approve was not switched on you will have to go to Intercompany Inbox Transactions and approve it manually, reject the document, send back to IC Partner, or leave it as it is in Inbox.

![image](https://user-images.githubusercontent.com/118689671/220186654-4d427321-40e2-498d-83e9-89be565a5398.png)

We have used the option to auto approve so the system creates the Purchase Order automatically

![image](https://user-images.githubusercontent.com/118689671/220186691-5beec8bf-6e44-499d-8aa5-54c5a72be697.png)

Create Sales Invoice for IC Customer, then Post

![image](https://user-images.githubusercontent.com/118689671/220186730-24b2eefb-85e7-4203-9f4d-7fc966a9d416.png)

In Handled Intercompany Outbox Transactions, you can see the Invoice was transfer

![image](https://user-images.githubusercontent.com/118689671/220186755-c4451998-ca33-4cb4-bbb9-b195f78c84ca.png)

In Handled Intercompany Inbox Transactions, you can see the Invoice was received. Incoming intercompany transactions can be automatically accepted only if task scheduler is enabled.

![image](https://user-images.githubusercontent.com/118689671/220186786-99e067a1-1638-4b3b-8d95-7cfa123b5f26.png)

We have used the option to auto approve so the system creates the Purchase Order automatically. That is nice because “older” users remember the system created before just a journal. Now we have an invoice card 😊

![image](https://user-images.githubusercontent.com/118689671/220186822-e5f91f13-2a28-4e39-b1d5-7d1f2032f84a.png)

IC Allocation costs – in the Intercompany General Journal you can create the posting of Purchase invoice. Then in next lines you can add the information how much from the main cost should be retransfer to your IC Partner. When the journal is posted the cost are deducted from the cost G/L Account and send to the daughter/mother company. 

![image](https://user-images.githubusercontent.com/118689671/220186860-c1ce8bf3-3c4e-4d46-974e-f7edfdd134ec.png)

You can transfer the below documents:
General Journal entries
Purchase and sales orders
Sales invoices
Credit memos
Return orders
You can print the report with all Intercompany transactions per period. Search in Tell me – Intercompany Transactions Report. 

![image](https://user-images.githubusercontent.com/118689671/220186903-025adffb-e0f0-42b3-8784-4d56fec9c917.png)

