# Table of Contents

- [Trello automation](#trello-automation)
  - [How Trello automation works](#how-trello-automation-works)
  - [Prerequisites](#prerequisites)
  - [Create automation](#create-automation)
  - [Create a card button](#create-a-card-button)
  - [Create a scheduled automation](#create-a-scheduled-automation)
  - [Troubleshooting](#troubleshooting)
    - [The automation did not run](#the-automation-did-not-run)
    - [The automation performed an unexpected action](#the-automation-performed-an-unexpected-action)
  - [Best practices](#best-practices)
  - [Summary](#summary)

---

## 1. Trello automation
Trello Automation allows users to automate repetitive actions on their dashboards. Instead of manually performing the same action each time a card changes, you can configure an automation to perform the action automatically when a specified condition is met.</br> </br>
![Screenshot](images/trello-12.png)
</br> </br>
For example, you can create an automation that moves a card to a specific list when a particular action occurs, or performs an action when a card is moved to another list.</br> </br>
![Screenshot](images/trello-10.png)
</br> </br>
This guide explains how to create and manage common automations in Trello.
### 2. How Trello automation works
A Trello automation generally consists of a trigger and one or more actions.
Trigger: Defines when the automation should run.
Action: Defines what Trello should do when the trigger occurs.
For example,
When a card is moved to the Done list (trigger), mark the card as complete (action).
Depending on the automation type, you can create automations based on rules, card buttons, board buttons, or scheduled events.
#### 2.1. Prerequisites
Before creating an automation:
- Sign in to Trello.
- Open the board where you want to create the automation.
- Create at least one list and a few cards that you can use to test the automation.
> **Note:** Ensure you have permission to configure automation on the board.
#### 2.2. Create automation
To create an automation rule in your board, follow the steps below.</br> </br>
![Screenshot](images/trello-05.png)
</br> </br>
- Select the **Create automation** button in the upper-right corner.</br> </br>
![Screenshot](images/trello-01.png)
</br> </br>
- In the Create a Rule page, select the Add Trigger button.</br> </br>
![Screenshot](images/trello-17.png)
</br> </br>
- For the **Select Trigger** step, select the required trigger category from the given options(For example, **Card Move**).

- Add the required trigger conditions.</br> </br>
![Screenshot](images/trello-15.png)
![Screenshot](images/trello-11.png)
</br> </br>
- Select the **+ (plus)** icon next to the required trigger to add it to the rule.</br> </br>
![Screenshot](images/trello-06.png)
</br> </br>
- Select the required action from the available options.
- Select the appropriate action category.
- Select the relevant conditions.
- Select the **+ (plus)** icon next to the action to add it to the rule.</br> </br>
![Screenshot](images/trello-02.png)
</br> </br>
- Review the rule configuration.
- Once you are ready, select **Save** in the upper-right corner.
#### 2.3. Create a card button
Card buttons allow users to manually trigger an automation from a card by selecting a button.</br> </br>
![Screenshot](images/trello-18.png)
</br> </br>
To create a button, follow the steps below.
- Select **Card buttons** on the left sidebar of your board.</br> </br>
![Screenshot](images/trello-13.png)
</br> </br>
- Select the **Create** button in the upper-right corner.</br> </br>
![Screenshot](images/trello-08.png)
</br> </br>
- Select the **Icon** button and select the appropriate icon for the button.
Add an appropriate Button Name.
- Select the **Enabled by default** and/or **Close card when action is performed** checkboxes if required.
> Note: Selecting Close card when action is performed archives the card automatically. Choose the option only if that is the intended outcome.
Once all the configurations are complete, select Add Action. The Select an Action section appears.</br> </br>
![Screenshot](images/trello-07.png)
</br> </br>
- Select the appropriate action category.
- Select the relevant conditions.
- Select the + (plus) icon next to the required action to add it to the button. The selected action is performed when you select the button.</br> </br>
![Screenshot](images/trello-03.png)
</br> </br>
- Once the configuration is complete, select Save in the upper-right corner.
#### 2.4. Create a scheduled automation
Scheduled automations allow you to configure actions that run according to a schedule.
For example, you could configure an automation to perform a recurring action on your board at a specified time.</br> </br>
![Screenshot](images/trello-16.png)
</br> </br>
To create a scheduled automation task, follow the steps below.
- Select **Scheduled** from the left sidebar.
- Select **Create automation**.</br> </br>
![Screenshot](images/trello-09.png)
</br> </br>
- Select **Add Trigger**.</br> </br>
![Screenshot](images/trello-04.png)
</br> </br>
- Choose an appropriate schedule and select the required schedule conditions.
- Select the **+ (plus)** icon next to the required schedule to add it.</br> </br>
![Screenshot](images/trello-19.png)
</br> </br>
- Select the appropriate action category.
- Select the relevant conditions.
- Select the **+ (plus)** icon next to the required action.
</br></br>The selected action will be performed at the scheduled interval.</br> </br>
![Screenshot](images/trello-14.png)
</br> </br>
- Once the configuration is complete, select **Save**.
### 3. Troubleshooting
#### 3.1. The automation did not run
Check the following:
- Confirm that the automation is saved and enabled.
- Verify that the trigger condition was actually met.
- Check that the configured action is valid.
- Test the automation with a new card.
- Review the automation configuration for incorrect conditions.
#### 3.2. The automation performed an unexpected action
Review the automation configuration and check all actions associated with the trigger. If multiple automations are configured on the same board, verify whether another automation could have affected the card.
### 4. Best Practices
When creating Trello automations:
- Start with simple automations and test them before creating complex workflows.
- Use descriptive names for automations.
- Test automations with sample cards before applying them to active workflows.
- Review existing automations before creating a new one to avoid duplicate actions.
- Document important automations so that other board members understand their purpose.
