# Outgoing message trigger



<aside>
💡 The outgoing message trigger is activated whenever there is a new message sent.

</aside>

### Using outgoing message trigger to modify contact and update ticket.

Using the "Outgoing Message" trigger and conditions, you can modify contact properties and also update CRM tickets.

For ex: When you send a message which contains the word “resolve” in it, you can modify contacts info and update their ticket.

Step 1: Add a new "Outgoing Message" trigger

Step 2: Add a condition for a specific channel, a condition for text, and input the keyword you want it to check, and a condition for a specific tag

Step 3: Add a Modify Contact App Node, which can change a contacts info.

Step 4: Add a Update Ticket App Node, which can change the status of a particular ticket of that contact

![Untitled](Outgoing%20message%20trigger/Untitled.png)

[](https://Messcat.sg.larksuite.com/space/api/box/stream/download/asynccode/?code=ZWU1ZjA4ZjI3ODQ4MDk4MzI3Mzg4ZDZhM2ViMWYxNWVfb0wyQW1PYnZycURBQVhVOHVBdHllSWQ2MzU4ZDhuYjlfVG9rZW46RHhsNWJIMXgyb0x3QjJ4WjQxTWxhV3JPZ2xlXzE3MTg5NTI3NTc6MTcxODk1NjM1N19WNA)

<aside>
💡 You can use conditions to filter out the contacts based on tags, what type of messages you want to respond to, which channel you want to enable the trigger for, time of the message, and much more

</aside>