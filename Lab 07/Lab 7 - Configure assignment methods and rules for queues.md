# Lab 7 - Configure assignment methods and rules for queues

### Introduction

This lab demonstrates how to configure **assignment methods and rules
for queues** in Dynamics 365 Customer Service. You will create a work
assignment, define prioritization rulesets to manage case urgency, and
configure assignment rulesets that determine how cases are allocated to
agents. These steps help ensure that work items are distributed fairly
and efficiently, based on priority, agent availability, and skill sets.

1.  In the **Copilot Service admin center**, navigate to the site map
    and select **Queues** under **Customer support** group.

2.  On the **Queues** page, select **Manage** next to **Advanced
    queues**.

    ![A screenshot of a computer Description automatically
  generated](./media/image1.png)


3.  Select **Contoso queue for supervisors**.

    ![A screenshot of a computer Description automatically
  generated](./media/image2.png)

4.  On the **Contoso queue for supervisors**, click **See more** next to
    **Assignment method**.

    ![A screenshot of a computer Description automatically
  generated](./media/image3.png)

5.  On the **Assignment method** page, select **Create New**.

    ![A screenshot of a computer Description automatically
  generated](./media/image4.png)

6.  In the **Create work assignment** dialog, enter
    !!Contoso work assignment!! in the **Name** field and
    **Description** field and then select **Create**.

    ![A screenshot of a computer Description automatically
  generated](./media/image5.png)

7.  On the **Prioritization Ruleset** area, click **+ Create ruleset**.

    ![A screenshot of a computer Description automatically
  generated](./media/image6.png)

8.  On the **Create Prioritization Ruleset** dialog, enter
    !!Contoso prioritization ruleset!! in the **Name** field and
    **Description** field.

9.  Select **Create**.

    ![Graphical user interface, application Description automatically
  generated](./media/image7.png)

10. On the **Contoso prioritization ruleset** page, in the **Decision
    list** area, select **+** **Create rule.**

    ![A screenshot of a computer Description automatically
  generated](./media/image8.png)

11. On the **Create prioritization rule** dialog, enter
    !!Contoso prioritization rule!! in the **Name** field.

12. Select **+ Add** and then select **Add related entity**.

13. Add **Issue (Case)** entity in the first block.

14. Create the following condition: Priority **Equals** High.

15. In the **Order by** area, select **First in first out**.

16. Click **Create**.
    
    ![Graphical user interface, application Description automatically
  generated](./media/image9.png)

17. The **Contoso prioritization rule** is listed under **Decision
    list**.

    ![Graphical user interface, text, application, email Description
  automatically generated](./media/image10.png)

18. Click on the **Contoso work assignments** at the top to navigate
    back.

    ![](./media/image11.png)

19. To create an assignment ruleset, click **+ Create ruleset** on the
    **Assignment rulesets** area.

    ![Graphical user interface, text, application Description
  automatically generated](./media/image12.png)

20. On the **Create Assignment Ruleset** dialog, enter
    !!Contoso assignment ruleset!! in the **Name** field and
    **Description** field.

21. Click **Create**.

    ![A screenshot of a computer Description automatically
  generated](./media/image13.png)

22. On the **Contoso assignment ruleset** page, in the **Decision
    list** area, select **+** **Create rule.**

    ![A screenshot of a computer Description automatically
  generated](./media/image14.png)

23. **On the Create Assignment rule** page, enter
    !!Contoso assignment rule!! in the **Name** field.

    ![](./media/image15.png)

24. Click on the ellipsis icon on each condition rule and Delete the
    rules that are already added.

    ![](./media/image16.png)

25. Select **+ Add** and then select **Add row**.

    ![](./media/image17.png)

26. Create the following condition in the first row: User skills **Exact
    match** Skill.

    ![](./media/image18.png)

27. Select **+ Add** and then select **Add group**.

    ![](./media/image19.png)

28. Create the following condition in the group: Presence status
    **Equals** Available, Busy.

    ![](./media/image20.png)

29. Select **+ Add** in the group and then select **Add row**.

    ![](./media/image21.png)

30. Create the following condition in the new row: Calendar schedule
    **Is working**

    ![](./media/image22.png)

31. In the **Order by** area, select **Unit-based available capacity**.

32. Click **Create**.

    ![Graphical user interface, application Description automatically
  generated](./media/image23.png)

33. The **Contoso assignment rule** is listed under **Decision list**.

    ![A screenshot of a computer Description automatically
  generated](./media/image24.png)

### Conclusion

By completing this lab, you created assignment methods, prioritization
rules, and assignment rulesets for queues. This setup ensures that cases
are routed and assigned systematically, improving workload distribution
and enhancing the overall efficiency of customer service operations.
