# SFC-Preparation

What is salesforce?<br>
Salesforce is a cloud-based CRM platform that helps business to manage their sales, marketing and customer service activities. 

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

What is page layout?
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

What is lightning app builder?<br>
The Lightning App Builder is a point-and-click tool that makes it easy to create custom pages for the Salesforce mobile app and Lightning Experience, giving your users what they need all in one place. 

What is alias is SFC?<br>
An alias is a short name to identify the user on list pages, reports, or other places where their entire name doesn't fit. 

What is leads in SFC?<br>
Leads are people who are interested in your product and service.

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

========================================================SFMC=================================================<br>

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



