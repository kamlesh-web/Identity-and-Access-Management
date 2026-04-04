**Detailed Step-by-Step Guide: How To Create AWS Users And Groups**

### Step 1: Log in to the AWS Management Console
Navigate to **https://signin.aws.amazon.com/** and sign in as the **root user**.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/af9f694a-7139-40b0-b45b-1c0119bfc40f" />

**What the screenshot shows**: The AWS sign-in page with the “Root user” option selected and the email address field ready.

### Step 2: Search for IAM
In the top search bar, type **IAM**.

**What the screenshot shows**: The AWS Console Home page with the search bar active.

### Step 3: Open the IAM Service
From the search results, click **IAM** to open the Identity and Access Management dashboard.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/4ffa26ca-b2e4-4a48-beae-104635a93cea" />

**What the screenshot shows**: The search dropdown highlighting IAM under Services.

### Step 4: Go to Users Section
In the IAM dashboard, click **Users** in the left navigation menu.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/821efa29-93eb-4594-816f-82d23c76375e" />

**What the screenshot shows**: The IAM Dashboard with the left sidebar expanded and “Users” highlighted under Access Management.

### Step 5: Start Creating a New User
Click the **Create user** button (orange) at the top right.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/7e9fbe15-6f03-422d-a8e1-43100f1b8700" />

**What the screenshot shows**: The Users list page with the Create user button visible.

### Step 6: Enter User Details
- In the **User name** field, enter a name (example used: **NewUser**).
- Check the box **Provide user access to the AWS Management Console**.
- Click **Next**.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/a5baf4fd-5881-476c-ba0a-2ccc44f20b42" />

**What the screenshot shows**: The “Specify user details” page with the console access checkbox selected.

### Step 7: Set a Custom Password
- Select **Custom password**.
- Enter a strong password.
- Check the box **Users must create a new password at next sign-in** (recommended).
- Click **Next**.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/4ab777c1-711e-4fd0-b832-e6530b02fad4" />

**What the screenshot shows**: The password settings section with the custom password option and the required checkbox selected.

### Step 8: Choose Permissions Option
For a single user (as in this example), select **Attach policies directly**.  
(For multiple users, the recommended best practice is “Add user to group” instead.)
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/6a342ea6-826c-45a4-969a-d417f9af23a4" />

**What the screenshot shows**: The “Set permissions” page with the three options displayed and “Attach policies directly” selected.

### Step 9: Attach Policies to the User
- In the search box, type the name of the policy you want (for example, AdministratorAccess or AmazonEC2FullAccess).
- Check the box next to the policy (or policies) you need.
- Click **Next** at the bottom.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/6d84e2d8-c34a-47d8-9f84-8837c3b7bf80" />

**What the screenshot shows**: The policies list with the search bar and selected policies ready.

### Step 10: Review and Continue
Review the selected policies, then click **Next**.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/2da8486c-332a-41a3-8ce6-bfcf55eba236" />

**What the screenshot shows**: The permissions review page with the Next button at the bottom.

### Step 11: Create the User
Click **Create user** to finish.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/7716388d-6bd5-4266-8797-aab296485190" />

**What the screenshot shows**: The final review screen with the Create user button highlighted.

### Step 12: Download Credentials
Click **Download .csv file** to save the user’s sign-in credentials (URL, username, and temporary password).  
This is the only time you can download the password.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/05d09900-6f0c-4c50-8ca1-b1cbca7a83f4" />

**What the screenshot shows**: The success page with the green banner and the Download .csv file button.

### Step 13: Test the New IAM User
- Copy the **Console sign-in URL** from the success page.
- Open a new browser tab, paste the URL, and sign in with the username and password from the .csv file.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/460749a7-66c7-4f6e-947e-84b9343a51b0" />

**What the screenshot shows**: The success message with the sign-in URL highlighted.

### Step 14: Sign In as IAM User
The Account ID is automatically filled when using the copied URL. Enter the username and password.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/b249d7d7-509a-4b5b-ba2b-43450182068b" />

**What the screenshot shows**: The IAM user sign-in page with the Sign in button.

### Step 15: Verify Successful Sign-In
You should now be logged in as the new IAM user (you will see the user name at the top right).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/0c4468db-ecec-49b8-b149-68aaa0c63e0f" />

**What the screenshot shows**: The AWS Console Home page after successful IAM user login.

### Step 16: Return to Root Account and Create a Group
Sign out of the IAM user account and sign back in as the root user.  
Then go to IAM → **User groups** (or click Users first if needed).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/de556318-d107-4efd-bba8-d2e890b0d8ee" />

**What the screenshot shows**: The IAM Users page for the newly created user.

### Step 17: Start Creating a Group
Click **Create group** (orange button) at the top right.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/2495a615-ec3f-4924-a5f0-bb785060b678" />

**What the screenshot shows**: The empty User groups list with the Create group button.

### Step 18: Name the Group
Enter a **User group name** (example used: **New_group**).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/9f2a7f2e-b018-4de6-ad4f-65bce5431617" />

**What the screenshot shows**: The “Create user group” page with the name field active.

### Step 19: Attach Policies to the Group
In the **Attach permissions policies** section, search for and select the policies you want the entire group to have (example: AmazonAuroraRDSFullAccess, AmazonEC2FullAccess, etc.).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/eee85b67-c10e-41e9-8873-8eef469e1dbb" />

**What the screenshot shows**: The policies list with the search bar and selected policies.

### Step 20: Confirm Policy Selection
After selecting the policies, scroll down to **Create user group**.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/7b85221b-3a26-4ee1-8967-eaa54e209a1f" />

**What the screenshot shows**: The bottom of the permissions page with the Create user group button.

### Step 21: Finalize Group Creation
Click **Create user group** to complete the process.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/0e321f8f-3f12-4622-8677-9abaefce76ef" />

**What the screenshot shows**: The full list of available policies with the final Create button.

### Step 22: View the New Group
In the User groups list, click the group name (**New_group**) to open its details.
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/525334d3-d8dc-415c-8931-08b83eb2c249" />

**What the screenshot shows**: The User groups list with the new group highlighted.

### Step 23: Check Users in the Group
On the group details page, go to the **Users** tab to see which users are members (example: **NewUser**).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/fd2f3c30-3037-4f3d-aa41-0005708d6081" />

**What the screenshot shows**: The group summary page with the Users tab and the added user listed.

### Step 24: Check Group Permissions
Switch to the **Permissions** tab to see all policies attached to the group (and therefore inherited by the user).
<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/3fefe374-a38f-4757-b37b-f77b2d1ad4d5" />

**What the screenshot shows**: The Permissions tab listing the attached policies (e.g., AmazonAuroraRDSFullAccess and others).

---

**Important Notes & Best Practices**
- Always use IAM users and groups instead of the root account for everyday work.
- Attach policies to groups whenever possible. It is much easier to manage permissions for many users.
- The .csv file from Step 12 contains sensitive credentials, store it securely and delete it after use.
- Force password reset on first login (Step 7) improves security.
- You can add the user to the group later if you create the user first (or attach policies directly as shown).
