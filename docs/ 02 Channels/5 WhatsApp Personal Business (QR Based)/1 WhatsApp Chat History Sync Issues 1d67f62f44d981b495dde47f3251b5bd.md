# WhatsApp Chat History Sync Issues

In depth guide to understand Chat History sync issues with QR based WhatsApp channels. 

## **WhatsApp Chat History Related Issues.**

To understand WhatsApp chat history sync issues, it would help us to first understand how QR based WhatsApp integrations work.

### **How do WhatsApp QR based integrations work?**

QR based WhatsApp integrations are like WhatsApp web connections with Messcat. This means that they will have all the limitations of WhatsApp Web but with powerful Messcat features.

### **Why are some of my previous chats missing?**

If you’ve recently connected a channel and the status shows that “waiting for chat history sync” then it is very likely that chats are syncing. If the volume of chats is large, it can take longer to sync, with some possible data loss in the process.

If the status instead shows that chat history sync is completed, and even then some of the chat history is missing. Then as mentioned earlier, QR based integrations suffer from all the limitations of WhatsApp Web. One of them being that chat history synced is sometimes not complete. This is a limitation that cannot be fixed.

To know more about this, please refer to the official WhatsApp article regarding chat history sync issues [here](https://faq.whatsapp.com/653480766448040). 

### **Where can I see missing old chats?**

Missing old chats should always be present on the primary WhatsApp device i.e. your phone. So, incase some chats are missing on Messcat but need to be accessed, your primary device is your best bet.

In some cases, we may be able to fetch older messages inside a chat, in that case the option to do so when scrolled to the topmost message in a chat. If, however, that option isn’t available/visible then it’s not possible.

### **Why are new chats after connecting to Messcat not syncing?**

If your new chats are not syncing with Messcat follow these steps –

1. Ensure your channel is connected by visiting the Manage Channels.
2. Refresh the page.

In most cases the above two steps will fix the issue. If not, then please report the issue and our team will look into it.

### **Will rescanning the QR code help in syncing all old messages?**

Rescanning QR code may or may not help in syncing all old messages. This is because when a channel is re-connected, the data received from WhatsApp can differ in its contents. In some cases, your issue may resolve, in other cases it may not. This is a limitation of QR based integrations.

It is important to note that rescanning the QR code may cause additional delays as lots of new data needs to be processed. **It is suggested that rescanning, if done, should be done during non-working hours to avoid disruptions during business hours**

### Why Can't I View Older Attachments (Images/Videos/PDFs/Other Files)?

Attachments are only available if they are downloaded on your mobile device. If an attachment has expired or cannot be downloaded on your phone, it will show an error in Messcat. 

Tips: Please enable auto-download in your WhatsApp mobile app to ensure all attachments are available.