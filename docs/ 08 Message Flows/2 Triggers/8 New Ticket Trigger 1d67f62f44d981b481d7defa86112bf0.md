# New Ticket Trigger



<aside>
💡 The Ticket Created trigger is activated whenever there is a new ticket created.

</aside>

### Using Ticket Created trigger to modify contact and update ticket.

Using the "Ticket Created" trigger and conditions, you can modify contact properties and also update CRM tickets

For ex: When a new ticket is created, you can add a tag and assign a team member. Also can start the minimum response timer.

Step 1: Add a new "Ticket Created" trigger.

Step 2: Add a condition for checking if the tag and an assignee is not there.

Step 3: Add a modifying contact node, which will add the tag and assign the team member to the contact.

Step 4: Add a update ticket node, which will start the minimum response timer for the assigned teammate.

Step 5: Add the flow/message you want to send in response if all conditions are met.

![Untitled](New%20Ticket%20Trigger/Untitled.png)

[](https://Messcat.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZWU1ZjA4ZjI3ODQ4MDk4MzI3Mzg4ZDZhM2ViMWYxNWVfb0wyQW1PYnZycURBQVhVOHVBdHllSWQ2MzU4ZDhuYjlfVG9rZW46RHhsNWJIMXgyb0x3QjJ4WjQxTWxhV3JPZ2xlXzE3MTg5NTI3NTc6MTcxODk1NjM1N19WNA)

<aside>
💡 You can use conditions to filter out the contacts based on tags, what type of messages you want to respond to, which channel you want to enable the trigger for, time of the message, and much more.

</aside>