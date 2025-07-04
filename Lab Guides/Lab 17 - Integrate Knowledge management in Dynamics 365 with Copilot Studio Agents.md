# Lab 17 - Integrate Knowledge management in Dynamics 365 with Copilot Studio Agents

**Objective** - In this lab, you will create a Copilot bot, add Topics to it and add the action to the Copilot Studio topic.

### Task 1 - Set connection references

To set connection references:

1.  Open a new tab and navigate
    to Power Apps portal !!https://make.powerapps.com/!!.

2.  Select the **Customer Service Trial** environment on the top right corner of
    the home page.

3.  Select **More** from the left navigation and then select **Connections**.

    ![A screenshot of a computer Description automatically
generated](./media/media18/image27.jpg)
  
4.  Select **New connection**.

   ![A screenshot of a computer Description automatically
generated](./media/media18/image28.jpg)

5.  Search for **Dataverse** and then select **Microsoft Dataverse**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image29.jpg)

6.  Select **Create**. Sign in with your credentials if prompted.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image30.jpg)

7.  Select **New connection**.

   ![A screenshot of a computer Description automatically
generated](./media/media18/image35.jpg)

8.  Search for and select **Content Conversion**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image36.jpg)

9.  Select **Create**. Sign in with your credentials if prompted.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image37.jpg)

     ![A screenshot of a computer Description automatically
generated](./media/media18/image38.jpg)

10.  From the left navigation of the Power Apps portal, select **Solutions** and then select **Default Solution**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image18.png)

11.  From the left navigation, select **Connection references** and then select **Microsoft Dataverse CDS Connection**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image31.jpg)

12. In the edit box that opens, select the connection that you created from the **Connection** dropdown menu.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image32.jpg)
   
13.  Select **Save changes**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image33.jpg)

14.  Similarly select **Content Conversion**.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image39.jpg)

15.  In the edit box that opens, select the connection that you created from the **Connection** dropdown menu.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image40.jpg)

16.  Select **Save changes**.

   ![A screenshot of a computer Description automatically
generated](./media/media18/image41.jpg)

17.  Go back to **Default Solution** \> **Cloud flows** and turn
    on **Search Dynamics 365 knowledge article flow** flow.

     ![A screenshot of a computer Description automatically
generated](./media/media18/image34.jpg)

## Task 2 – Create a Copilot Bot

1.  Open a tab in the browser and go to the Copilot Studio home page -
    !!https://copilotstudio.microsoft.com/!! . Login with the credentials
    provided to execute the lab. Accept the free trial, select United States for country/region.

2.  Select the Environment as **Customer Service Trial** on top right
    corner of the homepage

    ![A screenshot of a computer Description automatically generated](./media/media18/image1.png)

3.  Select **Agents** in the left navigation.

    ![A screenshot of a phone Description automatically generated](./media/media18/image2.png)

4.  Select **+ New agent**.

    ![A screenshot of a computer Description automatically generated](./media/media18/image3.png)

5.  Select **Skip to configure**

    ![A screenshot of a computer Description automatically generated](./media/media18/image4.png)

6.  Select **Create**.

    ![A screenshot of a computer Description automatically generated](./media/media18/image5.png)

    ![A screenshot of a computer Description automatically generated](./media/media18/image6.png)

7.  Your Agent is created.

    ![A screenshot of a computer Description automatically generated](./media/media18/image7.png)

## Task 3 - Create a Topic in Copilot Studio Bot

1.  For better visibility, close the **Test your agent** panel for now.

    ![A screenshot of a computer Description automatically generated](./media/media18/image8.png)

2.  On the top menu bar, select **Topics**.

    ![A screenshot of a computer Description automatically generated](./media/media18/image9.png)

3.  Select **Add a topic** and select **From blank**.

    ![A screenshot of a computer Description automatically generated](./media/media18/image10.png)

4.  Click on **Allow** if you are asked that copilot wants to access
    images and text.

    ![A screenshot of a computer Description automatically generated](./media/media18/image11.png)

    A **Trigger** node appears on an otherwise blank topic authoring canvas.

5.  Select **Details** on the toolbar to open the **Topic
    details** panel. Enter the name of the Topic as !!**Store hours**!!.

6.  Select **Save**.

        ![A screenshot of a computer Description automatically generated](./media/media18/image17.png)

### Task 4 - Add the action to the Copilot Studio topic

Perform the following steps to ensure that flow is properly configured
and can now be replaced with **Search Dynamics 365 knowledge
articles** action.

1.  Select **Add node** (**+**) and select **Add an action**.

2.  Select **Search Dynamics 365 knowledge article flow** action.

3.  Provide the input to the flow. An error might appear if the filter
    isn't provided to the flow.

    ![A screenshot of a computer Description automatically generated](./media/media17/image43-1.png)

    ![A screenshot of a computer Description automatically generated](./media/media18/image44.jpg)

3.  Select **Add node** (**+**) and select **Send a message** node to show the results returned by the flow. 

    ![A screenshot of a computer Description automatically generated](./media/media18/image45.jpg)

4.  Select **Save**.

5. Use the trigger phase and run the topic to verify the flow.

**Tip**

If your search doesn’t return any results, modify the search terms or
filter conditions. You can also add a filter condition if required.

**Summary** - You have created a Copilot Studio Agent, added Topics to it and then added the action to the Copilot Studio topic.
