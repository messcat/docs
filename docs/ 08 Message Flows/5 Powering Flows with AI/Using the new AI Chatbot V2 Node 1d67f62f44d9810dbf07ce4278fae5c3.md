# Using the new AI Chatbot V2 Node

Article Description: Experience the versatility of the new AI capabilities of Messcat
Last Updated: April 14, 2025


The new AI node lets you smartly classify messages from users, connect with a knowledge base, and much more! Let’s see how we can utilise this power via message flows

Tip: complete our “AI ⇒ Knowledge Base” tutorial, that’ll give you a knowledge base to play with.

## Answering Queries

Putting an AI on the frontlines can be risky — it could hallucinate, give false information or simply be unhelpful. In this tutorial, we’ll see how to configure the AI bot with a knowledge base, prompt & alternate actions to minimise this risk.

### 1. Installing the Template

We’d recommend installing this template to get the demo running ASAP, by clicking [here](https://beta.Messcat.tech/automation/messageFlows/addEdit/new?templateId=132).

- Once it opens, it’ll ask for variable inputs:
    - Enter any one of your team members to start with
    - Select a knowledge base. If you’re looking to just try it out — we’d recommend the knowledge base from our tutorial, that builds a knowledge base for this business.
    Note: if you’re using a different knowledge base, be sure to change the “instructions” as they’re fine tuned for an Airbnb bot!

![Screenshot 2025-04-14 at 7.28.51 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_7.28.51_PM.png)

The flow has the following capabilities:

- We start with a trigger, which activates the flow when a customer message is received.
- There's a condition check that only replies to contacts without a "Manual Reply" tag to conversations
    - and with names containing mentioning "AI Test” (for testing purposes, can be removed when deploying to all)
- The AI Node has a "Knowledge Base" that contains information to answer common customer inquiries.
    - Instructions that allow the AI to fetch the value of the “Stay” custom field set on a user, removing the unnecessary step of repeatedly asking the user for it.
    - The flow also includes a "Save Stay" action which saves “stay” information in a custom field when the AI collects it, in case it wasn’t already present
    - We add an "Alternate Action" with instructions on identifying aggressive or irate customers, customers asking for a refund, and directing them to human agents. The “Manual Reply” tag is attached, so the AI no longer responds to this customer. The human agent when done responding — must remove the tag to allow the AI to continue responding
    - It also shows typing while the bot types — so the user feels some feedback, as these responses can take 20-40 seconds sometimes
- When the AI generates a response, the flow has multiple paths for different conditions and outcomes:
    - If the AI generates a response successfully, it posts that in a message
    - If there's a problem with the AI or something goes wrong, it notifies a human agent
- There's a "This Wasn't Helpful" condition path that triggers when a customer indicates the AI response wasn't satisfactory.
    - A "Response when Unhelpful" branch shows a pre-written apologetic message, and tags the conversation as “Unhelpful Reply”

### 2. Testing the Template

Ensure you have at least 1 connected channel, and that you have a chat that you can control to test with. Now, rename that chat to include “(AI Test)” in the name, so our flow can execute

![Screenshot 2025-04-14 at 7.53.22 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_7.53.22_PM.png)

Let’s send some messages now, we’re using a messenger channel to test, but you can test via a WhatsApp, Instagram or any other channel too.

![Screenshot 2025-04-14 at 7.53.35 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_7.53.35_PM.png)

(Bonus: you can see, without the AI even asking the name — it’s able to fetch the information & address our user correctly!)

If we set the “Stay” custom field to an Airbnb in the data we uploaded, it automatically knows this & can immediately respond! It correctly answers with a complex piece of text including special characters & symbols

![Screenshot 2025-04-14 at 7.55.39 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_7.55.39_PM.png)

Let’s test what happens when the custom field isn’t set. For that, we’ll:

1. remove the custom field
2. also update the “Session Group” in the AI chatbot node, the session group is an arbitrary piece of text, that on changing, will refresh all chat history for the AI (changed to “v4” from “v2”)
    
    ![Screenshot 2025-04-14 at 7.58.08 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_7.58.08_PM.png)
    

Now, let’s see what happens when we ask it for wifi info. We see it answered correctly (despite a typo — the correct name is “Suggest Stay 65”), and saved it to a custom field

![Screenshot 2025-04-14 at 8.03.22 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_8.03.22_PM.png)

If we try asking for a refund — it correctly executes our assignment flow!

![Screenshot 2025-04-14 at 8.07.53 PM.png](Using%20the%20new%20AI%20Chatbot%20V2%20Node/Screenshot_2025-04-14_at_8.07.53_PM.png)

## FAQ

- **Does the main reply still get sent if an alternate action is called?**
    
    Yes, even if an alternate action gets executed — the main reply is still called. This is because we often need the AI to respond and execute another action (eg. in our template, we want it to assign to a human agent and send an apologetic response when it cannot answer)