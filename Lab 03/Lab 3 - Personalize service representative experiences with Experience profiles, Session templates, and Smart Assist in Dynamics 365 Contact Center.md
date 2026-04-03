# Lab 3 - Personalize service representative experiences with Experience profiles, Session templates, and Smart Assist in Dynamics 365 Contact Center

**Duration: 30 mins**

**Introduction**

This lab guide focuses on configuring the workspace and guided
assistance components in Dynamics 365 Contact Center. Learners create an
Experience Profile, enable productivity tools for an assigned agent,
configure a session template, register an application for bot
integration, and add Smart Assist and script guidance to the support
experience. By completing these exercises, learners gain practical
experience in preparing a structured agent workspace that supports
consistent session handling, guided productivity, and more efficient
customer engagement.

## Exercise 1 - Create and Configure an Experience Profile

In this exercise, learners create a new Experience Profile and prepare
it for agent use in the Contact Center environment. They add an agent
user, enable productivity tools, and define the rank and role settings
for the profile. This exercise establishes the profile structure that
controls how the assigned agent accesses workspace capabilities and
support tools.

### Task 1 - Create an Experience Profile

1.  Open a new private window. Use the URL that we extracted from the
    Power Platform admin center and log in to the Contact Center
    environment by using Michael Reynolds’s credentials. Michael
    Reynolds is assigned the **App Profile Manager Administrator and
    Basic User**.

    > Note: If you have any confusion about the login. Revisit Exercise 4 of Lab 0.

2.  On the App selector, select **Copilot Service admin center**.

    ![](./media/image1.png)

3.  In the left navigation pane, under **Support experience**, select
    **Workspaces**.

4.  In the **Experience profile** section, select **Manage**.

    ![](./media/image2.png)

5.  On the Experience Profiles page, select **+ New**.

    ![](./media/image3.png)

6.  On the **Create a new experience profile** dialog, enter the
    following details:

    - **Name**: !!Contoso Agent!!

    - **Unique name**: !!msdyn_custom_chatagent!!

    - **Description**: !!Contoso Agent!!

7.  Select **Create**.

    ![](./media/image4.png)

8.  Verify that the **Contoso Agent** Experience Profile is created
    successfully.

    ![](./media/image5.png)

### Task 2 - Enable Productivity Tools

1.  In the **Users** section, select **Add Users**.

    ![](./media/image6.png)

2.  Select **Megan Bowen**, and then select **Add**.

    ![](./media/image7.png)

3.  In the **Productivity pane**, select **Turn on**.

    ![](./media/image8.png)

4.  Enable the available productivity tools that agents can access while
    working on assigned tasks.

5.  Select **Save and Close**.

    ![](./media/image9.png)

### Task 3 - Set Rank and Roles

1.  Return to the **Experience Profiles** page.

2.  Select the **Contoso Agent** Experience Profile.

3.  From the top menu, select **Set Rank and Roles**.

    ![](./media/image10.png)

4.  Enter the required **rank number !!1!!**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image11.png)

5.  Select the required **security role as Basic User** for the
    Experience Profile.

6.  Select **Save and Close**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image12.png)

## Exercise 2 - Create and Configure a Session Template

In this exercise, learners create a session template and configure the
elements that shape how customer sessions appear in the agent workspace.
They define the session properties, add an application tab, enable
script expression support, and associate the template with the existing
workstream. This exercise helps prepare a more organized and consistent
workspace experience for handling customer interactions.

### Task 1 - Create a New Session Template

1.  Open a new private window. Use the URL that we extracted from the
    Power Platform admin center and log in to the Contact Center
    environment by using Mark Brown's credentials. Mark Brown is
    assigned the System Administrator and Omnichannel Administrator
    roles.

    > Note: If you have any confusion about the login. Revisit Exercise 4 of Lab 0.

    ![](./media/image13.png)

2.  On the app selector, select **Copilot Service admin center.**

    ![](./media/image14.png)

3.  In the Copilot Service admin center, navigate to **Workspaces**
    under the **Support experience** group.

4.  On the **Workspaces** page, select **Manage** for **Session
    templates**.

    ![](./media/image15.png)

5.  On the **Active Session Templates** page, select **+ New**.

    ![](./media/image16.png)

6.  On the **New Session Templates** page, in the **General** tab,
    specify the following:

    - **Name** – !!Contoso Session!!

    - **Unique Name** – !!msdyn_chat_custom!!

    - **Type** – Entity

    - **Entity** – Case

    - **Title** – !!{CustomerName}!!

    - **Communication panel mode** – Hidden

    - **Apply session title to anchor tab** – Yes

7.  Select **Save**.

    ![](./media/image17.png)

### Task 2 - Add Application Tabs and Enable Agent Script Expression

1.  On the session template page, in the **Additional Tab** section,
    select **Add Existing Application Tab Template**.

    ![](./media/image18.png)

2.  In the **Lookup Records** pane, search for and select **Customer
    Summary**.

3.  Select **Add**.

    ![](./media/image19.png)

4.  Verify that the application tab is added to the session template.

    ![](./media/image20.png)

5.  Select the **Scripts** tab.

    ![](./media/image21.png)

6.  Set the **Enable build expression** toggle to **Yes**.

7.  Select **Save and Close**.

    ![](./media/image22.png)

### Task 3 - Configure the Session Template in Workstream

1.  In the Copilot Service admin center site map, select
    **Workstreams**.

2.  Open **Contoso Chat workstream**.

    ![](./media/image23.png)

3.  Scroll down and expand **Show advanced settings**.

    ![](./media/image24.png)

4.  Select **Edit** beside **Sessions**.

    ![](./media/image25.png)

5.  On the **Sessions** pane, select **Chat session - default** in the
    **Default template** field.

6.  Select **Save and Close**. If the button is disabled, select
    **Cancel**.

    ![](./media/image26.png)

7.  Select **Edit** beside **Customer service representative
    notifications**.

    ![](./media/image27.png)

8.  On the notifications pane, review or select the required templates
    based on your requirements.

9.  Select **Save and Close**.

    ![](./media/image28.png)

## Exercise 3 - Register an Application and Create an Application User

In this exercise, learners register an application in Microsoft Entra ID
and create a corresponding application user in Power Platform. These
steps establish the application identity required to support bot-based
integration in the Contact Center environment. This exercise provides
the setup foundation needed before the Smart Assist bot can be
associated with the workstream.

### Task 1 - Register an Application in Microsoft Entra ID

1.  Open a new browser tab and navigate to the Microsoft Entra admin
    center: !!<https://entra.microsoft.com/!!>.

2.  Sign in by using the Mark Brown credentials.

3.  Complete the authentication process if prompted.

    ![](./media/image29.png)

    ![](./media/image30.png)

4.  Under **Entra ID**, navigate to **App registrations**.

    ![](./media/image31.png)

5.  Select **+ New registration**.

    ![](./media/image32.png)

6.  Enter the application name as !!Contoso App!!.

7.  Select **Register**.

    ![](./media/image33.png)

8.  Verify that the **Contoso App** registration page opens
    successfully.

    ![](./media/image34.png)

### Task 2 - Create an Application User in Power Platform

1.  Open a new browser tab and navigate to the Power Platform admin
    center: !!<https://admin.powerplatform.com/!!>. Log in with Mark
    Brown credentials.

2.  Select **Manage** \> **Environments** from the left navigation pane.

3.  Open the **ContactCenter Trial** environment.

    ![](./media/image35.png)

4.  Select **Settings**.

    ![](./media/image36.png)

5.  Under **Users + permissions**, select **Application users**.

    ![](./media/image37.png)

6.  On the **Application users** page, select **New app user**.

    ![](./media/image38.png)

7.  In the **Create a new app user** dialog, select **Add an app**.

    ![](./media/image39.png)

8.  Search and select **Contoso App**, and then select **Add**.

    ![](./media/image40.png)

9.  In the **Business unit** field, enter !!Org!! and select the trial
    environment business unit.

10. In the **Security roles** field, select **Edit**.

    ![](./media/image41.png)

11. On the **Add security roles** page, select **Omnichannel agent**,
    and then select **Save**.

    ![](./media/image42.png)

12. Select **Create**.

    ![](./media/image43.png)

13. Navigate to **Copilot Service Admin Center** \> **User Management**.

14. Select **Manage** for **Users**.

    ![](./media/image44.png)

15. From the **Enabled Users** dropdown, select **Application Users**.

    ![](./media/image45.png)

16. Open **Contoso App**.

    ![](./media/image46.png)

17. From the dropdown below the app name, select **Application Users**.

    ![](./media/image47.png)

18. Set **User Type** to **Bot Application user**.

    ![](./media/image48.png)

19. Switch back to the Microsoft Entra admin center and copy the
    **Application (Client) ID** for the app created in the previous
    task.

20. In the **Bot application ID** field, enter the copied application
    ID.

21. Select **Save & Close**.
    
    ![](./media/image49.png)

## Exercise 4 - Add a Smart Assist Bot and Create an Agent Script

In this exercise, learners add the bot application user to the
workstream, create a script for chat sessions, and associate that script
with the session template. This exercise introduces the guided
assistance features that support agents during customer conversations by
combining bot-based help and structured script guidance within the
workspace.

### Task 1 - Add a Smart Assist Bot to a Workstream

1.  In the Copilot Service admin center, select **Workstreams** under
    **Customer support**.

2.  Open **Contoso Chat Workstream**.

    ![](./media/image50.png)

3.  Scroll down and expand **Show Advanced settings**.
    
    ![](./media/image51.png)

4.  In the **Smart Assist bots** area, select **Add bot**.

    ![](./media/image52.png)

5.  In the **Add from existing** pane, select the **Contoso App** bot
    user from the list.

6.  Select **Add**.

    ![](./media/image53.png)

    > **Note:** Multiple bots can be added to a workstream based on business requirements.

### Task 2 - Create an Agent Script for Chat Sessions

1.  In the Copilot Service admin center, select **Productivity** under
    **Support experience**.

2.  On the **Productivity** page, select **Manage** for **Scripts**.

    ![](./media/image54.png)

3.  On the **Scripts** page, select **+ New**.

    ![](./media/image55.png)

4.  On the **New Script** page, specify the following:

    - **Name** – !!Chat session script!!

    - **Unique Name** – !!Contoso_script!!

    - **Description** – !!This agent script is used for chat
      sessions.!!

5.  Select **Save**.

    ![](./media/image56.png)

6.  In the **Script steps** section, select **+ New Script step**.
    
    ![](./media/image57.png)

7.  On the **New Script step** form, specify the following:

    - **Name** – !!Greet the customer!!

    - **Unique Name** – !!Greet_script!!

    - **Order** – !!1!!

    - **Action type** – Text

    - **Text instructions** – !!Greet the customer with the welcome
      message!!

8.  Select **Save and Close**.

    ![](./media/image58.png)

9.  Select **Save & Close** to save the script.

    ![](./media/image59.png)

### Task 3 - Associate the Script with a Session Template

1.  In the Copilot Service admin center, select **Workspaces** under
    **Support experience**.

2.  Select **Manage** for **Session templates**.

    ![](./media/image60.png)

3.  Open the **Chat session - default** template.
    
    ![](./media/image61.png)

4.  Select the **Scripts** tab.

5.  In the **Scripts** section, select **Add Existing script**.

    ![](./media/image62.png)

6.  In the **Lookup Records** pane, search for and select **Chat session
    script**.

7.  Select **Add**.

    ![](./media/image63.png)

8.  Select **Save & Close**.

    ![](./media/image64.png)

## **Conclusion**

In this lab guide, learners configured the key workspace components that
support a guided and productivity-focused agent experience in Dynamics
365 Contact Center. They created an Experience Profile, enabled agent
productivity tools, defined a session template, registered an
application for bot integration, and added Smart Assist and script-based
guidance to the workstream. Together, these configurations help
establish a more structured, efficient, and agent-ready support
environment.
