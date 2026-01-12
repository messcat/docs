# What are Template Messages?

## Messages Types

We support two types of messages: **free-form messages** and **template messages**. Template messages can only be sent to a user who has opted-in to allow a business to send messages to them. When using template messages, a template is required and must be approved by the review team before sending messages to customers.

## What are Template Messages?

Template messages are a specialized form of communication utilized in marketing, utility, and authentication interactions with customers. These templates are essential for initiating conversations with customers who have either not yet contacted the business or have not communicated in the past 24 hours. Before usage, these templates require approval and are subject to deactivation based on customer feedback. If disabled due to poor quality ratings or policy violations, they cannot be used until these issues are resolved.

## How to Submit Templates for Review (WABA)

Please refer to: [submit template for review](https://help.messcat.ai/message-flows/kSYFmwLcqbtLQQAhJb4Sek/how-to-fix-%E2%80%9Ca-template-is-required-to-start-a-new-conversation%E2%80%9D-issue/5JcftRTEFQudb971cteGPw)

## Message Flow Limitations (WABA)

While creating a message template to submit for review for WABA account, please refer below for the message template’s setting limitations.

| Button | Either [URL button] or [phone number button]
The combination will be either one of the below:
1. new message + URL button 
2. new message + phone number button 
3. new message + new message

- Maximum of 25 characters in Button name. |
| --- | --- |
| Delay | [Delay] action cannot apply to the “Starting Step” message. |
| User Input | [User input] feature is not allowed. |
| Voice Message | [Voice Message] cannot be inserted. |
| Image | media files format: image/jpeg, image/png
maximum size: 5MB

Images must be 8-bit, RGB or RGBA |
| Video | media files format: video/mp4, video/3gp
maximum size: 16MB 

Notes:
- Only H.264 video codec and AAC audio codec is supported.
- We support videos with a single audio stream or no audio stream. |

### Common Message Flow Rejection Reasons (WABA)

Submissions are commonly rejected for the following reasons, so make sure you avoid these mistakes.

- Variable parameters are missing or have mismatched curly braces. The correct format is `{{1}}`.
- Variable parameters contain special characters such as a `#`, `$`, or `%`.
- The message template contains content that violates WhatsApp’s Commerce Policy: When you offer goods or services for sale, we consider all messages and media related to your goods or services, including any descriptions, prices, fees, taxes and/or any required legal disclosures, to constitute transactions. Transactions must comply with the [WhatsApp Commerce Policy](https://www.whatsapp.com/legal/commerce-policy/?fbclid=IwAR0ChvA2WwuYF3wm1c-lm0QowlhhqQ0q0XXyAInUNAC4sAf2b9kSMGAl2OY).
- The message template contains content that violates the [WhatsApps Business Policy](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.whatsapp.com%2Flegal%2Fbusiness-policy%2F%3Ffbclid%3DIwAR3aEkRPDwU3orZ7acWbSCfoBTLAyDT-yyPDDRNIbbL6P5hhBtA_aiQNE64&h=AT3TmVTvpM52JvHbPSibw9G_AdLVtTVPBgV-mFEwJDZ6GLlRyl16rFAJK28HbbkwSDNpJqJRI4UVLUXwRvMr7dmLuvvg11DyHhjcrRiToVnMRK_DD74VEp6Abb2KVbqSXOwU8uWmjO-noRxqqUA6U-VTGcQ): Do not request sensitive identifiers from users. For example, do not ask people to share full length individual payment card numbers, financial account numbers, National Identification numbers, or other sensitive identifiers. This also includes not requesting documents from users that might contain sensitive identifiers. Requesting partial identifiers (ex: last 4 digits of their Social Security number) is OK.
- The content contains potentially abusive or threatening content, such as threatening a customer with legal action or threatening to publicly shame them.
- The message template is a duplicate of an existing template. If a template is submitted with the same wording in the body and footer of an existing template, the duplicate template will be rejected.

A rejection notification that includes the rejection reason will appear in [Business Support Home](https://business.facebook.com/business-support-home). You can view rejections in the Business Support Home by navigating to Account Overview > View my accounts (button) > (your Meta Business Account) > (your WABA) > Rejected message templates. Rejection info will also be sent via email.

You can refer to the Business Support Home notification to see the name and language of the existing template with the same content as the rejected duplicate template. You may also choose to edit the template and resubmit. This check does not apply to templates categorized as `AUTHENTICATION`.

### Messages Template Status (WABA)

Templates can have the following statuses.

- In-Review: Indicates that the template is still under review. Review can take up to 24 hours.
- Rejected: The template has been rejected during our review process or violates one or more of our policies.
- Active - Quality pending: The message template has yet to receive quality feedback from customers. Message templates with this status can be sent to customers.
- Active - High Quality: The template has received little to no negative customer feedback. Message templates with this status can be sent to customers.
- Active - Medium Quality: The template has received negative feedback from multiple customers but may soon become paused or disabled. Message templates with this status can be sent to customers.
- Active - Low Quality: The template has received negative feedback from multiple customers. Message templates with this status can be sent to customers but are in danger of being paused or disabled soon, so we recommend that you address the issues that customers are reporting.
- Paused: The template has been paused due to recurring negative feedback from customers. Message templates with this status cannot be sent to customers.
- Disabled: The template has been disabled due to recurring negative feedback from customers. Message templates with this status cannot be sent to customers.
- Appeal Requested: Indicates that an appeal has been requested. See [Appeals](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#appeals). The appeal will be reviewed and a decision made within 24 hours.

You can view a template's status by going to WhatsApp Manager > Overview, mousing over the suitcase icon (Account tools) and clicking Message templates. If you have multiple WhatsApp Business Accounts, select the account whose template statuses you want to view from the list of accounts in the dropdown menu in the top-right corner.

### **Message Sending Limits (WABA)**

Business phone numbers with a connected status and approved display name can initiate conversations with the following number of unique customers in a rolling 24-hour period:

- 1K business-initiated conversations
- 10K business-initiated conversations
- 100K business-initiated conversations
- An unlimited number of business-initiated conversations

This amount starts at 1K unique customers and scales automatically based on phone number status, phone number quality rating, and how often you initiate conversations with unique customers.

![image (9).png](What%20are%20Template%20Messages/image_(9).png)

### **How to Increase Your Message Limit**

Each time you initiate a new conversation with a unique customer, WhatsApp will determine if your limit should be increased. This determination is based on the following criteria:

- Your phone number status is **Connected**
- Your phone number quality rating is **Medium or High**
- In the last 7 days, you have initiated X or more conversations with unique customers, where X is your current messaging limit divided by 2

<aside>
💡 ***If you meet all conditions, WhatsApp will increase your messaging limit by one level in 24 hours.***

</aside>

## FAQ

### **How to check your message limit**

- You can check your current messaging limits in the WhatsApp Manager > Overview Dashboard > Insights tab. The panel depicted below will only show your current limit if your messaging limit has increased from the default limit of 250.

### **How to maintain a high-quality message template?**

- Make sure messages follow [WhatsApp's Business Policy](https://www.whatsapp.com/legal/business-policy/?fbclid=IwAR0UOSi5UFphXQyWnkH-rVn--pBJcMiyz4D1cqA9m0D25hSSKC7dvF0Aqxk) and [Commerce Policy](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.whatsapp.com%2Flegal%2Fcommerce-policy%2F%3Ffbclid%3DIwAR2x-7FFJ7YYS4YY92kFtYN3OVcFvt1Y5cwEKjnIMqu-A7bFTEyMa4uFVFc&h=AT1xIOb3fW4iQksucE3KCIkZzOUiLcj5dUuGPJ58vxBfkmqNWu7arIU5aSc8BWIid1SlZU8iU-rvnTTtf3MNnouvKnzAAatKuqBaYNveXPR4fEzmu9oeTB4Rf4zHa450RG5RSpxmOB8).
- Only send messages to users who have opted into receiving messages from your business.
- Make the messages highly personalized and useful to users. Avoid sending open-ended welcome or introductory messages.
- Be mindful of messaging frequency; avoid sending customers too many messages a day. Be thoughtful of informational messages, optimizing for content and length.

### **Why is my message limit being decreased?**

- Each time you initiate a new conversation with a unique customer we will check your phone number quality rating. If the rating has been flagged for the last 7 days, we will immediately decrease your messaging limit by one level.