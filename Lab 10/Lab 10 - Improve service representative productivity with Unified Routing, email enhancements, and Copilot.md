# Lab 10 - Improve service representative productivity with Unified Routing, email enhancements, and Copilot

**Duration: 120**


**Introduction**  
This lab guide focuses on improving the day-to-day productivity of
service representatives in Dynamics 365 Contact Center. Learners work in
Copilot Service workspace to manage inbox items, cases, queues,
activities, and parent-child case relationships, while also using
Copilot-assisted email drafting and enabling the new insert template
dialog in Power Apps. By completing these exercises, learners gain
practical experience in handling customer work more efficiently through
workspace productivity features, routing actions, email enhancements,
and AI-assisted support tools.

## Exercise 1 - Work with the inbox, cases, timeline, and presence

In this exercise, learners work in Copilot Service workspace to manage
the inbox, create and update cases, add timeline activities, and review
presence options. This exercise introduces the core workspace tools that
help service representatives organize work, manage customer records, and
maintain visibility into their availability.

### Task 1 - Navigate and manage the inbox

1.  Log in to the Contact Center environment by using **David Flores**
    credentials. David Flores is assigned the required Customer Service
    Representative and Omnichannel agent role to perform workspace-based
    case and queue tasks.

2.  From the top app option select **Copilot Service workspace**.

    ![](./media/image1.png)

3.  Select **Inbox** from the left navigation bar.

    ![](./media/image2.png)

4.  In the inbox, select the **Filter** icon.

5.  Select the required filter views. The following options are
    available:

    **Filter**

        - All - Displays both read and unread items.

        - Unread - Displays only unopened items.

        - Read - Displays only opened items.

    **Sort by**

        - Customer - Displays items based on the customer record.

        - Date - Displays items based on the date they were created.

    **Sort order**

        - Oldest on top - Displays old items first in the inbox.

        - Latest on top - Displays most recent items first in the inbox.

        ![](./media/image3.png)

### Task 2 - Create and edit a case

1.  On the Copilot Service workspace navigation page there are two
    options available, **Account** and **Contact**. Participants can
    create cases with both options. For this lab guide we are creating
    cases with **Contact**. In Copilot Service workspace, select
    **Contacts**.

    ![](./media/image4.png)

2.  Select the contact, then Select **All Contacts** option and click on
    **Claudia Mazzanti**.

    ![](./media/image5.png)

3.  Click the down arrow next to **Related** and then select **Cases**.

    ![](./media/image6.png)

4.  Click **+ New Case** and fill in the following details:

    - Case title: !!**A Mineral Build Up in Water Supply!!**

    - Subject: **Water Supply**

    - Priority: **Normal**

    - Case type: **Problem**

    - Case status: **In Progress**

5.  Click **Save and Close**.

    ![](./media/image7.png)

    ![](./media/image8.png)

6.  Open the created case.

    ![](./media/image9.png)

7.  Scroll down and select the **Product** field.

8.  Choose **Smart Brew 300**.

9.  Click **Save**.

    ![](./media/image10.png)

    ![](./media/image11.png)

### Task 3 - Add activities to timeline

1.  Scroll down and navigate to the **Timelines** section of the case.

    ![](./media/image12.png)

2.  Click on the **+** icon to add activity in the timeline.

    ![](./media/image13.png)

3.  Filter and view important notes, posts, and activities using
    multiple filter options.

    ![](./media/image14.png)

4. Click on the **Save and Close.**
    
    ![](./media/image15.png)

### Task 4 - Manage presence status

1.  In Copilot Service workspace you can view your presence status on
    the navigation bar.

    ![](./media/image16.png)

2.  Select the status icon.

3.  Select the appropriate status from the available list:

    - Available

    - Appear away

    - Busy

    - Don’t disturb

    - Offline

    ![](./media/image17.png)

## Exercise 2 - Work with queues and activities

This exercise focuses on queue and activity management in Copilot
Service workspace. Learners pick and release queue items, route work to
another queue, create and assign task activities, add records to queues,
and use routing rules to direct cases. These tasks help build an
understanding of how Unified Routing and queue-based work handling
support operational efficiency.

### Task 1 - Pick items from queue

1.  Continue in Copilot Service workspace by using **David Flores**
    credentials.

2.  In the Copilot Service workspace, select the **Site Map** and then
    select **Queues**.

    ![](./media/image18.png)

3.  From the dropdown for **Items, I am working on**, select **All
    items**.

    ![A screenshot of a search box Description automatically generated](./media/image19.png)

4.  Next, from the dropdown for **Queues I’m member of**, select **All
    Queues**.

    ![A screenshot of a computer Description automatically generated](./media/image20.png)

5.  Select the checkbox next to the required item, and then select
    **Pick** from the command menu.

    ![](./media/image21.png)

6.  The **Pick** dialog appears. For the **Also remove the item(s) from
    the Queue** dropdown, if you select **Yes**, the item is removed
    from the queue. For this scenario, select **No**.

7.  Select **Pick**.

    ![A screenshot of a computer Description automatically generated](./media/image22.png)

8.  If the item is in an advanced queue and is tracked through unified
    routing, the following action occurs:

    - The **Worked By** attribute of the queue item will be updated with
      your user ID. The unified routing system takes this as an
      indicator of work assignment.

    ![](./media/image23.png)

9.  To manually add another user or team, select the item.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image24.png)

10. Click on the **Vertical Ellipsis** icon and select **Queue Item
    details** from the command menu.

    ![](./media/image25.png)

11. Select the lookup for the **Worked By** field and then select the
    user. If the queue item is assigned to a private queue, the lookup
    displays only the members of that queue.

    ![](./media/image26.png)

    > **Note:** Remove the items from the queue can’t be set for work items in an advanced queue. Advanced queues are used in unified routing to which work items are routed through workstreams.

12. Click **Save and Close** from the top bar.

    ![](./media/image27.png)

### Task 2 - Release items from queue

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Queues**.

    ![A screenshot of a computer Description automatically generated](./media/image28.png)

2.  From the dropdown for **Items, I am working on**, select **All
    items**.

    ![A screenshot of a search box Description automatically generated](./media/image19.png)

3.  Next, from the dropdown for **Queues I’m member of**, select **All
    Queues**.

    ![A screenshot of a computer Description automatically generated](./media/image20.png)

4.  Select the item that you want to release, and on the command bar
    select **Release**.

    ![](./media/image29.png)

5.  On the **Release Queue Item** dialog box, select **Release**.

    ![A screenshot of a computer Description automatically generated](./media/image30.png)

6.  When you release an item, your name is removed from the **Worked
    By** field, and the item is no longer assigned to you; it’s assigned
    to the queue owner.

    ![](./media/image31.png)

### Task 3 - Route items to another queue

1.  Select the case that you want to move to another queue, and then
    select **Route**.

    ![](./media/image32.png)

2.  On the **Route Queued Item** dialog box, select **Queue** for the
    **Route to** field.

3.  Select **Contoso queue for supervisors**.

4.  Select **Route**.

    ![A screenshot of a computer screen Description automatically generated](./media/image33.png)

5.  The queue is routed to **Contoso queue for supervisors**.

### Task 4 - Create task activity

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Activities**.

    ![A screenshot of a computer Description automatically generated](./media/image34.png)

2.  Click on **Task** to create task activity.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image35.png)

3.  Enter the following details in the field and then click **Save and
    Close**:

    - Subject - !!Setup Warranty Account!!

    - Regarding – **A mineral build Up in Water Supply**

    - Duration - **30 minutes**

    ![](./media/image36.png)

### Task 5 - Assign activity

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Activities**.

    ![A screenshot of a computer Description automatically generated](./media/image34.png)

2.  Select the activity you want, and on the command bar click on the
    **ellipsis** icon from the top and select **Assign**.

**Note:** If activity is not visible in **My activity**, convert **My
activity** to **All activity**.

![](./media/image37.png)

3.  In the **Assign To** field select **User or team / Me**. For this
    scenario, select **Me** as assign to and then click on the
    **Assign** button.

    ![A screenshot of a computer screen AI-generated content may be
    incorrect.](./media/image38.png)

### Task 6 - Add activity to queue

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Activities**.

2.  Select the activity you want.

3.  From the top, click on the **Vertical ellipsis** icon and then
    select **Add to Queue**.

    > **Note:** If the **Add to Queue** button is not seen on the ribbon, select the **Vertical ellipses** and then select **Add to Queue**.

> ![](./media/image39.png)

4.  The **Queue** field displays the queue the activity belongs to. The
    queue lookup displays only the queues that the activity can be added
    to.

5.  Select the **Default entity queue** and then select **Add**.

    ![A screenshot of a computer Description automatically
    generated](./media/image40.png)

### Task 7 - Add case to queue

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Contact**.

    ![A screenshot of a computer AI-generated content may be
    incorrect.](./media/image41.png)

2.  Navigate to **All Contacts** and select the **Claudia Mazzanti**
    contact.

    ![](./media/image42.png)

3.  In the list of cases, select the case that you want to add to a
    queue.

4.  On the Related Cases section, Select **Case** and click on the
    **Vertical Ellipsis** and select **Add to Queue**.

    ![A screenshot of a computer AI-generated content may be
    incorrect.](./media/image43.png)

5.  In the **Queue** field, select **Default entity queue**, and then
    select **Add**.

    ![A screenshot of a computer Description automatically
    generated](./media/image44.png)

    > If a case is already added to a queue, the **Queue** field displays the current queue by default.

    > The lookup for the **Queue** field displays only the queues that are configured for a specific entity. Voice and messaging queues aren’t displayed in the lookup results since cases can’t be added to those queues.

### Task 8 - Route case using rule set

1.  From the list of cases, open a case record.

    > ![A screenshot of a web page AI-generated content may be incorrect.](./media/image45.png)

2.  Make any changes, and on the command bar, select **Save & Route**.

    > ![](./media/image46.png)

3.  In the **Route Case** dialog, select **Route**.

    > ![A screenshot of a computer Description automatically generated](./media/image47.png)

    The case will be routed based on the active routing rule set.

## Exercise 3 - Manage parent-child cases and Smart Assist

In this exercise, learners manage related customer cases and explore
Smart Assist capabilities. They review customer cases, create parent and
child cases, associate cases manually, and convert a case into a
knowledge article. This exercise shows how service representatives can
organize related issues more effectively and connect case resolution
work to knowledge creation.

### Task 1 - View and create cases for a customer

1.  In the Copilot Service workspace, select the **Site Map** and then
    select **Contacts**.

    ![](./media/image48.png)

2.  Select all contacts and then click on the **Claudia Mazzanti**
    contact to see the summary.

    ![](./media/image49.png)

3.  On the Claudia contact page, click on the **Related** option and
    then select **Cases** to see all cases related to contact.

    ![](./media/image50.png)

4.  If you select a case record from the case view, you see these
    additional options on the command bar:

    - Save & Route

    - Resolve Case

    - Cancel Case

    - Assign

    - Add to Queue

    - Queue Item Details

    ![](./media/image51.png)

5.  Select **New Case** to create.

    ![](./media/image52.png)

6.  Enter the following information on the **Basic Detail** tab and then
    select **Save and Close**:

    - Case Title – !!Minerals level is not maintained!!

    - Customer – !!Claudia Mazzanti!!

    - Subject – !!Water supply!!

    - Case Type - Problem

    - Priority – Normal

    - Case Status - In Progress

    ![](./media/image53.png)

7.  Click on the newly created case.

    ![](./media/image54.png)

8.  Select **Product** field and select **Water Filtration System** and
    then click on the **Save** button from top.

    ![](./media/image55.png)

### Task 2 - Create a child case

1.  On the command bar, select the **three dots** and then select
    **Create Child Case**.

    ![](./media/image56.png)

2.  On the **Quick Create: Case** pane that appears on the right side,
    enter the following information and then select **Save and Close**:

    - Case Type – !!Request!!

    - Customer – !!Claudia Mazzanti!!

    - Case Title – !!Share a quotation for replacement!!

    ![](./media/image57.png)

3.  On **Minerals level is not maintained** case select **Details** tab
    from the command bar and then scroll down.

![](./media/image58.png)

4.  You will view the child case on the **Child Cases** tile.

    ![](./media/image59.png)

5.  Select **Save & Close** from top command bar.

    ![](./media/image60.png)

### Task 3 - Associate parent and child cases manually

1.  On **Claudia Mazzanti** contact, select two or more cases that you
    want to associate as parent and child cases.

2.  On the command bar, select **Associate Child Cases**.

    ![](./media/image61.png)

3.  The **Set Parent Child Relationship** dialog appears.

4.  In the list, select the case that you want to set as parent, and
    then select **Set**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image62.png)

5.  Select **OK**.

    ![A white background with black text Description automatically generated](./media/image63.png)

6.  Select the case that was selected as a Parent case by you.

    ![](./media/image64.png)

7.  Select **Details** tab from the command bar and then scroll down.

8.  You will view the Child case on the **Child Cases** tile.

    ![](./media/image65.png)

### Task 4 - Convert case to knowledge article

1.  On the command bar, select the **ellipsis** icon and go to **Convert
    To** \> **To Knowledge Article**.

    ![](./media/image66.png)

    ![](./media/image67.png)

2.  On **Convert to knowledge article** page, keep the default values
    and then select **Convert**.

    ![](./media/image68.png)

3.  The knowledge article is created.

## Exercise 4 - Resolve, cancel, assign, and merge cases

This exercise focuses on common case management actions used during
support operations. Learners resolve, cancel, reassign, create, and
merge cases while reviewing how these actions affect related activities
and case relationships. This helps demonstrate how case lifecycle
management supports more accurate tracking and streamlined service
delivery.

### Task 1 - Resolve a case

1.  Continue in Copilot Service workspace by using **David Flores**
    credentials.

2.  In the Copilot Service workspace, select the **Site Map** and then
    select **Contact** and then click on **Claudia Mazanti**.

    ![](./media/image69.png)

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image70.png)

3.  Scroll down and click on the **A Mineral Build Up in Water Supply**
    case.

    ![](./media/image71.png)

4.  On the command bar, select **Resolve case**.

    ![](./media/image72.png)

5.  If you have open activities linked to the case, you see a message
    with the following actions:

    - A link with the number of open activities. You can select the link
      to view the open activities associated with the case on a tab your
      administrator has configured.

    ![A screenshot of a computer Description automatically generated](./media/image73.png)

    - **Confirm**: If you select **Confirm** on the warning, the system
       automatically cancels the open activities when the case is resolved.

    ![A blue square with black text Description automatically generated](./media/image74.png)

6.  Select **Confirm**.

7.  On the **Resolve Case** dialog box, enter the !!Demo resolution!!
    and then select **Resolve**.

    ![](./media/image75.png)

8.  Click on **Reactivate Case** to execute further steps of lab guide.

    ![](./media/image76.png)

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image77.png)

### Task 2 - Cancel a case

1.  On the Case window click on **Cancel Case** to cancel the case. If
    the option is not visible click on the **ellipsis** icon and select
    **Cancel Case**.

    ![](./media/image78.png)

2.  In the **Confirm Cancellation** dialog box, select the case status:

    - **Canceled**: The case is canceled and is no longer assigned to
      you.

    - **Merged**: The case is merged with another case. When the case is
      merged, the case activities are moved to the case it was merged
      with.

    ![A screenshot of a computer Description automatically generated](./media/image79.png)

3.  Select **Cancelled** and then Select **Confirm**.

    ![A screenshot of a computer error Description automatically generated](./media/image80.png)

    > **Note:** Reactivate case for the further execution.

### Task 3 - Reassign a case

1.  Click on the **Vertical Ellipsis** and select **Assign** to reassign
    the case.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image81.png)

2.  In the **Assign to Team or User** dialog box, in the **Assign To**
    field, there are two options: **Me** / **User or Team**. For this
    lab guide click on **Me** and select **Assign**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image82.png)

### Task 4 - Create and merge cases

1.  Navigate back to **Claudia Mazzanti** window, scroll down and select
    **+ New Case**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image83.png)

2.  Enter the given details in the field and then click on **Save and
    Close** to create a new case:

    - Case title – **Mineral Contain is not Fitting**

    - Subject – **Water Supply**

    - Case Type – **Problem**

    - Status – **In Progress**

    ![](./media/image84.png)

3.  Select at least two active case records that you want to merge.

4.  Select **Merge Cases** from the command menu. If option is not
    visible click on the **vertical ellipsis** icon and select **Merge
    Case** option.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image85.png)

5.  In the **Merge Cases** dialog box, from the list of cases, select
    the case the other cases will be merged into, and then select
    **Merge**.

6.  Select **OK**.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image86.png)

7.  To see the merged case, open the case it was merged into.

8.  Select the **Details** tab, scroll down and you’ll find the merged
    case listed in the **Merged Cases** section.

    ![A screenshot of a computer AI-generated content may be incorrect.](./media/image87.png)

## Exercise 5 - Enable the new insert template dialog in Power Apps

In this exercise, learners switch to Power Apps to enable the new insert
template dialog through a solution setting. They review how the feature
can be configured at the environment level and optionally controlled for
specific model-driven apps. This exercise introduces a configuration
step that supports an improved email template selection experience.

### Task 1 - Enable the New Insert Template Dialog in a solution

1.  Open a new tab in the browser, navigate to the Power Apps -
    !!https://make.preview.powerapps.com/!!,

2.  Log in to Power Apps by using **Mark Brown's** credentials. Mark
    Brown is assigned the required **System Administrator** role to
    perform solution and customization tasks.

3.  Select the **ContactCenter Trial** environment.

    ![](./media/image88.png)

4.  Select **Solutions** on the left navigation pane.

    ![A screenshot of a computer Description automatically generated](./media/image89.png)

5.  Click on **New Solution** from top command bar.

    ![](./media/image90.png)

6.  Enter the below details:

    - Display Name of the solution – **Test**

    - Publisher – **Default publisher for your organization**

    - Select **Set as preferred solution** check box

7.  Select **Create**.

    ![](./media/image91.png)

8.  Select **Add Existing** \> **More** \> **Setting**.

    ![](./media/image92.png)

9.  On the **Add existing Setting Definition** pane, search and select
    **Enable the New Insert Template Dialog** option and then select
    **Next**.

    ![](./media/image93.png)

10. Select **Add** on the **Selected Setting Definition**.

    ![](./media/image94.png)

11. The **Enable the New Insert Template Dialog** option is added to
    your solution. Select **Enable the New Insert Template Dialog** and
    click **Edit**.

    ![](./media/image95.png)

12. Set the **Setting environment value** option to **Yes** on the
    **Edit Enable the New Insert Template Dialog** pane.

13. Select **Save**.

    ![](./media/image96.png)

    ![](./media/image97.png)

14. Unselect and select **Publish All Customizations**.

    ![](./media/image98.png)

    ![A screenshot of a computer Description automatically generated](./media/image99.png)

### Task 2 - Configure for specific model-driven apps

1.  Go to **Add Existing** \> **App** \> **Model-driven app**.

    ![](./media/image100.png)

2.  On the **Add existing model-driven apps** pane, select the app for
    which you want to disable the enhanced insert email template
    selection dialog. The app is added to the solution. For this lab, we
    are not selecting any app. Hence select **Cancel**.

    ![A screenshot of a computer Description automatically
    generated](./media/image101.png)

**Note**

    - Select the **Enable the New Insert Template Dialog** option in the
    solution.

    - On the **Edit Enable the New Insert Template Dialog**, in the
    **Setting app value** section, the selected app is displayed.

    - Select **New app value** for the app, and select **No** for the
    specified app.

    - Select **Save** and **Publish All Customizations**.

## Exercise 6 - Draft an email with Copilot

This exercise introduces Copilot-assisted email drafting in Copilot
Service workspace. Learners open a case, start a new email activity,
review the predefined Copilot prompts, and use a generated response in
the email draft. This exercise demonstrates how Copilot can help service
representatives respond faster and more effectively to customer issues.

1.  Log in to the Contact Center environment by using **David Flores**
    credentials.

2.  Open a case from the Copilot Service workspace.

    ![](./media/image102.png)

3.  Select the **Write an email** tab on the Copilot pane.

    ![](./media/image103.png)

4.  On the case overview page, select **Related** tab and then select
    **Activities**.

    ![](./media/image104.png)

5.  Select **+ New Activity** \> **Email**.

    ![](./media/image105.png)

6.  When you start to draft an email, Copilot opens in the right-side
    panel and presents five predefined prompts and one custom prompt:

    - **Suggest a call**: Drafts a reply that suggests a call with the
      customer today or tomorrow.

    - **Request more information**: Drafts a reply that requests more
      details from the customer to help resolve the problem.

    - **Empathize with feedback**: Drafts a reply that provides an
      empathetic response to a customer who expresses a complaint.

    - **Provide product/service details**: Drafts a reply that offers
      details or answers customer questions about a particular product
      or service.

    - **Resolve the customer’s problem**: Drafts a reply that provides a
      resolution—and resolution steps, if applicable—to the customer’s
      problem.

    - **Custom**: Allows you to provide your own prompt for the reply.

    ![](./media/image106.png)

    ![](./media/image107.png)

7.  Select **Empathize with feedback** from the predefined prompts list.

    ![](./media/image108.png)

8.  You can see Copilot has generated suggestion.

    ![](./media/image109.png)

9.  You can now review the response. Make any necessary changes, and
    then select **Copy to email** to copy the entire response to your
    draft. Or select part of the response and use the right-click menu
    to copy and paste the selection.

    ![](./media/image110.png)

10. Response is now available in body part on left side.

    ![](./media/image111.png)

11. Now you can send the email or save it. For this lab click on the
    **Save and Close** button from top.

    ![](./media/image112.png)

## Conclusion

By completing this lab, learners gain practical experience using
workspace productivity features, queue and routing actions, case
management capabilities, email enhancements, and Copilot-assisted
drafting in Dynamics 365 Contact Center. Together, these tasks help
create a more efficient and connected service experience for
representatives handling customer interactions.
