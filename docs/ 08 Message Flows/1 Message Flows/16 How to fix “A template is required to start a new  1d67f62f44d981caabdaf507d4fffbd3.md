# How to fix “A template is required to start a new conversation” Issue



## What does this issue mean?

![image.png](How%20to%20fix%20%E2%80%9CA%20template%20is%20required%20to%20start%20a%20new%20/image.png)

If you are using a WABA or WhatsApp Business account, there are some limitations that WhatsApp enforces when you are messaging a new contact:

1. If you are messaging a new contact who you have never contacted before, you must use a “Template” that is approved by WhatsApp
2. Once you start messaging a contact, that particular conversation lasts **24 hours**. After this time period, you can only start another conversation using a “Template” that is approved by WhatsApp

## What is a "Template"?

Template messages are pre-approved messages used for marketing, utility, and authentication communications with customers. They are required when starting conversations with customers who haven't contacted the business before or haven't communicated in the past 24 hours. These **templates require approval** and are **subject to deactivation** if customers report them negatively. If templates are disabled due to low quality ratings or policy violations, they remain unusable until the issues are fixed.

## How to submit a template for approval to WhatsApp

[[https://drive.google.com/file/d/1IhB_yagjx_fXxydjeLgDJ4WomnzkuaKf/view?usp=sharing](https://drive.google.com/file/d/1IhB_yagjx_fXxydjeLgDJ4WomnzkuaKf/view?usp=sharing)](https://drive.google.com/file/d/1IhB_yagjx_fXxydjeLgDJ4WomnzkuaKf/view?usp=sharing)

Follow these steps to submit a template for review:

1. Access 'Automation' in Messcat and select 'Messages Flow'.
2. Click '+Create New Flow', then choose your desired template or select 'Start from Scratch'.
3. Edit/create your flow as required
4. Click on the 3 dot menu on the top right and then select
    
    ![image.png](How%20to%20fix%20%E2%80%9CA%20template%20is%20required%20to%20start%20a%20new%20/image%201.png)
    
5. Choose your Channel, Category, and Language, and click 'Submit'.
6. You can check the submission status of the template in the template editor; Once a template is submitted, the approval process may take up to 24 hours.

## Limitations

While creating a message template to submit for review for WABA account, please refer below for the message template’s setting limitations.

| Button | Either [URL button] or [phone number button]
The combination will be either one of the below:
1. new message + URL button 
2. new message + phone number button 
3. new message + new message

- Maximum of 25 characters in Button name. |
| --- | --- |
| Delay | [Delay] action cannot apply to the “Starting Step” message. |
| List | [List] action cannot apply to the “Starting Step” message. |
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

## Why was my template rejected?

Submissions are commonly rejected for the following reasons, so make sure you avoid these mistakes.

- Variable parameters are missing or have mismatched curly braces. The correct format is `{{1}}`.
- Variable parameters contain special characters such as a `#`, `$`, or `%`.
- The message template contains content that violates WhatsApp’s Commerce Policy: When you offer goods or services for sale, we consider all messages and media related to your goods or services, including any descriptions, prices, fees, taxes and/or any required legal disclosures, to constitute transactions. Transactions must comply with the [WhatsApp Commerce Policy](https://www.whatsapp.com/legal/commerce-policy/?fbclid=IwAR0ChvA2WwuYF3wm1c-lm0QowlhhqQ0q0XXyAInUNAC4sAf2b9kSMGAl2OY).
- The message template contains content that violates the [WhatsApps Business Policy](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.whatsapp.com%2Flegal%2Fbusiness-policy%2F%3Ffbclid%3DIwAR3aEkRPDwU3orZ7acWbSCfoBTLAyDT-yyPDDRNIbbL6P5hhBtA_aiQNE64&h=AT3TmVTvpM52JvHbPSibw9G_AdLVtTVPBgV-mFEwJDZ6GLlRyl16rFAJK28HbbkwSDNpJqJRI4UVLUXwRvMr7dmLuvvg11DyHhjcrRiToVnMRK_DD74VEp6Abb2KVbqSXOwU8uWmjO-noRxqqUA6U-VTGcQ): Do not request sensitive identifiers from users. For example, do not ask people to share full length individual payment card numbers, financial account numbers, National Identification numbers, or other sensitive identifiers. This also includes not requesting documents from users that might contain sensitive identifiers. Requesting partial identifiers (ex: last 4 digits of their Social Security number) is OK.
- The content contains potentially abusive or threatening content, such as threatening a customer with legal action or threatening to publicly shame them.
- The message template is a duplicate of an existing template. If a template is submitted with the same wording in the body and footer of an existing template, the duplicate template will be rejected.

A rejection notification that includes the rejection reason will appear in [Business Support Home](https://business.facebook.com/business-support-home). You can view rejections in the Business Support Home by navigating to Account Overview > View my accounts (button) > (your Meta Business Account) > (your WABA) > Rejected message templates. Rejection info will also be sent via email.

You can refer to the Business Support Home notification to see the name and language of the existing template with the same content as the rejected duplicate template. You may also choose to edit the template and resubmit.This check does not apply to templates categorised as `AUTHENTICATION`.

## Messages Template Status (WABA)

![image.png](How%20to%20fix%20%E2%80%9CA%20template%20is%20required%20to%20start%20a%20new%20/image%202.png)

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