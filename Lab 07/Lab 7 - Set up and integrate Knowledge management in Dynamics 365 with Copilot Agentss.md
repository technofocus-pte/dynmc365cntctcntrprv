# Lab 7 - Set up and integrate Knowledge management with Copilot Agents

**Introduction**

This lab guide focuses on configuring Knowledge Management in Dynamics
365 and extending that experience through Copilot Agents. In this lab,
**Mark Brown** performs all configuration tasks by using the **System
Administrator** and **Omnichannel Administrator** roles. You will enable
Knowledge management for additional record types, configure general
knowledge settings, create a knowledge category, manage search filters,
configure portal settings, create the required Power Apps connections,
and integrate a Copilot Agent with a knowledge article flow. By
completing this lab, learners gain practical experience in building a
knowledge-driven support experience that improves information access and
guided assistance in the Contact Center environment.

## Exercise 1 - Configure Knowledge management settings

In this exercise, you will configure the core Knowledge management
settings in the Copilot Service admin center. You will enable knowledge
management for an additional record type, configure general settings,
create a category, manage search filters, and review portal-related
settings. These steps establish the administrative foundation required
to organize, search, and surface knowledge articles effectively.

### Task 1 - Enable Knowledge Management for record types

In this task, you will enable knowledge management for additional record
types, such as **Account**, and configure automatic search behavior.

1.  Open a new private window. Use the URL that we extracted from the
    Power Platform admin center and log in to the Contact Center
    environment by using Mark Brown's credentials. Mark Brown is
    assigned the System Administrator and Omnichannel Administrator
    roles.

    > Note: If you have any confusion about the login. Revisit Exercise 4 of Lab 0.

    ![](./media/image1.png)

2.  Click on **App selector** to display the list of apps.

3.  Select the **Copilot Service Admin center** from the list of Apps.

    ![A screenshot of a computer Description automatically generated](./media/image2.png)

4.  Select **Knowledge** in **Support experience**. The **Knowledge**
    page appears.

5.  In the **Record types** section, select **Manage**.

    ![](./media/image3.png)

6.  On the **Record Types** page, review the available record types that
    can be configured for knowledge management.

7.  By default, knowledge management is enabled for **Case** and
    **Conversation** record types.

    ![](./media/image4.png)

8.  On the **Record Types** page, select **Add**.

    ![](./media/image5.png)

9.  The **Add record type** dialog appears.

10. On the **Add record type** dialog, from the **Select record type**
    dropdown list, select the record type – **Account**.

11. Set the toggle for **Turn on autometic search**.

12. Select **Account Name** to **Provide search results using field**.

13. Select **Save and Close**.

    ![](./media/image6.png)

### Task 2 - Configure Knowledge general settings

In this task, you will configure the general settings for knowledge
search, authoring, and global display options.

1.  Select **Knowledge** again on the left navigation pane.

2.  In the **General Settings** section, select **Manage**. The
    **General Settings** page appears.

    ![](./media/image7.png)

3.  In the **Search results display count** section:

    - Select the display count from the dropdown. – **10**

    - In the **Feedback** section, set the **Enable feedback** toggle to
      **Yes**

    ![](./media/image8.png)

4.  In the **Authoring language** section:

    - Set the **Enable default authoring language for your users** to
      **Yes**

    - Select the **Organization’s UI language** option

    - Set the **Allow users to set default knowledge authoring
      language** toggle to **Yes**

    ![](./media/image9.png)

5.  In the **Knowledge search experience** section, enable the following
    as required:

    - **Enable suggest as you type** - **Yes**

    - **Set search mode as all** - **Yes**

    - **Show recently accessed knowledge articles** - **Yes**

    ![](./media/image10.png)

6.  In the **Global search knowledge configuration** section, switch the
    **Enable Kb preview mode from global search option** toggle to
    **Yes**.

    ![](./media/image11.png)

7.  Scroll up towards the top of the page and select **Save**.

    ![](./media/image12.png)

### Task 3 - Create a Knowledge category

In this task, you will create a new category to organize knowledge
articles logically. Categories help structure knowledge for easy access
and retrieval.

1.  Go back and select **Knowledge**.

2.  In the **Categories** section, select **Manage**.

    ![](./media/image13.png)

3.  The **Categories System Views** page appears. You can create and
    manage a logical structure of categories for your records.

4.  On the command bar, select **New** to create a new category record.

    ![](./media/image14.png)

5.  Enter the required information in the **General** section:

    - **Title:** !!Contoso Demo Category!!

    - **Description:** !!Contoso Demo Category!!

    - **Display Order:** !!1!!

6.  Select **Save & Close**.

    ![](./media/image15.png)

### Task 4 - Manage search filters

In this task, you will enable and configure search filters to allow
agents to refine their search experience in the knowledge base.

1.  Go back and select **Knowledge**.

2.  In the **Filters** section, select **Manage**.

    ![](./media/image16.png)

3.  Make sure that the **Enable search filters** toggle is set to
    **Yes**.

4.  Set the **Allow agent to personalize** toggle to **Yes**. This
    allows the service representatives to save the search filters
    relevant to their areas.

5.  Select **Save**.

    ![](./media/image17.png)

### Task 5 - Configure Knowledge portal settings

In this task, you will review and configure portal settings for
publishing knowledge articles to an external portal. You will also
define how attachments are synchronized to the portal.

1.  Go back and select **Knowledge**.

2.  In the **Portal** section, select **Manage**. The **Portals** page
    appears.

    ![](./media/image18.png)

3.  In the **Support portal connection** section, review the options
    available.

4.  Set the **Use an external portal** toggle to **Yes** to integrate an
    external portal to publish knowledge articles. For this lab, toggle
    to **No**.

5.  In **URL Format**, type the portal URL to use to create external
    (public-facing) portal links for knowledge articles, which the
    service representatives can share with the customers.

6.  The external URL is created in the following format: https://support
    portal URL/kb/{kbnum}.

7.  The placeholder, **{kbnum}**, is replaced by an actual knowledge
    article number.

8.  Enter Demo URL: !!http://webserver.contoso.com/kb/%7Bkbnum%7D!!

9.  In the **Sync knowledge article attachments to portal** section, set
    the **Sync attachments to the portal** toggle to **Yes**.

10. Select **Save**.

    ![](./media/image19.png)

## Exercise 2 - Create and integrate a Copilot Agent

In this exercise, you will configure the required connections in Power
Apps, create a Copilot Agent in Copilot Studio, create a topic, and
integrate the Search Dynamics 365 Knowledge Article flow into the topic.
These steps demonstrate how knowledge content can be surfaced through a
Copilot-driven experience.

### Task 1 - Configure connections in Power Apps

In this task, you will create and configure connections in Power Apps
for **Microsoft Dataverse** and **Content Conversion**, then link them
to your flows.

1.  Open a new tab and navigate to Power Apps portal
    !!https://make.powerapps.com/!!.

2.  Sign in with the **Mark Brown** credentials.

3.  Select the **ContactCenter Trial** environment on the top right
    corner of the home page.

    ![](./media/image20.png)

4.  Select **More** from the left navigation and then select
    **Connections**.

    ![](./media/image21.png)

5.  From top command bar select **+ New connection**.

    ![](./media/image22.png)

6.  Search for **Dataverse** and then select **Microsoft Dataverse**.

    ![](./media/image23.png)

7.  Select **Create**. Sign in with your credentials if prompted.

    ![](./media/image24.png)

8.  Again from top command bar select **New connection**.

    ![](./media/image25.png)

9.  Search and select **Content Conversion**.

    ![](./media/image26.png)

10. Select **Create**. Sign in with your credentials if prompted.

    ![](./media/image27.png)

11. From the left navigation of the Power Apps portal, select
    **Solutions** and then select **Default Solution**.

    ![](./media/image28.png)

12. From the left navigation, select **Connection references** and then
    select **Microsoft Dataverse**.

13. Click on the **Edit** from the top bar.

    ![](./media/image29.png)

14. In the edit box that opens, select the connection that you created
    from the **Connection** dropdown menu.

15. Select **Save** and then **Save changes**.

    ![](./media/image30.png)

    ![](./media/image31.png)

16. Similarly, select **Content Conversion** and then click on the
    **Edit** button.

    ![](./media/image32.png)

17. In the edit box that opens, select the connection that you created
    from the **Connection** dropdown menu. Click on the **Save** button.

    ![](./media/image33.png)

18. Select **Save changes**.

    ![](./media/image34.png)

19. Go back to **Default Solution** \> **Cloud flows** and turn on
    **Search Dynamics 365 knowledge article flow** .

    ![](./media/image35.png)

### Task 2 - Create a Copilot Agent

In this task, you will create a Copilot Agent in Copilot Studio and
configure it to use the **Search Dynamics 365 Knowledge Article** flow.

1.  Open a tab in the browser and go to the Copilot Studio home page -
    !!https://copilotstudio.microsoft.com/!!.
    Click on the **Try Free.**

    ![](./media/image36.png)

2.  Enter the Mark Brown credentials in the field and click on the
    **Next** button **and Sign in.**

    ![](./media/image37.png)

    ![](./media/image38.png)

3.  Enter the required details in the field and click on **Get
    Started.**

    ![](./media/image39.png)

4.  Accept the free trial.

5.  Select **United States** for country/region.

6.  Select the environment as **ContactCenter Trial** on top right
    corner of the homepage.

    ![](./media/image40.png)

    > **Note:** If you are unable to sign in to Copilot Studio or cannot switch the environment, open **Power Platform admin center** and sign in with **Mark Brown’s credentials**. Go to the **ContactCenter Trial** environment and copy the **Environment ID**.

    ![](./media/image41.png)

    ![](./media/image42.png)

    > Then return to the Copilot Studio page and update the URL by replacing the default environment ID with the copied **Environment ID**.

    ![](./media/image43.png)

    ![](./media/image44.png)

7.  Click on **Agent** from the left menu and then select **+ Create
    blank agent**.

    ![](./media/image45.png)

8.  Wait for a few seconds. Your agent is created successfully.

    ![](./media/image46.png)

### Task 3 - Create a topic in the Copilot Agent

In this task, you will create a topic named **Store hours** to handle
user queries about store timings.

1.  For better visibility, close the **Test your agent** panel for now.

2.  On the top menu bar, select **Topics**.

    ![](./media/image47.png)

3.  Select **Add a topic** and select **From blank**.

    ![](./media/image48.png)

4.  In the top left corner, enter the name of the topic as !!Store
    hours!!

    ![](./media/image49.png)

5.  In the describe field of trigger node, enter !!Store hours, what
    time do you open?, Are you open on Sunday!! in the field.

6.  Select **Save** from top right corner.

    ![](./media/image50.png)

### Task 4 - Add the Knowledge Article flow to the topic

In this task, you will integrate the **Search Dynamics 365 Knowledge
Article** flow to the topic and configure the input and output
variables.

1.  Select **Add node (+)** and select **Add a tool**.

2.  Select **Search Dynamics 365 knowledge article flow** action.

    ![](./media/image51.png)

3.  Provide the input to the flow. An error might appear if the filter
    isn’t provided to the flow.

4.  Click on the **Search Text Input** option on the action note,
    navigate to **system** and select **Activity.Name Variable**.

    ![](./media/image52.png)

5.  Repeat the same process on **Filter Input** and select
    **Activity.Recipient.ID** variable.

    ![](./media/image53.png)

6.  Under **Action** node click on the **(+)** and then select **Send a
    message** node.

    ![](./media/image54.png)

7.  On the **Message** node click on the **{X} add variable** button and
    in **custom variable** select **textResult** variable.

    ![](./media/image55.png)

8.  From top right corner click on the **Save** button to save the
    topic.

    ![](./media/image56.png)

    > **Tip:** If your search doesn’t return any results, modify the search terms or filter conditions. You can also add a filter condition if required.

## Conclusion

In this lab guide, you configured Knowledge management in Dynamics 365
and extended it with a Copilot Agent experience. You enabled Knowledge
management for the **Account** record type, configured general settings,
created a category, enabled filter personalization, reviewed portal
settings, created the required Power Apps connections, activated the
knowledge article flow, and integrated that flow into a Copilot Agent
topic. Together, these configurations help establish a more
knowledge-driven and AI-assisted support experience in the Contact
Center environment.
