# Lab 0 - Set up a Dynamics 365 Contact Center trial environment and configure initial users and roles

**Duration: 15 mins**

**Introduction** This lab introduces the foundational setup required to prepare a Dynamics 365 Contact Center trial environment for future hands-on activities. Learners activate the trial, create the required user accounts, add those users to the environment, assign security roles, and validate sign-in access so each persona is ready for upcoming administrative, supervisory, and agent-based tasks.


## Exercise 1: Create Initial Users in Microsoft 365 Admin Center

This exercise focuses on creating the initial user accounts in the
Microsoft 365 admin center for the personas used throughout the lab
series. Learners assign the appropriate trial license to each user so
the accounts are available for later configuration, access validation,
and role-based exercises.

1.  Open a browser and navigate to the Microsoft 365 admin center:
    !!https://www.microsoft.com/en-us/microsoft-365/business/microsoft-365-administration!!

2.  Select **Admin sign in**.

    ![](./media/image5.png)

3.  Sign in using the Microsoft 365 admin tenant ID.

    ![](./media/image6.png)

    ![](./media/image7.png)

4.  From the left navigation pane, expand **Users** and select **Active
    users**.

    ![](./media/image8.png)

5.  Select **Add a user**.

    ![](./media/image9.png)

6.  In the user creation form, enter the following details:

    - **First name**: !!Mark!!

    - **Last name**: !!Brown!!

    - **Display name**: !!Mark Brown!!

    - **User name**: !!MarkBrown!!

7.  Select all required checkboxes, and then select **Next**.

    ![](./media/image10.png)

8.  Assign the **Dynamics 365 Customer Service Enterprise vTrial**
    license.

9.  Select **Next** to continue.

    ![](./media/image11.png)

10. Again, click on the **Next** button.

    ![](./media/image12.png)

11. Select **Finish adding**.

    ![](./media/image13.png)

12. After the user is created successfully, select **Close**.

    ![](./media/image14.png)

13. Repeat the same steps to create the following users:

    - !!David Flores!!

    - !!Remy Morris!!

    - !!Michael Reynolds!!

    - !!Megan Bowen!!

## Exercise 2: Add Users to the Environment and Assign Security Roles

In this exercise, learners add the newly created users to the Contact
Center trial environment and assign the security roles required for
administrator, supervisor, and agent responsibilities. They also capture
the environment URL, which will be reused in later labs for
persona-based sign-ins and task execution.

1.  Open a new tab, navigate to the Power Platform admin center:
    !!https://admin.powerplatform.microsoft.com/!!

2.  Sign in using the Microsoft 365 admin tenant credentials.

    ![](./media/image15.png)

3.  From the left navigation pane, select **Manage**.

4.  Select **Environments**.

5.  Open the **ContactCenter trial** environment.

    ![](./media/image16.png)

6.  In the environment page, locate the **Users** section and select
    **See all**.

    ![](./media/image17.png)

7.  From the top bar, select **+ Add user**.

    ![](./media/image18.png)

8.  In the search field, enter !!Mark Brown!!.

9.  Select **Mark Brown** from the search results, and then select
    **Add**.

    ![](./media/image19.png)

10. Assign the following roles:

    - **Omnichannel Administrator**

    - **System Administrator**

    ![](./media/image20.png)

    ![](./media/image21.png)

11. On the confirmation window, select **Save** again.

    ![](./media/image22.png)

12. Repeat the same process to add the following users with their
    respective roles:

    - **David Flores** – **Customer Service Representative and
      Omnichannel Agent**

    - **Remy Morris** – **CSR Manager** and **Omnichannel Supervisor**

    - **Michael Reynolds** — **App Profile Manager Administrator and
      Basic User**

    - **Megan Bowen – Omnichannel Agent and Basic User**

13. Click on the **ContactCenter Trial** environment.

    ![](./media/image23.png)

14. Copy the URL and save it in Notepad. This URL is used to log in to
    the Copilot Service Admin Center or the Copilot Service workspace by
    signing in with different user accounts.

    ![](./media/image24.png)

## Exercise 3: Reset Passwords and Validate User Access

This exercise finalizes the setup by resetting temporary passwords and
validating that each user can successfully sign in to the environment.
Learners confirm access for the created personas and save the
credentials needed to support future labs.

1.  In the Microsoft 365 admin center, navigate to the **Active**
    **users** section.

2.  Open the required user account by selecting the user name.

    ![](./media/image25.png)

3.  From the top menu, select **Reset password**.

    ![](./media/image26.png)

4.  On the confirmation page, select **Reset password** again.

    ![](./media/image27.png)

5.  Review the generated sign-in details displayed on the screen.

6.  If the password is hidden, select **Show** to view it.

7.  Note the **Username** and **Password** for later sign-in.

    ![](./media/image28.png)

8.  Open a **new private (InPrivate/Incognito) browser window**.

9.  Navigate to the **URL copied from the Contact Center Trial
    environment**.

10. On the sign-in page, enter the **user tenant for David Flores** in
    the required field, and then click **Next**.

    ![](./media/image29.png)

11. Enter the **temporary password** that was extracted from the
    **Microsoft Admin Center**, and then click **Sign in**.

    ![](./media/image30.png)

12. When prompted, enter the **current (temporary) password**, then
    **set a new password** as required, and click **Sign in**.

    ![](./media/image31.png)

13. When asked **“Stay signed in?”**, click **Yes**.

    ![](./media/image32.png)

14. You will be redirected to the **David Flores Dynamics 365 app
    selector window**.

15. The apps displayed in this window depend on the **roles assigned**
    to the user in the **Power Platform Admin Center environment**.

    ![](./media/image33.png)

16. Repeat the **same steps** to set up passwords for **all other
    users** that were created.

17. Save **all User IDs and passwords** in a **Notepad file**.

18. These user credentials and the **environment URL** will be required
    for **future labs**.

## Conclusion

By completing this lab, learners establish a fully prepared Dynamics 365
Contact Center trial environment with the required users, role
assignments, and validated access. This setup creates the baseline
needed to support the remaining labs and ensures each persona can
participate in future configuration and operational scenarios.
