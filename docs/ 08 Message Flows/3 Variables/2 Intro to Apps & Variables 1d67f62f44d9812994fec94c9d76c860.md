# Intro to Apps & Variables

Article Description: Use variables & apps to automate your business


App nodes are a powerful way for your flows to interact with the Messcat ecosystem & the rest of the world. You can do everything from creating a ticket, asking GPT a question to requesting data from your own servers.

This power can be compounded by chaining multiple apps together that pass information between each other via variables.

We’ll attempt to build an automated flow where all incoming inquiries are passed to our trained chatbot, and then if the chatbot couldn’t answer the query — we’ll create a ticket for it and notify our customer service (CS) teammate.

For the impatient of you, you can play with the created flow by clicking [here](https://app.messcat.ai/message-flow/slug_02b2f6c7c064cc809ba12fdccaa92282)

1. We’ll start by setting up our AI chatbot, which you can do [here](https://www.app.messcat.ai/ai/aiChatbot)
    
    ![Screenshot 2024-07-03 at 3.53.55 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_3.53.55_PM.png)
    
2. Next, let’s create a Kanban board where we’ll put all customers whose queries the chatbot couldn’t answer, and need manual attention. You can create one in the CRM [here](https://www.app.messcat.ai/crm/crm-board). We’ve created a simple one here with 2 stages:
    1. Customers will first be put into the “Open” stage
    2. Once we’ve answered their query, we’ll close their ticket & move into the “Closed” stage
    
    ![Screenshot 2024-07-03 at 3.55.16 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_3.55.16_PM.png)
    
3. Once the chatbot is setup, we’ll create a message flow and add an “Incoming Message” trigger. This trigger will start the flow whenever we receive any message from our customers. We’ll attach a condition node after it.
    
    ![Screenshot 2024-07-03 at 3.49.23 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_3.49.23_PM.png)
    
4. Next, we’ll add some conditions.
    1. First, from the trigger node — we’ll add a condition node to it.
        
        ![Screenshot 2024-07-03 at 4.06.42 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_4.06.42_PM.png)
        
    2. Next, we’ll check if the customer messaging us doesn’t already have an open ticket. We do this because if the AI isn’t able to answer a customer — if the customer texts again, the AI shouldn’t respond again to avoid spamming the customer with nonsense.
    3. We achieve this by clicking the “Add Condition” variable & accessing the “Ticket Stage” variable & then ensuring no open ticket exists via an “is not” condition
    
    ![Screenshot 2024-07-03 at 3.57.28 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_3.57.28_PM.png)
    
    ![Screenshot 2024-07-03 at 4.02.59 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_4.02.59_PM.png)
    
5. Next, we’ll connect the condition to an “AI Chatbot” node.
    - Click “Choose Next Step” and select “AI Chatbot”
        
        ![Screenshot 2024-07-03 at 4.11.57 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_4.11.57_PM.png)
        
    - Add the integration we created step 1
        
        ![Screenshot 2024-07-03 at 4.25.56 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_4.25.56_PM.png)
        
    - To pass the incoming message’s text to the chatbot, so it can process it — we’ll use the “Text” variable. We’ll access this by pressing the `{` key since “Input Text” is a free text field.
        
        ![Screenshot 2024-07-03 at 4.29.34 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_4.29.34_PM.png)
        
6. Once we get a response from the AI chatbot, we’d want to check if the bot was able to actually give a meaningful response. If so, we’d want to forward the response back to the user.
    - We’ll can do so by adding a condition from the AI chatbot node, and checking if “Successful Response” is true — i.e. the AI chatbot managed to generate a successful response
        
        ![Screenshot 2024-07-03 at 5.36.58 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_5.36.58_PM.png)
        
    - We’ll connect a message node when this condition matches, and there — we’ll use the textual output of the AI chatbot & send it back to the customer. The text output can be obtained via the “Reply” variable — we’ll select that and just let that be the text of the message
        
        ![Screenshot 2024-07-03 at 5.44.31 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_5.44.31_PM.png)
        
    - Bonus: scroll down and check “read chat on send” — this will automatically mark the chat as read as soon as this message is sent. On WhatsApp channels, it’ll even show a “typing…” sign to the recipient
        
        ![Screenshot 2024-07-03 at 5.47.42 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_5.47.42_PM.png)
        
7. Now, let’s handle the case where the AI chatbot failed to create a “successful response”. We’d want to create a ticket so our CS teammate can respond to them
    1. From the condition node created in step 6, we’ll connect a new “Create Ticket” node from the “If None Match” section. (The node connected in the section is called when none of the conditions you have set matched)
        
        ![Screenshot 2024-07-03 at 5.51.55 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_5.51.55_PM.png)
        
    2. In the Create Ticket App — we’ll set the name of the ticket alongside the stage it’ll get created in.
        1. For the title, we’ll use the “Name” variable suffixed with “- AI Fail” so we know where it came from
        2. For the stage, we’ll select the “Open” stage from the CRM board we created in step 2
        
        ![Screenshot 2024-07-03 at 5.56.37 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_5.56.37_PM.png)
        
8. Let’s assign this customer to our CS teammate.
    1. For this, we’ll select the “Modify Contact” app in the next step section of the “create ticket” app we made in step 7
        
        ![Screenshot 2024-07-03 at 6.03.28 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_6.03.28_PM.png)
        
    2. Next, in the “Modify Contact” app — we’ll select our CS teammate as the assignee
        
        ![Screenshot 2024-07-03 at 6.04.09 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_6.04.09_PM.png)
        
9. Finally, let’s send a message to the customer — letting them know we’ll get back to them ASAP
    1. We’ll simply connect a message node from the “Modify Contact” node we just created & type in a message
        
        ![Screenshot 2024-07-03 at 6.08.40 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_6.08.40_PM.png)
        
10. Voila! We’ve an automated flow to take care of possibly all your CS & product inquiries. Test it out by sending one of your connected channels a message
    
    ![Screenshot 2024-07-03 at 6.10.06 PM.png](Intro%20to%20Apps%20&%20Variables/Screenshot_2024-07-03_at_6.10.06_PM.png)