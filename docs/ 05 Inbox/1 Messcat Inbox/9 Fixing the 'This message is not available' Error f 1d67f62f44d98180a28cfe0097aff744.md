# Fixing the 'This message is not available' Error for Keyword Reply


![image.png](Fixing%20the%20'This%20message%20is%20not%20available'%20Error%20f/image.png)

## Intro

Sometimes messages show up as "This message is not available", preventing your keyword reply from working properly. In this guide, we'll show you how to fix this common issue and get your keyword replies working smoothly again.

## What Can You Do?

You can combat this by setting a keyword reply for such messages to let customers know that you are not able to view the message. They can ask the customer to send it again or send any other response.

### **Steps**

Here's how to set up an auto-response for unavailable messages:

1. Prepare a message flow that asks the customer to resend their message or provide an alternative response. Example:
    
    ![image.png](Fixing%20the%20'This%20message%20is%20not%20available'%20Error%20f/image%201.png)
    
2. Navigate to "Automation" > "Keyword Reply" from the left sidebar
3. Click [Create] in the top-right corner
4. Set condition to [Message Exactly Is] and enter "*ciphertext*" as the keyword
5. Select the message flow you created in step 1
    
    ![image.png](Fixing%20the%20'This%20message%20is%20not%20available'%20Error%20f/image%202.png)
    
6. Enable [Only Reply to New Message] in Advanced Settings to prevent duplicate responses
    
    ![image.png](Fixing%20the%20'This%20message%20is%20not%20available'%20Error%20f/image%203.png)
    
7. Click [Save] to finish setup.

### Video Refer

[[https://drive.google.com/file/d/180smaGRvaFNndZQQpkHx_bBM8PpFiL7o/view?usp=sharing](https://drive.google.com/file/d/180smaGRvaFNndZQQpkHx_bBM8PpFiL7o/view?usp=sharing)](https://drive.google.com/file/d/180smaGRvaFNndZQQpkHx_bBM8PpFiL7o/view?usp=sharing)

## FAQ

### Can I automatically respond to customers when I see "Message is not available"?

Yes, you can!  A good way to handle this is to set up a keyword reply specifically for these unavailable messages. This allows you to inform customers that you can't view their message and guide them on what to do next.

### Why do I use "ciphertext" as the keyword?

When you use "ciphertext" as the keyword, our system will be able to detect when messages are unavailable and automatically send your response. This exact keyword is required to properly identify these unavailable messages, so make sure to enter it exactly as shown in the steps above.