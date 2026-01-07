# Running Live Giveaways and Contests with Comment Trigger


## Intro

This guide focuses on using Messcat to automate live giveaways and contests, streamlining the process and increasing participation.

## **Use Case: Running Live Giveaways and Contests**

- **Goal:** Efficiently manage live giveaways and contests based on specific comment actions.
- **Benefit:** Simplifies contest management, collects participant data, and boosts engagement.

![image.png](Running%20Live%20Giveaways%20and%20Contests%20with%20Comment%20T/image.png)

## **Steps to Implement:**

### **1. Define Your Giveaway/Contest Rules:**

- Determine the participation criteria (e.g., comment a specific word, tag friends, share the live video).
- Choose the prize and the method for selecting the winner.

### **2. Create the Giveaway Automation in Messcat:**

- **Trigger:**
    - Create a new "Facebook/Instagram Comment" trigger.
    - Set the condition: "Comment Text" contains your chosen keyword (e.g., "GIVEAWAY").
    - Set the condition: "Live Video Status" is "Live".
    - Optionally, add condition: "Time" is before "5:00 PM 5 Apr 2025"
    
    ![image.png](Running%20Live%20Giveaways%20and%20Contests%20with%20Comment%20T/image%201.png)
    
- **Action:**
    - Add a "Send Message" action.
    - Craft a private message (DM) confirming entry and providing further instructions.
    - Example: "You're entered! Stay tuned for the winner announcement. The giveaway end in 5pm 5 Apr 2025!"
    
    ![image.png](Running%20Live%20Giveaways%20and%20Contests%20with%20Comment%20T/image%202.png)
    
- **Optional Action:**
    - Add an "Add Tag" action.
    - Tag participants (e.g., "GiveawayEntry").
    
    ![image.png](Running%20Live%20Giveaways%20and%20Contests%20with%20Comment%20T/image%203.png)
    

### **3. Announce the Giveaway/Contest During the Live Stream:**

- Clearly explain the rules and how to enter.
- Prompt viewers to comment with the required keyword or perform the desired action.
- Example: "To enter, comment 'GIVEAWAY' and tag two friends!"

### **4. Monitor and Manage Entries:**

- Monitor the live chat and ensure Messcat is sending confirmation DMs.
- Use the tags to track participants.

### **5. Select and Notify the Winner:**

- After the live stream, use the tagged participants to select the winner.
- Send a private message (DM) to the winner with instructions on claiming the prize.

## **Key Considerations:**

- **Clear Instructions:** Provide easy-to-understand rules.
- **Engagement:** Encourage viewers to participate actively.
- **Transparency:** Be clear about the selection process.
- **Compliance:** Ensure your giveaway complies with platform rules.
- **Testing:** Test your automation before the live event.