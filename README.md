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

- Configuring and enforcing some basic security policies

<h3>Configure Email settings</h3>

- Configuring email settings for better security

<h3>Troubleshoot some common issues</h3>

- Resetting user passwords
- Renaming of users 

<h2>Environments and Technologies Used</h2>

- Google Workspace Admin console
- Windows 10

<br>

<h3>Background</h3>

  For this exercise, I have already signed up for the Google Workspace trial account and connected a subdomain from [Carrd](https://carrd.co/).
  The best practice for creating a Google Workspace domain is to connect and verify a domain that an organization owns

<h3>&#9312; User Addition</h3>

<h4>Adding individual users</h4>
  
  I. In the admin console, go to "Directory" > Users > Click "Add new user"

![image](https://github.com/user-attachments/assets/15a913a6-de70-4fa1-a272-20be4e149fdc)

  II. Fill out the form that appears. You can choose to add a password or let Google Workspace automatically generate a password
  
 III. Click "ADD NEW USER" to create the account

  
![image](https://github.com/user-attachments/assets/341daa28-6de5-447f-8691-1f47b3097de4)

  ![image](https://github.com/user-attachments/assets/325f8224-aad2-451d-93e1-396f1de9837b)

 <br>
 <br>

 <h4>Adding multiple users in bulk</h4>
  
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

<h4>Adding Email alias</h4>

In this exercise, we will create a user's email alias. An email alias allows a user to receive emails sent to multiple addresses in their Gmail inbox.

I. In the left panel in the admin console, click "Directory" > Users

II. Locate Jon Snow in the user list, select his name, and click the "User information" section.

III Click the "Alternative email addresses (email alias)" section.

IV. In the "Alternative email" text field, enter "jonny" and click "SAVE".
   
   ![image](https://github.com/user-attachments/assets/705fff6b-cfe2-4629-b977-ff9965cd5830)

<strong>NOTE:</strong> Though the user can receive emails on the new email alias added to his account, he can only log in to his Google Workspace account with his primary email address

<br>
<br>

<h3>&#9313; Creating Organizational Units</h3>


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

<br>

<h4>Password Management</h4>

I. On the "Security" page, scroll down and select "Password management".
 
II. Google Workspace supports many password policies.
- You can enforce password strength and also set a password length policy by setting minimum and maximum length values. 
- You can enforce the length and strength policies when users sign in to their account or when they change their password. The default enforcement occurs when the password is next changed.
- You can choose whether to allow users to reuse their old passwords although this is not recommended. 
- Finally, you can enforce password expiry although we recommend you allow passwords to never expire.
- Settings can be applied at the OU level



  ![image](https://github.com/user-attachments/assets/662a2e8b-4c64-4c0a-878a-2b0683157bce)

   <br>

<h4>Account Recovery</h4>

I. Return to the "Security" page, scroll down and click "Account Recovery."

II. This setting allows you to control whether a Super Admin can recover their account themselves using the Forgot Password link, or whether they must ask another Super Admin or Google Support to reset their password.

III. This setting is also where you control whether users can recover their own passwords. This is achieved through the use of a recovery email address or phone number. Note that password recovery is not available when using SSO, and 2-step verification users must use the email recovery option.

IV. By default, only a domain administrator can reset a user’s password. To enable user password recovery, click User account recovery and check the Allow users and non-super
admins to recover their account box, Then click SAVE.

![image](https://github.com/user-attachments/assets/abceb274-bf16-4fb2-a9e4-9051a6eb034e)

V. Settings can be applied at the OU level

<br>

<h4>Configuring Session Controls</h4>

As an administrator, you can control how long users stay signed in to Google services like Gmail. Session lengths can be set from 1 hour to indefinite, with the default being 14 days.

<strong>Scenario</strong>

To enhance security, your company requires off-site consultants to sign in to their laptops at least once a day, ensuring that no device is left with an active Google Workspace session.

I. Click the "Security" icon > select "Access and data control" > click "Google session control."

II. Click on the "Consultants" OU (left side of the page).

III. Set "Session control" to 8 hrs.

IV. Click "OVERRIDE." This will override the top-level organization's setting of 14 days.

![image](https://github.com/user-attachments/assets/a144ff69-4887-4150-89e1-84fc7d9ac8e1)

<br>

<h4>Less Secure Apps Restriction</h4>

I. On the Security page, scroll down, and click "Less secure apps."

Some third-party apps continue to use less secure sign-in technology. You can choose to deny access for these apps, which we recommend, or choose to allow access despite the risks.

II. Make sure that "Disable access to less secure apps (recommended)" is selected. Click SAVE if you need to change this setting.

III. This policy can be applied at the OU level.

![image](https://github.com/user-attachments/assets/aa9b2a88-ab61-48cc-9780-b59bb69389d3)

<br>
<br>

<h3>&#9315; Configuring Email settings</h3>

<h4>Configuring Email Safety</h4>

I. Click the "Apps" icon > Google Workspace > click the "Gmail" service > Click "Safety."

This will take you to the Safety page which is divided into four sections:
- Attachments: Policies to protect against malware.
- IMAP view time protections: Malicious link protection for users of IMAP clients.
- Links and external images: Prevent email phishing attacks.
- Spoofing and authentication: Reduce phishing due to spoofing and unauthenticated emails.
  
II. Click the "Attachments" card to manage protections. You can enable or disable settings and view the default actions.

III. If not already enabled, check 'Protect against encrypted attachments from untrusted senders' and choose an action for messages that trigger this policy. The options are:
- Keep email in the inbox and show warning (default)
- Move email to spam
- Quarantine

IV. If you choose to quarantine the message you will be able to select which quarantine to use.

V. Choose a desired option and click SAVE.

![image](https://github.com/user-attachments/assets/18be5081-75fa-4877-8c5f-9657dabe0efb)

Explore the other settings in this section and also click on each of the other three cards and review the available settings

<br>

<h4>Configuring end user access</h4> 

<strong>Scenario</strong>

Your company strongly emphasizes the confidentiality of corporate information. John, the CEO, has become aware that it is common practice for non-permanent staff to use their personal email accounts to conduct business. Some non-permanent staff have created a Gmail filter that forwards all mail received to their personal account, and John would like to stop this practice.


I. Click the "Apps" icon >  Google Workspace > click the "Gmail" service.

II. Click "End User Access." You will need to scroll down to see this section if you don't mind.

III. Click on your top-level organization on the left to ensure that POP and IMAP access are set to OFF.

IV. If you made changes, click SAVE.

![image](https://github.com/user-attachments/assets/3db283ac-37be-41a4-8f3a-b4d07fc77697)

V. Click the "Consultants" OU.

VI. Click on the Automatic forwarding row and ensure the "Allow users to automatically forward incoming email to another address" box is unchecked. Any existing forwarding rules will now cease working

VII. Click OVERRIDE (you are overriding the inherited setting from the top-level organization).

![image](https://github.com/user-attachments/assets/2fcbb878-5c51-4ec3-a01f-d2f0543d9e1e)

<br>

<h4>Creating an email allowlist and a blocked sender list</h4>

If legitimate emails from specific contacts are marked as spam, you can add their IP address to an allowlist so that messages from them are no longer flagged as spam.

A blocked sender list includes email addresses that cannot send emails to your domain. Administrators can block specific users or entire domains.

- Creating an Allowlist

I. Click  "Apps" >  Google Workspace > click the "Gmail" service.

II. Scroll down and click "Spam, Phishing and Malware."

III. Click on the 'Email allowlist' row, and add an IP address. If you want to add more IP addresses, separate entries with a comma.

IV. Click SAVE.

![image](https://github.com/user-attachments/assets/f4f3084f-f385-40eb-8c80-1f13eb3526bc)


- Creating a blocked sender list</h4>
  
I. On the "Spam, Phishing and Malware" settings page, scroll down to the "Blocked senders" row and click "CONFIGURE."

II. Enter a short description.

III. Click "Create or edit list." This will open the address list page in a new tab.

![image](https://github.com/user-attachments/assets/93149f2e-fb1b-4a17-ae9f-2c6f16eb38a6)

IV. Click "ADD BLOCKED LIST."
  
V. Enter a name for the list, and click "Add' or "ADD ADDRESS" to add a list entry
  
VI. Enter the email address of your external account, then click "SAVE." Note: In addition to user
email addresses, you can enter domain names here.

![image](https://github.com/user-attachments/assets/68e872cf-d5ae-451e-a863-0ebc6f7038bf)

VII. Return to the "Spam, Phishing and Malware" tab, and click Use existing list.

VIII. Select the "Block senders" list you created, and click "SAVE"
    
![image](https://github.com/user-attachments/assets/9f862657-143f-4165-a249-f55898af4814)


![image](https://github.com/user-attachments/assets/bd4629c4-7a4d-46a2-ae0e-2a7b22746923)


<br>

<h4>Creating an approved sender list</h4>

The main distinction between an email allowlist and an approved sender list is that the latter permits the addition of email addresses and domain names, while the allowlist is restricted to IP addresses only.

I. Click the "Apps" icon > Google Workspace > click the "Gmail" service.

II. Scroll down and click "Spam, Phishing and Malware."

III. Scroll down to the "Spam" row and click "CONFIGURE."
   
IV. Enter a short description.
   
V. Check the "Bypass spam filters for messages from senders or domains in selected lists" box and click the Create or edit list link. This will open the address list page in a new tab.

VI. Click "ADD ADDRESS LIST."
    
VII. Enter a name for the list of Approved senders.
    
VIII. Click "Add or ADD ADDRESS" to add a list entry.
    
IX. Enter the email address of someone external to your organization that you trust and click "SAVE."
    
X. Return to the "Spam, Phishing and Malware" tab, and click Use existing list.
    
XI. Select your Approved senders list, and click "SAVE."
    
You have just successfully created an approved sender list for your organization.


![image](https://github.com/user-attachments/assets/efc90909-6380-4085-a70f-65b5b093cc22)


![image](https://github.com/user-attachments/assets/727eebbc-1b95-46e7-859a-c66d7feccaf9)

<br>
<br>

<h3>&#9316; Troubleshooting some common issues</h3>

<h4>Resetting user password</h4>

<strong>Scenario</strong>
An employee, Elias Grey, reaches out to the IT administrator because he has forgotten his password for his corporate Gmail account under the organization's Google Workspace.


I. In the left panel, click "Directory" > Users.

II. Access the reset password function in one of two ways:
- Option 1: Hover over Elias Grey in the user list and click "Reset password" on the right.
- Option 2: Click on Elias Grey in the user list to open his profile and then click "RESET PASSWORD" on the left.
  
III. In the "Reset password" dialog box, there are two options:
- Option 1: Allow Google to auto-generate a password.
  - Click RESET.
 

- Option 2: Create a temporary password.
   - Check the "Ask for a password change at the next sign-in" box.
   - Click RESET.

    ![image](https://github.com/user-attachments/assets/c713e04c-2a8d-46b3-82fa-784643e0bedb)


IV. In either option, click the COPY PASSWORD link to copy the password to your clipboard and then click DONE.

![image](https://github.com/user-attachments/assets/f0407965-646a-4c60-ba1e-d0fcc4e9cdfe)

V. Provide Elias with his new password. When he next signs in he will be asked to change his password.
