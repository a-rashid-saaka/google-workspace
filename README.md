![image](https://github.com/user-attachments/assets/43e35afa-fe11-495c-b8c1-d927b8f5872b)


<h1 align = 'center'>Google Workspace Administration</h1>

<p> This comprehensive project focuses on Google Workspace Administration as part of my IT support and administration professional development. This project encompasses the setup, configuration, and management of a Google Workspace environment, highlighting key administrative tasks such as user provisioning, organizational unit structuring, and policy enforcement. The objective is to demonstrate proficiency in managing cloud-based productivity tools like Google Workspace, ensuring secure and efficient operations within an organizational context.</p>

<h2>Objectives</h2>
<h3>User Addition</h3>

- Manual addition of individual users
- Bulk addition of multiple users
- Addition of email alias for users
  
<h3>Creation of Organizational Units</h3>

- Creating Organizational Units to simulate real-world scenarios 

<h3>Configure Security Settings</h3>

- Configure and enforce some basic security policies

<h3>Configure Email and Drive settings</h3>

- 

<h3>Troubleshoot some common issues</h3>

- Password Reset
- Rename user 

<h2>Environments and Technologies Used</h2>

- Google Workspace Admin console
- Windows 10

<br>
<br>


  For this exercise, I have already signed up for the Google Workspace trial account and connected a subdomain from [Carrd](https://carrd.co/).
  The best practice for creating a Google Workspace domain is to connect and verify a domain that an organization owns

<h3>&#9312; User Addition</h3>

<h4>Addition of individual users</h4>
  
  I. In the admin console, go to "Directory" > Users > Click "Add new user"

![image](https://github.com/user-attachments/assets/15a913a6-de70-4fa1-a272-20be4e149fdc)

  II. Fill out the form that appears. You can choose to add a password or let Google Workspace automatically generate a password
  
 III. Click "ADD NEW USER" to create the account

  
![image](https://github.com/user-attachments/assets/341daa28-6de5-447f-8691-1f47b3097de4)

  ![image](https://github.com/user-attachments/assets/325f8224-aad2-451d-93e1-396f1de9837b)

 <br>
 <br>

 <h4>Bulk addition of multiple users</h4>
  
   I. In the admin console, go to "Directory" > Users > Click "Bulk update users"
  
   II. Click "DOWNLOAD BLANK CSV TEMPLATE". This will download a blank file with all the required columns to your local machine.
   
   ![image](https://github.com/user-attachments/assets/54be859f-ddbd-4119-ab64-b1ef1080c9aa)


   III. Open the CSV file in a spreadsheet application and populate the file with user information
   
  The following columns are mandatory:
  - First Name
  - Last Name
  - Email Address
  - Password (enter hellohello1)
  - Organizational Unit Path (For this exercise, enter the forward slash symbol / into this column. This represents the root organization)

![image](https://github.com/user-attachments/assets/08ccaced-26f0-438c-8877-f1a06ec0929f)

IV. Return to the 'Bulk update users' dialog box, click "ATTACH CSV FILE" and browse to your
file, then click "UPLOAD" to  create the user accounts.

- If your file has formatting errors, a warning will prompt you to re-edit it.
- If successful, the upload progress will be reported in the Tasks list at the top of the
page. 

![image](https://github.com/user-attachments/assets/a629508f-e716-4705-9054-84bbd6d0770e)


IV. The new users may take a couple of minutes to appear in the user list. If you don’t see them right away, try refreshing the screen.

![image](https://github.com/user-attachments/assets/dc2db5f9-8d7c-4baf-8744-41758459a0d6)

<br>
<br>

<h4>Addition of Email alias</h4>

In this exercise, we will create a user's email alias. An email alias allows a user to receive emails sent to multiple addresses in their Gmail inbox.

I. In the left panel in the admin console, click "Directory" > Users

II. Locate Jon Snow in the user list, select his name, and click the "User information" section.

III Click the "Alternative email addresses (email alias)" section.

IV. In the "Alternative email" text field, enter "jonny" and click "SAVE".
   
   ![image](https://github.com/user-attachments/assets/705fff6b-cfe2-4629-b977-ff9965cd5830)

<strong>NOTE:</strong> Though the user can receive emails on the new email alias added to his account, he can only log in to his Google Workspace account with his primary email address

<br>
<br>

<h3>&#9313; Creation of Organizational Units</h3>
I. In the left panel, select "Directory" > Organizational Units > click "Create organizational unit"


![image](https://github.com/user-attachments/assets/158ac30a-f51b-4755-84c4-ecee60156d81)

 II. Give the OU the name of "Employees", provide a description if required, and click "CREATE".


![image](https://github.com/user-attachments/assets/b01fe68d-d41a-4270-8f4b-fc1ca7e21641)

III. Follow the steps to create another OU called "Executive"

IV. Navigate to your users list. You should see the two new OUs on the left hand side beneath top level organization.

V. Select Edwin Jon, and Elias Grey by checking the box to the left of their name in the user list.

VI. Click More options > Change organizational unit, and select Executive. Then click
CONTINUE.


![image](https://github.com/user-attachments/assets/df162f0a-f398-4aa6-9678-fcd20d1216e5)

![image](https://github.com/user-attachments/assets/8d2a8c66-e214-4cb5-b47d-df147cf7c203)

VII. Click CHANGE to confirm the move.


![image](https://github.com/user-attachments/assets/0be48ba9-dc40-4e78-bdee-f99c69b940d4)

VIII. Repeat Steps V - VII but this time move Ellie, Jon, Tom, and Will to the Employees OU.

<br>
<br>

<h3>&#9314; Configuring common security settings</h3>

In this section, we will review and set some common security features and settings for our organization.

<h4>Enabling 2-step verification for users</h4>

I. Select "Security" from the left panel in the admin console > select "Authentication" to expand the list of options 

II. Select "2-step verification" and review the settings.

III. Ensure "Allow users to turn on 2-Step verification" is checked. This makes 2-step verification available for your users. Click "SAVE"

![image](https://github.com/user-attachments/assets/19f40d13-4881-4434-a17c-47048580f7e5)


<h4>Password Management</h4>

I. On the "Security" page, scroll down and select "Password management".
 
II. Google Workspace supports many password policies.
- You can enforce password strength and also set a password length policy by setting minimum and maximum length values. 
- You can enforce the length and strength policies when users sign in to their account or when they change their password. The default enforcement occurs when the password is next changed.
- You can choose whether to allow users to reuse their old passwords although this is not recommended. 
- Finally, you can enforce password expiry although we recommend you allow passwords to never expire.
- Settings can be applied at the OU level



  ![image](https://github.com/user-attachments/assets/662a2e8b-4c64-4c0a-878a-2b0683157bce)

   

<h4>Account Recovery</h4>

I. Return to the "Security" page, scroll down and click "Account Recovery."

II. This setting allows you to control whether a Super Admin can recover their account themselves using the Forgot Password link, or whether they must ask another Super Admin or Google Support to reset their password.

III. This setting is also where you control whether users can recover their own passwords. This is achieved through the use of a recovery email address or phone number. Note that password recovery is not available when using SSO, and 2-step verification users must use the email recovery option.

IV. By default, only a domain administrator can reset a user’s password. To enable user password recovery, click User account recovery and check the Allow users and non-super
admins to recover their account box, Then click SAVE.

![image](https://github.com/user-attachments/assets/abceb274-bf16-4fb2-a9e4-9051a6eb034e)

V. Settings can be applied at the OU level

<h4>Configuring Session Controls</h4>

As an administrator, you can control how long users stay signed in to Google services like Gmail. Session lengths can be set from 1 hour to indefinite, with the default being 14 days.

<strong>Scenario</strong>

To enhance security, your company requires off-site consultants to sign in to their laptops at least once a day, ensuring that no device is left with an active Google Workspace session.

I. Click the "Security" icon > select "Access and data control" > click "Google session control."

II. Click on the "Consultants" OU (left side of the page).

III. Set 'Session control' to 8 hrs.

IV. Click "OVERRIDE." This will override the top-level organization's setting of 14 days.

![image](https://github.com/user-attachments/assets/a144ff69-4887-4150-89e1-84fc7d9ac8e1)

<h4>Less Secure Apps Restriction</h4>

I. On the Security page, scroll down, and click "Less secure apps."

Some third-party apps continue to use less secure sign-in technology. You can choose to deny access for these apps, which we recommend, or choose to allow access despite the risks.

II. Make sure that "Disable access to less secure apps (recommended)" is selected. Click SAVE if you need to change this setting.

III. This policy can be applied at the OU level.

![image](https://github.com/user-attachments/assets/aa9b2a88-ab61-48cc-9780-b59bb69389d3)
