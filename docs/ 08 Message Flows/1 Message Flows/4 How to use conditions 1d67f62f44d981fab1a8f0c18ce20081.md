# How to use conditions



The conditions block allows you to change your customer interactions based on where they live, a particular tag, their assignee, and much more. 

### Step-by-Step Guide

1. Navigate to the message flow where you want to add conditions
2. Click on the "Condition" block and then on “Check Condition” to open the condition settings
3. You will see an option to specify if **"All"** or **"Any"** of the conditions should match. This allows you to determine whether all specified conditions must be met (AND logic) or if any one of them can trigger the action (OR logic).
4. In the dropdown, you will see various properties such as **Unique ID**, **Channel**, **Name**, **Phone Number**, **Tag**, **Country**, **Assignee**, and more. Select the property that you want to use as a condition.
5. Once you select a property, specify whether the condition **"is"** or **"is not"** met. In some cases such as Name, Phone number etc, you will also see options like “**contains”**, **“starts with”**, **“ends with”**, etc.
6. Next, you will see a list of possible values. For the **Channel** property, this includes various phone numbers. For properties like **Name**, you can input custom values. Check the appropriate boxes to select the specific channels you want to include or exclude.
7. If you want to add more conditions, go to the “**If not**” section and click on “**Check Another Condition**”
8. Continue building your message flow by choosing the next step or adding further conditions

Here are the available condition options and how you can use them:

**Contact/ Contact Updated/ New Contact Properties**

- Unique ID
- Channel
    
    Specify the channel name to condition. The following message will only be sent if the contact does or does not belong to that channel.
    
    **Example**: If a contact belongs to the "Malaysia" channel, send them a special discount code for the Deepawali holiday.
    
- Name
- Phone number
- Tag
- Country
- Assignee
- Messages received
- Messages sent
- Type (Individual/Group)
- Ticket stage
- Ticket ID

---

### Difference Between Contact Properties and Contact Updated Properties

- **Contact Properties**
    
    Use this when you want to check a contact’s property, regardless of whether it was just updated.
    
    **Example**: To check if "John" is the assignee, and you don’t care when the assignment was made, use "**Contact Properties**."
    
- **Contact Updated Properties**
    
    Use this to check if a specific property of the contact has just been updated, causing the trigger.
    
    **Example**: If the assignee was just updated to "John" and you want to verify that change specifically, use "**Contact Updated Properties**."
    

**Key Use Case:**

"**Contact Updated Properties**" is especially useful when multiple conditions, like adding a "Responded" tag and assigning "John" as the assignee, are applied simultaneously in one node (e.g., a Modify Contact node).

**Incoming/Outgoing Message Properties**

- Text
- Time
- Channel
- Chat ID
- Is Button Click
- Sender(Outgoing messages only)

**AI Chatbot Response**

- Successful Response
- Reply

**Context**

- Time of event

**Miscellaneous**

- Custom