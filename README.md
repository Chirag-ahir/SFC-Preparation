# SFC-Preparation

What is sales?<br>
Sell your product to prospects is known as sales.

What is sales process?<br>
A sales process maps out the stages an opportunity follows through its sales cycle, affecting what’s available to view in a sales path. Within a specific sales process, you can easily add and remove stages.

What is salesforce?<br>
Salesforce is a cloud-based CRM platform that helps business to manage their sales, marketing and customer service activities. 

What is case?<br>
A case is a customizable record in Salesforce that tracks and describes a customer issue, complaint, request.

What is object?<br>
Object in salesforc represents a entity which stores particular type of information in our database. 

[Table in DB represent as a object for SFC]
[Column in table represent as a field for SFC]
[Row is table represnt as a record for SFC]

What is a standard object?<br>
Standard objects are objects that are included with Salesforce. Common business objects like Account, Contact, Lead, and Opportunity are all standard objects.

What is a custom object?<br>
Custom objects are objects that you create to store information that’s specific to your company or industry. For DreamHouse, D’Angelo wants to build a custom Property object that stores information about the homes his company is selling.

What is list view in SFC?
A list view is a filtered list of records where you can view records for one object at a time. For example, a list of Contacts, Accounts, or Opportunities.

Modify list view of object: https://youtu.be/PjiSTxBWcrk?si=UWXs9AOtFnbGTDSV&t=850

What is Schema Builder?
Schema Builder is a tool that lets you visualise and edit your data model. It’s useful for designing and understanding complex data models like the company’s employees and all sales (Setup > Schema Builder)

What are two ways to import data into SFC?<br>
Data import wizard (Setup > Data import wizard - Supports <= 50000 Records)<br>
Data loader (Client application - supports 5M+ data)

What are two ways to export data into SFC?<br>
Data export wizard (You can export data once in a week)<br>
Data loader (As many as you want but not works in professional edition)

What is validation rules?<br>
Validation rule used to validate data when entering data into salesforce.

What is detail page?<br>
When you open any student record in salesforce what you see is detail page. You can find field like name, phone no, DOB on detail page.

What is edit page?<br>
When you click on edit record button, the page you see on pop-up window is edit page.

What is user license in SFC?<br>
User license defines which type of functionality user can access in salesforce.

What is junction object?<br>
Any object which is got two master-detail relationship field on it is called as a junction object.

What is page layout?<br>
Page layouts control the layout and organization of buttons, fields, s-controls, Visualforce, custom links, and related lists on object record pages. It controls details page and edit page. 

Modify page layout: https://youtu.be/gHHXE3FcxJM?si=J-hAfYB5odXILk5U&t=277  

Assign different page layout to different users based on role: https://youtu.be/gHHXE3FcxJM?si=U_iHVtgLk06UdfRr&t=820 

What is compact layout?<br>
Compact layouts control which fields your users see in the highlights panel at the top of a record. 

customize compact layout: https://trailhead.salesforce.com/content/learn/modules/salesforce1_mobile_app/salesforce1_mobile_app_compact_layouts

What is Profile?<br>
Profile is collection of settings and permission which define what user will be able to see and what user will be able to do. Two types of profile in salesforce: Standard Profile and Custom Profile.

What is Permission sets?<br>
Permission sets are collection of setting and permissions which give a user additional access from the access that they have already got from their profile.

Can user restrict the access of user that he got from profile using permission sets?<br>
No user can restrict the acess of user that he has got from profile using permission set. permission set used for give additional acess to user.

One user only assign to one profile, <br>
But one user can be assigned to multiple permission sets.

Is it possible to delete a user from SFC completely?<br>
You can not delete a user completely at all from SFC, It's not allowed to delete a user from SFC in any org. But you can revoke the access of user by making that user inactive (Setup > Users > User > Uncheck active box)

What is difference between Deactivate user and Freeze user?<br>
When you deactivate user the license associated with that user can be assigned to someone else but if you freeze user the license associated to that user will remain with him. 

What are different levels of Data level security?<br>
1. Organization level security<br>
    - User management (Setup > Users > Particular user > Active checkbox)<br>
    - Password policies (2 level)<br>
        - Organization level (Setup > Password policies)<br>
        - Profile level (Setup > Profiles > Particular profile > Password policies > Edit)<br>
    - Restricting access by location/IP (2 level) <br>
        - Organization level (Setup > Network Access > New) Applies to all users<br>
        - Profile level (Setup > Profiles > Particular profile > Network Access)<br>
    - Restricting access by time (Applies to profiles only: Setup > Profiles > Particular Profile > Login Hours)<br>
2. Object level security (CRUD) (2 level)
    - Profile level (Setup > Profiles > ParticularProfile > Custom Object Permission)<br>
    - Permission sets (Setup > PermissionSet > ParticularProfile > Object Settings)<br>
3. Field level security (read Only and Visible)<br>
    - Profile level (Setup > Profile > Particular profile > Field level security)<br>
    - Permission sets (Setup > Profile > Particular permission set > Object setting)<br>
    - Page layout (Required & Read Only)<br>
    - “Field Accessibility” is a one place to set security for all profile at once<br>
4. Record level security: Three permission: (Public read/write + Public read only + Private)<br>
    - Four level<br>
    - Organization wide default (Baseline level of access)<br>
    - Role hierarchy (E.g., Manager will have access to all VP)<br>
    - Sharing rules (Automatically share the rule)<br>
    - Manual sharing (Sharing rules manually)<br>

User management - Manage/Remove person to access org: https://youtu.be/PKpXBb-9s54?si=4PHjSY0aR18I5KMS&t=1274<br>
Assign Permission set to user: https://youtu.be/4X1xyvon4E8?si=r_oYcviNWcOZqdwI&t=806<br>
Assign field level security to user: https://youtu.be/BAMj19o9BmE?si=iIO1Ywswk5IiBIJS&t=194<br>
Set OWD Record security: https://youtu.be/19f59sq6S6I?si=qg_ExhfLgPKxPgrV&t=1096 <br>
Revoke access of object shared with role hierarchy: https://youtu.be/Za3HvlSuTCs?si=n3pK9kgKBUjD6FwT&t=1353 <br>
Shae record to another role using Sharing rule (Based on record owner): https://youtu.be/OphMKt86TMY?si=Gl9gVbzi1GzCwiWs&t=2021 <br>

Data Security playlist in SFC: https://www.youtube.com/watch?v=hqTJ_v7ZzdA&list=PL-gW8Fj5TGrp3d-f6P-58aRgyuKKZdhCp 

What is lightning app builder?<br>
The Lightning App Builder is a point-and-click tool that makes it easy to create custom pages for the Salesforce mobile app and Lightning Experience, giving your users what they need all in one place. 

What is alias is SFC?<br>
An alias is a short name to identify the user on list pages, reports, or other places where their entire name doesn't fit. 

What is leads in SFC?<br>
Leads are people who are interested in your product and service.

Create new lead in SFC: https://youtu.be/IIpFA3mMR8s?si=D__GcQhUZYQx1fxU&t=2 

What is campaign?<br>
It is a collection of Leads and Contacts who have been introduced to specific advertising messages.

What is Account?<br>
Account is a standard object where we storing customer, prospect and partners data. Acccount contains data of leads and contacts. 

customer: customer is the individual who purchases our product<br>
prospect: prospect is a lead who has been qualified by a sales team to match a company's ideal customer profile<br>
partner: partners are the companies with which you collaborate to close your sales deals. 
users: the individual who works at our place to run our business

An individual's information only store in one of the 4 object: 
1. Contacts
2. Leads
3. Accounts
4. Users

What is opportunity?<br>
Opportunity records track details about deals, including which accounts they're for, who the players are, and the amount of potential sales.

What is product object?<br>
In product you are storing information of your service and product. 

What is opportunity line item?<br>
When we add a product to Opportunity it is called Opportunity Line Item which you use during your sales.

What is A/B testing?<br>
If you have a two different content or two different email and you want to see which content performing well then you can use A/B testing.

What is record types?<br>
Record types determine the business processes, picklist values, and page layouts that are available to you when creating records.

What is partner in SFC?<br>
Partners are the companies with which you collaborate to close your sales deals

What is dependent picklist?<br>
A dependent picklist is a custom or multi-select picklist for which the valid values depend on the value of another field, called the controlling field.

What is assignment rule?<br>
Assignment rules define conditions that determine how leads or cases are processed. 

What is salesforce identity?<br>
Salesforce Identity lets you give the right people the right access to the right resources at the right time. You control who can access your orgs and who can use apps running on the Salesforce Platform, on-premises, in other clouds, and on mobile devices.

What is app launcher?<br>
The App Launcher presents tiles for all the standard apps, custom apps, and connected apps in your Salesforce org. Your users can go to one location in Salesforce to access all apps—without having to log in again. 

What's the difference between single sign-on (SSO) and social sign-on?<br>
With SSO, users can access services without logging in to each one. With social sign-on, users can access a service using their social account credentials.

Which objects we can transfer using mass transfer tool?<br>
Use the Mass Transfer tool to transfer multiple accounts, leads, service contracts, and custom objects from one user to another.

How many days after data will be deleted from recyclebin of SFC?<br>
15 Days

How many users we can add at once in SFC?<br>
10

What is queues?<br>
Queues automatically prioritize your support team’s workload by creating lists from which specific agents can jump in to resolve certain types of cases based on category. To efficiently distribute cases and get the right people involved for quicker resolution, creating queues that group support agents by expertise or function and utilizing assignment rules to automatically route cases to the appropriate queues is recommended. This approach streamlines case distribution, ensuring cases are handled by agents best equipped to resolve them promptly.

What is assignmennt rules?<br>
Assignment rules automatically assign incoming cases to specific agents so that the right people work on the right cases.

What is Big deal alerts?<br>
Big Deal Alerts automatically email your users whenever an opportunity reaches a threshold of amount and probability.

What access we can give in salesforce dashboard folder?<br>
View, Edit and Manage

Explain Tabular report <br>
-This report is the simplest and fastest way to look at data. Similar to spreadsheets, it consists simply of an ordered set of fields in columns, with each matching record listed in a row.<br>
-Use this report type for creating lists of records or a list with a single grand total.<br>
-They can't be used to create groups of data or charts, and can't be used in dashboards unless rows are limited.<br>
-Examples include contact mailing lists and activity reports<br>

Explain Summary report <br>
-This report is similar to a tabular report, but allow users to group rows of data, view subtotals, and create charts.<br>
-It can be used as the source report for dashboard components.<br>
-Use this type of report to show subtotals based on the value of a particular field, or when you want to create a hierarchical list, such as all opportunities for your team, subtotal by Stage and Owner.<br>

Explain matrix report<br>
-Matrix reports allow you to group and summarize data by both rows and columns.<br>
-They can be used as the source report for dashboard components.<br>
-Use this type of report for comparing related totals, especially if you have large amounts of data to summarize and you need to compare values in several different fields, or you want to look at data by date and by product, person, or geography.<br>
-Matrix reports without at least one row and one column grouping show as summary reports on the report run page.<br>

Use a controlling picklist to filter the values of one picklist based on the value of another picklist.<br>

What are three ways to group campaigns in salesforce?<br>
- Group campaigns by marketing strategy<br>
- Group campaigns by time period<br>
- Group campaigns by large event

Who can be added to campaigns as members?<br>
Leads, Contacts and Person accounts

What is event monitoring?<br>
Event Monitoring is one of many tools that Salesforce provides to help keep your data secure. It lets you see the granular details of user activity in your organization. You can view information about individual events or track trends in events to swiftly identify abnormal behavior and safeguard your company’s data. Developer Edition organizations have free access to all log types with 1-day data retention.

Which URL you need to use for login into Production org and Sandbox?<br>
Production: You can use https://login.salesforce.com/<br>
Sandbox: You can use http://test.salesforce.com/

What's the difference between page layouts and field-level security?<br>
Unlike page layouts, which only control the visibility of fields on detail and edit pages, field-level security controls the visibility of fields in any part of the app, including related lists, list views, reports, and search results.

How many ways to control record-level access?<br>
There are four ways to control record-level access<br>
Org-wide defaults specify the default level of access users have to each other’s records.<br>
Role hierarchies ensure managers have access to the same records as their subordinates. Each role in the hierarchy represents a level of data access that a user or group of users needs.<br>
Sharing rules are automatic exceptions to org-wide defaults for particular groups of users, to give them access to records they don’t own or can’t normally see.<br>
Manual sharing lets record owners give read and edit permissions to users who might not have access to the record any other way.

What is a public group?<br>
A public group is a collection of individual users, other groups, individual roles or territories, and/or roles or territories with their subordinates that all have a function in common.

What are permission sets groups?<br>
With permission set groups, you can bundle permission sets together based on a job function. A permission set group includes all permissions in the permission sets. You can even include a permission set in more than one permission set group.

What is Quote in CPQ?<br>
A quote is both the document you give the customer and the electronic record of quote data.

What is bundle in CPQ?<br>
A collection of products that's sold together is called a bundle.

What is PDF Quote in CPQ?<br>
A PDF Quote in a CPQ is a list of products the customer wants, pricing information, terms and a signature area. 

Where can i find Recycle Bin button in salesforce?<br>
We can find recycle bin button in classic version of salesforce. <br>
Click on My Profile > Switch to Salesforce Classic > Home > Recycle Bin

How many values we can add in picklist field?<br>
In single-select picklist you can add 1000 values while in multi-select picklist you can add 500 values.<br>
For standard picklist fields limits are below:<br>
Lead Status - 100<br>
Case Status - 100<br>
Opportunity Stage - 100<br>

What are the diffference between Lookup and Master Detail relationship?<br>
![image](https://github.com/Chirag-ahir/SFC-Preparation/assets/72852725/379a4f80-0a2e-4333-8423-8cbcfa343790)

From where can you recover deleted fields of any object?<br>
Go to particular object > Field & Relationships > Deleted fields<br>
![image](https://github.com/Chirag-ahir/SFC-Preparation/assets/72852725/10ae256c-ec79-4e00-9ef0-dd107ef32722)

How many duplicate rules we can create on object ?<br>
You can use up to five active duplicate rules per object.

How many fields we can track of object using field history tracking?<br>
20

What are different ty[es of cloud in salesforce?
Sales cloud
Service cloud
Marketing cloud 
Health cloud
Finance cloud
Data cloud (Recently added)
AI Cloud (Recently added)

What are two types of apps in salesforce?<br>
Standard navigation app<br>
Console navigation app

Can you give example of junction object in non technical terms?<br>
School is a best example of junction object between students and techers. <br>
One students can be studied with multiple techer (One to many)<br>
Onc techer can be give session to multiple students (One to many)<br>
Both teacher and students have many to many relationship between them 

Can you give me real time example of self relationship.<br>
On account object there is a field called parent account which is lookup to account. it is one type of self relationship which is used for denoting parent account (e.g, one company might have it’s parent company) 

Can you give example of roll up summary field.<br>
You can use roll up summary field on account to see total count of opportunities on particular account. 

What is web to case with assignment rules?<br>
- To enable customers to log cases with structured data and route them based on urgency and product line, using Standard Web-to-Case with assignment rules is recommended.<br> 
- This feature allows for the creation of web forms that customers can fill out, which then become cases in Salesforce.<br>
- Assignment rules can then be used to automatically route these cases to the appropriate teams or agents based on predefined criteria, ensuring efficient and relevant case handling.

What is support process<br>
To accommodate the common stages and fields for new product support cases and the additional stages and fields for maintenance cases, implementing Support Processes is recommended. Support Processes allow for the customization of case stages based on the type of support being provided, ensuring that all necessary information is captured accurately for each case type.

What is Einstein Bot?<br>
Einstein Bots can be integrated into websites and configured to provide real-time, automated responses to common customer inquiries, such as order status updates, enhancing the customer experience by providing instant access to information without human intervention. To provide automated self-service on an ecommerce site for customers to check order status, creating an Einstein Bot is recommended.

What is knowledge component?<br>
Knowledge component dynamically suggests articles based on case details, aiding agents in providing accurate and efficient responses. To assist service agents in finding relevant Knowledge articles for new cases, adding the Knowledge component to the Case record page in the Lightning Service Console is recommended.

====================================SFMC=====================================<br>

What are different email terminologies used in SFMC:<br>
We can check status of the email in Tracking tab, which allows her to view:<br>
Sent - Total number of emails sent.<br>
Delivered - Total number of emails delivered.<br>
Deliverability Rate - The percentage of emails that were delivered compared to the number that bounced (soft and hard).<br>
Total Soft Bounces - The number of emails that were recognized by recipients’ mail servers but were returned to the sender because their mailboxes were full or the mail servers were temporarily unavailable.<br>
Total Hard Bounces - Number of emails that permanently bounced back to the sender because the addresses were invalid.<br>
Email Opens - The total number of times subscribers open an email where the images render.<br>
Open Rate - The percentage of emails that were opened (images rendered) compared to the number that were delivered.<br>
Clicks - The number of subscribers who clicked on a link in the email.<br>
Click Rate - The percentage of subscribers who clicked on a link compared to the number of emails delivered<br>
Unsubscribes - Total number of subscribers who clicked unsubscribe.<br>
Unsubscribe Rate - Percentage of subscribers who clicked unsubscribe compared to total number of emails delivered

What is Transactional messages?<br>
Transactional messages are sent in response to a user’s interaction with your website or business or service. Examples include shipping notifications, account alerts, and identity validation. 

What are promotional messages?<br>
Promotional messages are sent to a list of subscribers who have opted-in to receive promotional/marketing-type content from your brand. Examples include newsletters, sale notifications.

What is difference between Sales and Marketing?<br>
Marketing comes before the sales<br>

![image](https://github.com/Chirag-ahir/SFC-Preparation/assets/72852725/5e4bfc80-9273-4e48-98e5-e2629db75641)

What is the difference between B2B and B2C?<br>

![image](https://github.com/Chirag-ahir/SFC-Preparation/assets/72852725/7d2c1336-6db8-47b1-925e-459e626a11db)

What are two data storage options available in SFMC?<br>
Data extensions (Available for all channels)<br>
Subscriber list (Available in email)

What is Data Extension?<br>
A data extension is a table within the application database that contains your data.

What is data filter?<br>
A data filter is a group of criteria that segments a list or data extension.

What is group?<br>
A group is a subset of subscribers you’ve taken from a list. 

What is difference between list and data extension in SFMC?<br>
Lists: A collection of subscribers that receive specific communications. These contain < 500,000 subscribers, offer slower import speed, and a limited number of subscriber attributes.<br>
Data extensions: A table within the database that contains your data. You could use a data extension to store subscriber data (like lists) or any other relational data. These can hold >500,000 subscribers, offer faster import speed, and can be used for SOAP and REST APIs.

What is sales cloud?<br>
Salesforce Sales Cloud is a customer relationship management (CRM) platform designed to support sales, marketing and customer support in both business-to-business (B2B) and business-to-customer (B2C) contexts.

SFMC Definitions:<br>
Agile development: A project methodology used to manage software development work. Agile methodology focuses on completing small, short-term tasks versus a waterfall approach that focuses on a large-scale project.<br>
Bug: An identified error or flaw found in our product that is being tracked for status and completion.<br>
Downtime: The amount of time a product is unavailable.<br>
Emergency release: A product update that occurs when an update needs to be made immediately to fix a bug that is impacting security or performance.<br>
Feature: A change made to Marketing Cloud that adds new functionality or improves current functionality.<br>
Freeze: A cut-off date for changes. Feature freeze relates to what will be added to a release and a release freeze refers to the date no additional changes can be made to an upcoming release.<br>
Functional test: A Quality Assurance (QA) test that evaluates a group of functional requirements.<br>
GA: Denotes a product feature that is generally available (GA) to all customers.<br>
Integration test: A QA test that tests if different parts of the system work together after updates.<br>
Known issues: Issues discovered and logged by members of the Trailblazer Community. These issues are monitored and tracked by Salesforce product teams as bugs.<br>
Lifecycle: The cadence of product improvements and fixes.<br>
Patch release: A weekly release that focuses on fixing bugs and known issues.<br>
Pilot features: A feature offered to a limited number of customers who have signed up to test that feature.<br>
Sprint: A short time period (often 2 weeks) when product teams work on a specific list of tasks.<br>
Stack: The database group that your Marketing Cloud account is part of. Your stack and specific database (called an instance) impacts your account’s release date.<br>
Unit test: A QA test to ensure an individual update meets requirements and follows expected behavior.

what is the difference between Export and Export All? <br>
when you do export it will export all the records of object which is present in SFC while in Export All all the records of that object including records from Recycle bin also export. 

What is ROI?<br>
Return on investment, or ROI, measures the all-important cost-effectiveness of campaigns—that is, how much a campaign earns compared to how much it costs.

What is subscriber key?<br>
Subscriber Key is the primary key for your subscribers and allows you to identify subscribers with a value that you choose.

what is contact key?<br>
The Contact Key is a unique identifier that you assign to a contact.

what is contact id?<br>
The Contact ID is a number Salesforce uses to uniquely identify a contact on the backend. Salesforce uses the Contact ID to identify a contact in various channels.

What is difference between contact and subscriber?<br>
contact is a person you are going to send messages to. A subscriber opted to receive communications or belongs to a particular channel.

what is data designer?<br>
Which type of data source connects two different contact data tables to each other based on a particular field?

What is the right to rectification?<br>
The right to correct personal data

What is Journey Builder?<br>
Journey Builder is a campaign planning tool in Marketing Cloud Engagement. You use it to design and automate campaigns that guide customers through their journey with your brand. 

What is Demographic data?<br>
A subscriber’s name, mailing address, gender, age, birth date, and other information the subscriber shared on a signup form.

What is Behavioral data?<br>
Data from tracking actions across multiple channels, including purchase history, downloads, browsing activity, and email opens, usually accessible in your CRM or analytics platform.

What is Contextual data?<br>
Contextual data delivers information about the moment a subscriber opens an email, including device, location, date, time, or weather.

What is email template?<be>
Email template is a foundation and structure of your email message.

What is Setup Assistant?<br>
Setup Assistant is a prioritized account configuration checklist that guides you through the essential steps to set up your Marketing Cloud account. It provides links to relevant documentation and resources to help you complete each task.

What is IP Allowlist?<br>
 IP Allowlist is a feature that restricts API access to Marketing Cloud from a specific set of IP addresses. 

What is Scrum?<br>
Scrum is a process, with defined roles, meetings, and deliverables that provides the framework to deliver high-quality value to our customers faster.


