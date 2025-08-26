# Lab 21 - Configure rules-based suggestions for contacts in Microsoft Teams

### Introduction

In this lab, you will learn how to configure rules-based suggestions for
contacts in Microsoft Teams through the Copilot Service admin center. By
enabling and customizing these rules, users can automatically receive
relevant contact suggestions when collaborating on Dynamics 365 records.
This capability improves team productivity by ensuring the right
individuals are recommended for ongoing cases or records, thereby
streamlining communication and reducing manual effort in identifying
stakeholders. The lab also covers how to enable collaboration, reorder
or disable rules, and create new custom rules for effective contact
suggestions.

## Exercise 1 - Turn on the suggested contacts for a record type

### Task 1 - To enable collaboration with Microsoft Teams and chat

1.  In the site map of Copilot Service admin center, in **Support
    experience**, select **Collaboration**.

2.  In **Embedded chat using Teams**, select **Manage**.

    ![](./media/image1.png)

3.  To get suggested contacts for any record type, perform the following
    steps:

    1.  In **Connect chat to Dynamics 365 records**, select record type-
        **Case** which we want to enable rules-based suggested contacts.
        The relative settings pane appears on the right.

        ![](./media/image2.png)

2.  In **Suggest contacts**, ensure the toggle for **Rules-based
    suggested contacts** is turned on if it is not already enabled.

3.  Select **Save** (If its already turned on it save option is not
    active click on the Cancel button).

    ![](./media/image3.png)

4.  In the **Update rules for suggesting contacts** section on the
    **Case** record, reorder or disable the rules for suggesting
    contacts. Users see the suggestions in the order we choose.

    - To reorder the rules, hover over a rule, and then select the up or
      down arrow to move the rules up or down, respectively.

      ![](./media/image4.png)

    - To disable a rule, hover over a rule, and then select the icon to
  disable the rule ![](./media/image5.png) . When the rule is disabled,
  a check mark is displayed when you hover over the disabled rule.

      ![](./media/image6.png)

    - To delete a rule, hover over the rule, and then
      select ![](./media/image7.png) . Deleting a rule removes it entirely
      so it won’t influence suggested contacts in the future.

      ![](./media/image8.png)

5.  Select **Save**.

## Exercise 2 - Adding a new rule

1.  On the settings pane, in the **Update rules for suggesting
    contacts** section, Select **Updates a timeline activity** rule.
    Delete the rule.

    ![A screenshot of a computer Description automatically
  generated](./media/image9.png)

2.  From the bottom of the section select **+** **Add rule**.

    ![](./media/image10.png)

3.  The **Add rule** pane is displayed for the record type you selected.

    ![A screenshot of a computer Description automatically
  generated](./media/image11.png)

4.  Enter the information as mentioned below.

    - **Rule name** - !!Created By!!

    - **Rule Type** - Relational

    - **Select a user or related record** – Created By

    - Select **Save**

      ![](./media/image12.png)

5.  A new rule is created. Select **Save** again.

      ![](./media/image13.png)

6.  Select **Save** on **Microsoft Teams collaboration and chat**

      ![A screenshot of a computer Description automatically
  generated](./media/image14.png)

### Conclusion

By completing this lab, you have successfully configured rules-based
suggestions for contacts in Microsoft Teams. You explored how to
enable suggested contacts for a record type, update and manage rules,
and create a new rule to ensure meaningful collaboration. These steps
enhance the integration between Microsoft Teams and Dynamics 365,
making it easier for users to engage with the right people at the
right time. With these configurations, organizations can improve
collaboration efficiency, reduce communication gaps, and strengthen
case resolution processes through intelligent, rules-driven contact
suggestions.
