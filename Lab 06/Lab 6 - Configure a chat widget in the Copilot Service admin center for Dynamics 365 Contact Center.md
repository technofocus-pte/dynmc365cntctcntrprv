# Lab 6 - Configure a chat widget in Copilot Service admin center 

**Introduction**

This lab guide focuses on creating and configuring a chat widget in the
Copilot Service admin center. In this lab, Mark Brown performs the
required configuration tasks to create a chat channel, connect it to an
existing workstream, customize the widget appearance, and configure
automated and survey messages. By completing this lab, learners gain
practical experience in setting up a web-based chat experience that
supports real-time customer engagement in Dynamics 365 Contact Center.

## Exercise 1 - Configure a chat widget

In this exercise, you will create a new chat channel in the Copilot
Service admin center and configure the chat widget settings. You will
associate the channel with an existing workstream, apply a theme, enable
proactive chat, add an automated message, and configure a
pre-conversation survey. This exercise demonstrates how to prepare a
customer-facing chat experience for real-time support.

1.  Log in to the Contact Center environment by using **Mark Brown**
    credentials. Mark Brown is assigned the **System Administrator** and
    **Omnichannel Administrator** roles.

2.  Navigate to the **Copilot Service admin center**.

    ![](./media/image1.png)

3.  Under **Customer support**, select **Channels**.

4.  On the **Channels** page, select **Manage** for **Chat**.

    ![](./media/image2.png)

5.  On the **Chat channels** page, select **Add chat channel**.

    ![](./media/image3.png)

6.  On the **Channel details** page, enter the following:

    - **Name** – !!Contoso Chat Widget!!

    - **Language** – **English – United States**

    - Keep the default values for the remaining settings.

    ![](./media/image4.png)

7.  Select **Next**.

    ![](./media/image5.png)

8.  On the **Workstream details** page, select **Add to Existing
    Workstream**.

9.  Select **Contoso Chat Workstream**.

10. Select **Next**.

    ![](./media/image6.png)

11. On the **Color Settings** page, select the **Cobalt** theme.

12. Select **Next**.

    ![](./media/image7.png)

13. On the **Header** page, select **Next**.

    ![](./media/image8.png)

14. On the **Chat Widget** page, keep the default values.

15. Set the **Proactive chat** toggle to **Yes**.

16. Select **Next**.

    ![](./media/image9.png)

17. On the **Behaviors** page, under **Custom automated messages**,
    select **Add a message**.

    ![](./media/image10.png)

18. In the **Add automated message** pane, select **Agent assigned to
    conversation** from the **Message trigger** dropdown list.

19. In the **Automated message** box, enter:

    !!Hi, how can I help you?!!

20. Select **Confirm**.

    ![](./media/image11.png)

21. Enable the **Pre-conversation survey** option.

22. Select **Add**.

    ![](./media/image12.png)

23. Enter the following survey details:

    - **Survey question name**: !!ContosoConsent!!

    - **Question text**: !!We collect demographic data. Please confirm
    whether you agree to provide the basic information.!!

    - **Answer type**: **User consent**

    - **Required**: **Yes**

24. Select **Confirm**.

    ![](./media/image13.png)

25. Select **Add** again.

    ![](./media/image14.png)

26. Enter the following survey details:

    - **Survey question name**: !!FirstName!!

    - **Question text**: !!FirstName!!

    - **Answer type**: **Single line**

    - **Required**: **Yes**

27. Select **Confirm**.

    ![](./media/image15.png)

28. Select **Add** again.

    ![](./media/image16.png)

29. Enter the following survey details:

    - **Survey question name**: !!LastName!!

    - **Question text**: !!LastName!!

    - **Answer type**: **Single line**

    - **Required**: **Yes**

30. Select **Confirm**.

    ![](./media/image17.png)

31. Select **Add** again.

    ![](./media/image18.png)

32. Enter the following survey details:

    - **Survey question name**: !!Age!!

    - **Question text**: !!Enter your Age!!

    - **Answer type**: **Single line**

    - **Required**: **Yes**

33. Select **Confirm**.

    ![](./media/image19.png)

34. Set the **Post-conversation survey** toggle to **Off**.

    ![](./media/image20.png)

35. Open the dropdown under **Authentication name** and review the
    **Create authentication setting** option.

    ![](./media/image21.png)

36. For this lab, do not continue with authentication setup because the
    remaining steps require a paid **Power Pages** license and custom
    certificate configuration.

37. Select **Cancel** after reviewing the authentication requirement.

    ![](./media/image22.png)

## Conclusion

In this lab guide, you created and configured a chat widget in the
Copilot Service admin center. You defined the channel details,
associated the widget with an existing workstream, applied a theme,
enabled proactive chat, configured an automated message, and added
pre-conversation survey questions. Together, these steps demonstrate how
organizations can prepare a structured chat experience for real-time
customer engagement in Dynamics 365 Contact Center.
