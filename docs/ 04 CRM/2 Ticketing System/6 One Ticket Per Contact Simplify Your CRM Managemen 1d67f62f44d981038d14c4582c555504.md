# One Ticket Per Contact: Simplify Your CRM Management

Imagine this: Your customer support team is managing tickets in your CRM, and every time a customer interacts with your business, a new ticket gets created. Now, instead of resolving issues efficiently, your team is drowning in duplicate tickets for the same contact. 😵‍💫

Here’s another scenario: You have a setup where tickets are created automatically, but once a ticket is resolved, there’s no way to reopen the system for a new ticket without manual intervention. Sounds frustrating, right? 😖

This is where the **One Ticket Per Contact Flow** comes to the rescue! 🎉

- **No Duplicate Tickets**: It ensures only one active ticket per contact is allowed at a time, keeping your CRM organized.
- **Re-enabling Ticket Creation**: Once a ticket is closed, the flow reopens the system for new tickets, fully automated.
- **Customizable**: Easily adjust triggers, ticket names, board stages, and more to fit your business needs.

Let’s dive into how this flow works and how you can tailor it to streamline your CRM workflows!

---

<aside>
📌

### **Important Pre-Requisites**

1. **CRM Setup**:
    - Create a **new CRM board** dedicated to this setup.
    - Alternatively, ensure your existing CRM board contains only **one ticket or no ticket per contact**.
    - This prevents issues caused by multiple tickets per contact.
2. **Enable Triggers**:
    - Once you import the template into your team, make sure to **enable all triggers** in the flow.
    - Without enabling the triggers, the flow will not work as intended.
</aside>

---

### **How the Flow Works**

This message flow uses smart automation to check for existing tickets before creating a new one, tag contacts to track ticket status, and even re-enable ticket creation after closure. You can start using it with the provided [Message Flow Template](https://www.app.messcat.ai/automation/templateMarket/view/118).

Here’s a detailed breakdown:

---

### **Step 1: Setting the Event Trigger**

- **Default Trigger in Template**:
    
    The flow is triggered by an **incoming message**.
    
- **Customizable Options**:
    
    You can change the trigger to better match your use case, such as:
    
    - **Contact Updated** ([Learn more](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/contact-updated-trigger/x2LKj5xzjxdZ8nSyPd5JiS))
    - **New Contact** ([Learn more](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/new-contact-trigger/7K5rUuLmLCd3DmSeF2Xdt5))
    - **New Chat Started** ([Learn more](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/new-chat-trigger/43A1hEZi9QDYBAmDPtsj5V))

---

### **Step 2: Using the Condition Node**

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image.png)

The **Condition Node** is at the heart of the flow. It prevents duplicate tickets by checking if the contact has a specific tag (default: **Ticket Checker**).

- **Tag Setup**:
    - In the template, this tag is set as a **Flow Variable** for easy updates across the flow.
    - Learn more about [Flow Variables here](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/flow-variables/vPrCvh6mu2cFo7q2iwP2aQ).

If the tag exists, no new ticket is created. If it doesn’t, the flow moves to the next step.

---

### **Step 3: Creating a Ticket**

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image%201.png)

When the Condition Node allows it, the **Create Ticket Node** is activated.

- **Customizing Ticket Details**:
    - **Ticket Name**: Use custom fields and predefined variables like `{{Name}}` or `{{Phone Number}}` to dynamically personalize ticket names. Learn about [available variables here](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/available-variables/ebJmBZuZStuzg7j3gH2zi2).
    - **Board Stage**: Set this using the Flow Variable **Ticket Board and Stage** for centralized management.

For a deeper understanding of the Create Ticket Node, click [here](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/how-to-use-the-create-ticket-node/gs1JR1RbELeWv8zzPh3vvF).

---

### **Step 4: Tagging the Contact**

After creating the ticket, the **Modify Contact Node** adds the **Ticket Checker** tag to the contact.

- **Purpose**: This tag ensures the flow skips creating another ticket if triggered again.
- **Default Configuration**: The template uses the **Ticket Checker Flow Variable** to manage this step.

For a deeper understanding of the Modify Contact Node, click [here](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/how-to-use-the-modify-contact-node/3gRYWsiT6aJ6wUxBEQUaUq).

---

### **Step 5: Adding Custom Steps (Optional)**

Feel free to add more steps, such as:

- Sending a confirmation message to the contact.
- Adding a delay for processing time.
- Triggering additional automated actions.

---

### **Step 6: Re-enabling Ticket Creation for Closed Tickets (Highly Recommended)**

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image%202.png)

Want to automatically create tickets for a contact again after their current ticket is closed? Here’s how to do it:

1. Add a **Ticket Updated Trigger**.
2. Connect the trigger to a **Condition Node** that checks if the ticket is in the **last stage** (e.g., "Closed").
    - The template uses the Flow Variable: **Last Stage for Removing Tag**.
3. Connect the Condition Node to a **Modify Contact Node** that removes the **Ticket Checker** tag.

### **Why Step 6 is a Game-Changer?**

Without this step, you’d need to manually manage tags to allow new tickets after closure. With it, your system is fully automated, ensuring a seamless workflow for repeat interactions.

---

### **Start Using the Flow**

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image%203.png)

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image%204.png)

To access the flow variables follow these steps:

- Open the “horizontal 3 dots” menu in the top-right corner.
- Click “Flow Variables” to view and edit all flow variables used in this template.

![image.png](One%20Ticket%20Per%20Contact%20Simplify%20Your%20CRM%20Managemen/image%205.png)

Ready to optimize your ticketing system? Import the [Message Flow Template](https://www.app.messcat.ai/automation/templateMarket/view/118), customize it to your needs, and experience a streamlined, automated CRM setup.

For further guidance, reach out to our support team anytime!

---