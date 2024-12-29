![image](https://github.com/user-attachments/assets/43e35afa-fe11-495c-b8c1-d927b8f5872b)


<h1 align = 'center'>Google Workspace Administration</h1>

<p> This comprehensive project focuses on Google Workspace Administration as part of my IT support and administration professional development. This project encompasses the setup, configuration, and management of a Google Workspace environment, highlighting key administrative tasks such as user provisioning, organizational unit structuring, and policy enforcement. The objective is to demonstrate proficiency in managing cloud-based productivity tools like Google Workspace, ensuring secure and efficient operations within an organizational context.</p>

<h2>Objectives</h2>
<h3>User Addition</h3>

- Manual addition of individual users
- Bulk additon of multiple users
- Addition of email alias for users
  
<h3>Creation of Organizational Units</h3>

- Creating Organizational Units to simulate real-world scenarios 

<h3>Enforce Security Policies</h3>

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


  For the purpose of this exercise, I have already signed up to the Google Workspace trial account, and connected a subdomain from [Carrd](https://carrd.co/).
  Best practice to creating a Google Workspace domain is to connect and verify a domain that an organization owns

<h3>&#9312; User Addition</h3>

<h4>Addition of indivdual users</h4>
  
  I. In the admin console, go to "Directory" > Users > Click "Add new user"

![image](https://github.com/user-attachments/assets/15a913a6-de70-4fa1-a272-20be4e149fdc)

  II. Fill out the form that appears. You can choose to add a password or let Google Workspace automatically generate password
  
 III. Click "ADD NEW USER" to create the account

  
![image](https://github.com/user-attachments/assets/341daa28-6de5-447f-8691-1f47b3097de4)

  ![image](https://github.com/user-attachments/assets/325f8224-aad2-451d-93e1-396f1de9837b)

 <br>
 <br>

 <h4>Bulk addition of multiple users</h4>
  
   I. In the admin console, go to "Directory" > Users > Click "Bulk update users"
  
   II. Click "DOWNLOAD BLANK CSV TEMPLATE". This will download a blank file with all the required columns to your local machine.
   
   ![image](https://github.com/user-attachments/assets/54be859f-ddbd-4119-ab64-b1ef1080c9aa)


   III. Open CSV file in an spreadsheet application and populate the file with user information
   
  The following columns are mandatory:
  - First Name
  - Last Name
  - Email Address
  - Password (enter hellohello1)
  - Organizational Unit Path (For this exercise, enter the forward slash symbol / into this column. This represents the root organization)

![image](https://github.com/user-attachments/assets/08ccaced-26f0-438c-8877-f1a06ec0929f)

IV. Return to the 'Bulk update users' dialog box, click "ATTACH CSV FILE" and browse to your
file, then click "UPLOAD" to  create the user accounts.

- If your file has formatting errors, a warning prompts that you may need to re-edit the file.
- If successful, the progress of the upload will be reported in the Tasks list at the top of the
page. 

![image](https://github.com/user-attachments/assets/a629508f-e716-4705-9054-84bbd6d0770e)


IV. The new users may take a couple of minutes to appear in the user list. If you don’t see them right away, try refreshing the screen.

![image](https://github.com/user-attachments/assets/dc2db5f9-8d7c-4baf-8744-41758459a0d6)
