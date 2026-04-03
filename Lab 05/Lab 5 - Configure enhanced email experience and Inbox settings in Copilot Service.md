## Lab 5 - Configure enhanced email experience and Inbox settings in Copilot Service admin center

**Duration: 30 mins**


**Introduction**

This lab guide focuses on enabling the enhanced email experience in
Power Apps and configuring Inbox settings in Copilot Service. In this
lab, **Mark Brown** performs all configuration tasks by using the
required administrative access. You will start a Power Apps free trial,
configure the email form order, enable the enhanced experience for email
attachments, review and enable Inbox settings in the **Contoso Agent**
Experience Profile, and create a new Inbox view. By completing this lab,
learners gain practical experience in improving the email handling and
Inbox experience for service representatives.

## Exercise 1 - Configure the enhanced email experience in Power Apps

In this exercise, you will start a Power Apps free trial, configure the
email form order, and enable the enhanced experience for email
attachments. These steps help prepare a more consistent and improved
email experience in the Contact Center environment.

### Task 1 - Enable Power Apps free trial

1.  Open a tab and paste the link of the Power Apps -
    !!<https://powerapps.microsoft.com/>!! and then click on **Try for
    free** to start free trial.

    ![](./media/image1.png)

2.  Enter the **Mark Brown** ID, select the signing up check box and
    then click on **Start free**.

    > **Note:** After clicking **Start trial**, if prompted, provide the required preliminary information to begin the trial, then continue with the process.

    ![](./media/image2.png)

3.  Select the **Contact Center Trial Environment** from the top right
    corner of the home page.

    ![](./media/image3.png)

### Task 2 - Configure the email form order

4.  In Power Apps, go to **Settings** \> **Advanced Settings**.

    ![](./media/image4.png)

5.  From the top menu, select **Customizations** \> **Customizations**.

6.  Select **Customize the System**.

    ![](./media/image5.png)

7.  Expand **Entities**.

    ![](./media/image6.png)

8.  Select and expand **Email** and then select **Forms**.

    ![](./media/image7.png)

9.  On the command bar, select **Form Order**, and then select **Main
    Form Set** from the drop-down list.

    ![](./media/image8.png)

10. The **Form Order** window appears, which displays the enabled email
    forms that are available. If **Enhanced email** doesn’t display at
    the top of the list, use the arrows to move it up so it displays
    first on the list, and then select **OK**.

    ![](./media/image9.png)

11. When you complete your updates, select **Publish All
    Customizations** in the top-left corner to display the changes.

    ![](./media/image10.png)

### Task 3 - Enable enhanced experience for email attachments

You can enable the enhanced email attachment control for forms to
provide a consistent email attachment experience to representative. Do
the following steps:

12. Navigate back to Power Apps homepage and from left menu click on the
    **Tables**.

13. In the Table windows, scroll down and select **Email** table.

    ![](./media/image11.png)

14. Select **Forms** under **Data experiences**.

    ![](./media/image12.png)

15. Click on the **Email** form.

    ![](./media/image13.png)

16. Select **Attachment** and the subgrid displays on the right hand
    side of the page.

17. Scroll down and expand **Components** select **+ Component**.

    ![](./media/image14.png)

18. Select **Get More Components**.

    ![](./media/image15.png)

19. Scroll down and select **Attachment control** then click on the
    **Add** button.

    ![](./media/image16.png)

20. From the top right corner click on the **Save and publish**.

    ![](./media/image17.png)

## Exercise 2 - Configure Inbox settings in Copilot Service

In this exercise, you will review and enable Inbox settings in the
**Contoso Agent** Experience Profile and then create a new Inbox view.
These steps help improve productivity by making email records easier to
organize and access in Copilot Service.

### Task 1 - Review and enable Inbox settings

In this task, you will navigate to the **Contoso Agent** Experience
Profile in the Copilot Service Admin Center and verify if the Inbox
feature is enabled. You will also explore available configuration
options for record types and visibility.

21. Log in to the Contact Center environment by using **Mark Brown**
    credentials and open the **Copilot Service admin center**.

    ![](./media/image18.png)

22. On the **Copilot Service admin center** app, under **Support
    experience**, select **Workspaces**.

23. In **Experience profiles** section, select **Manage**.

    ![](./media/image19.png)

24. Select the **Contoso Agent** profile.

    ![](./media/image20.png)

25. Scroll down and select **Edit** in **Inbox** section.

    ![](./media/image21.png)

26. On the **Inbox Settings** page, check if the **Enable Inbox** toggle
    is already enabled. If not, enable the toggle.

    ![](./media/image22.png)

27. Select a **Closed work items** view and select **Edit** to explore
    the existing view.

    ![](./media/image23.png)

28. For this lab guide we are not changing any configuration,
    Participants can explore below given options. Click on the **Save
    and Close** button.

    - **Name:** Specify a name that shows in the inbox. Alphanumeric values
    are valid names.

    - **Record Type:** Select the record types for which the settings need
    to be applied. You can select more than one record type.

    - **Agent Visibility:** Select one of the following options to show or
    hide the view of agents:

    - **Show**

    - **Hide**

    ![](./media/image24.png)

### Task 2 - Create a Multiple View in Inbox

In this task, you will create a new Inbox view called **“Multiple
View”** to help agents organize their incoming and assigned emails
efficiently. This setup enhances productivity by segmenting email
records into logical views.

29. Select **+ Add**. **Add a new view** page is displayed.

    ![](./media/image25.png)

30. On the **Add a new view** page, enter the following details:

    - **Name:** !!Multiple View!!

    - **Agent visibility:** Select **Show**

    - **Record type:** Select **Email**

33. For each record type, choose one of the following settings. The
    settings are different for each record type. Select **Simple** and
    select:

    - **Emails sent to me**

    - **Emails Assigned to me**

34. Select **Save and close**.

    ![](./media/image26.png)

35. Select **Save and close** again.

    ![](./media/image27.png)

## Conclusion

In this lab guide, you enabled the Power Apps free trial, configured the
email form order, enabled the enhanced experience for email attachments,
reviewed and enabled Inbox settings, and created a new Inbox view in the
**Contoso Agent** Experience Profile. Together, these steps help improve
the email handling and Inbox experience for service representatives by
providing a more consistent, organized, and productivity-focused
workspace.
