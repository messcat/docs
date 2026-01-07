# Messenger/Instagram Channel FAQs


Here's a breakdown of common issues and solutions for Messenger and Instagram messages not appearing or functioning correctly in Messcat:

## **Why am I not getting any Messenger or Instagram messages in Messcat?**

- **No Facebook Business Page:**
    - Messcat requires a connected Facebook Business Page for Messenger integration. Personal Messenger accounts are not supported.
    - Ensure you have created and linked a Facebook Business Page.
- **Not Connected to Messcat:**
    
    ![image.png](Messenger%20Instagram%20Channel%20FAQs/image.png)
    
    - Verify that your Facebook Page is properly connected to Messcat.
    - Navigate to "Manage Channels" within Messcat.
    - Confirm that your page displays "Connected" along with the page's name.
- **Wrong Facebook Account:**
    - Double-check that you're looking at the messages on your Facebook Business Page, not your personal Facebook profile.
- **Another App is the Primary Receiver:**
    - Facebook allows only one application to manage messages from a page at a time.
    - If another application is set as the "Primary Receiver," Messcat will not receive messages.
- **Messages Sent from Another Platform:**
    - If the messages were sent using a platform outside of Messcat, they will not be shown within Messcat. Only the messages that are sent and recieved through Messcat will be visible.

## **Why are some chat names missing in Messcat?**

![image.png](Messenger%20Instagram%20Channel%20FAQs/image%201.png)

- **User Privacy:**
    - The user may have configured their Facebook privacy settings to hide their name.
- **Deleted User:**
    - The user's Facebook account might have been deleted or flagged as spam.
- **Permission Issue:**
    - Messcat may lack the necessary permissions to retrieve the user's name.
    - To resolve this:
        - Go to "Manage Channels" in Messcat.
        - Locate your Messenger channel.
        - Click the "Relink" button.
        - If the user sends a new message, their name should appear.
        
        ![image.png](Messenger%20Instagram%20Channel%20FAQs/image%202.png)
        

## **Why don't I see old Messenger chats in Messcat?**

- Facebook's API restricts applications from accessing messages that were sent before the connection was established.
- Consequently, Messcat will only display messages received after you connect your Messenger account.

## **Why am I getting an error when I try to send a message?**

- **"Error validating access token":**
    
    ![image.png](Messenger%20Instagram%20Channel%20FAQs/image%203.png)
    
    - This error typically occurs when you've logged out of Facebook or changed your password.
    - **Fix:** Navigate to "Manage Channels" in Messcat and click "Relink with Meta" for your Messenger channel.
- **"Message failed to send because another app is controlling this thread now":**
    - Only one application can manage a message thread at a time.
    - **Fix:** Relink with Meta and ensure Messcat is the primary receiver.
- **"(#10)Message is being sent outside the allowed window":**
    
    ![image.png](Messenger%20Instagram%20Channel%20FAQs/image%204.png)
    
    - Facebook enforces a 24-hour standard messaging window for automated responses.
    - After 24 hours only manually sent messages are allowed within a 7 day window, and must be used to follow up on a issue or provide assistance.
    - **Fix:** You must reply within 24 hours of the customer messaging you for automated messages, and 7 days for manually sent messages. Please refer to [this guide](https://developers.facebook.com/docs/messenger-platform/policy/policy-overview) for Meta’s full policy.