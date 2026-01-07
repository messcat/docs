# Contact Updated trigger



<aside>
💡 The Contact Updated trigger is activated whenever there is a change made to the contact (add/remove tag, changing name, etc.)

</aside>

### Using **Contact Updated Trigger**

You can use this trigger to send a message flow when a new tag has been added to a contact

![Untitled](Contact%20Updated%20trigger/Untitled.png)

### Using **Contact Updated Trigger** with **AI ChatBot**

You can use conditions to filter out the contacts based on tags, what type of messages you want to respond to, which channel you want to enable the trigger for, time of the message, and much more

![Screenshot 2024-06-07 at 1.18.49 PM.png](Contact%20Updated%20trigger/Screenshot_2024-06-07_at_1.18.49_PM.png)

---

### Difference Between Contact Properties and Contact Updated Properties when using condition with Contact Updated Trigger

**Contact Properties**

- Use this when you want to check a contact’s property, regardless of whether it was just updated.
- **Example**: To check if "John" is the assignee and you don’t care when the assignment was made, use "**Contact Properties**."

**Contact Updated Properties**

- Use this to check if a specific property of the contact has just been updated, causing the trigger.
- **Example**: If the assignee was just updated to "John" and you want to verify that change specifically, use "**Contact Updated Properties**."
- Key Use Case for Contact Updated Properties
    - "**Contact Updated Properties**" is particularly useful when multiple conditions need to be met in the same instance.
    - **Example**: If a "Responded" tag is added and "John" is assigned as the assignee simultaneously (e.g., in a **Modify Contact node**), you can use **Contact Updated Properties** to ensure the trigger is based on these updates.