# How to Migrate your Whatsapp Business API from another service provider?

# **Intro**

Migrating a WhatsApp Business Account (WABA) can be a complex process that involves several critical steps and considerations. This guide will walk you through the necessary preparations, the migration steps, and provide a use case to illustrate the process.

![Migration.jpeg](../../Channels/WhatsApp%20Business%20API/How%20to%20Migrate%20a%20Whatsapp%20Business%20API%20Account/Migration.jpeg)

# Pre-requisites for Migration

<aside>
❗ **Important Note:**
1. These prerequisites are **mandatory** for processing your migration request. 
2. Partial or incomplete information cannot be processed and may extend the time, or cancel the request altogether for the migration.

</aside>

## Before you begin

- Retrieve your **Business Manager ID** and check on the **verified status** on [here](https://business.facebook.com/settings/info?business_id=286937502422506&global_scope_id=286937502422506).
- Retrieve the WhatsApp Display name on this [page](https://business.facebook.com/wa/manage/phone-numbers/?business_id=286937502422506&waba_id=107209238888967).
- Make sure you have admin access to the Facebook Business Manager associated with your WABA. You can check through you access here.
- Locate your Facebook Business Manager ID. You'll need it during the process.
- Ensure your Facebook Business Account is verified.
- Have a phone number ready to receive a 6-digit verification code via SMS or call.
- Note down your current WhatsApp Business Account's display name.
- Please make sure the two-step verification (2FA) for your WhatsApp number is disabled.

# **Migration Steps**

## **Access MesscatChannels**

- Go to the **Manage Channels** section on Messcat.

## **Add a WhatsApp Channel**

- Click the **+ Channel** button and select **WhatsApp Business API**.
    
    ![waba channel.jpeg](../../Channels/WhatsApp%20Business%20API/How%20to%20Migrate%20a%20Whatsapp%20Business%20API%20Account/waba_channel.jpeg)
    
    <aside>
    ❗ When creating a WABA (WhatsApp Business API) channel, please be aware that charges will apply based on the number of channels created. For more detailed pricing information, please refer to the MesscatCredit Price List via the "Manage Plan" section. If you have any questions or need further assistance, feel free to reach out to our support team.
    
    </aside>
    

## **Login to Facebook Business Manager**

- Log in to your Facebook Business Manager account.

## **Select Business Account**

- Choose the correct Meta Business account you want to connect and click **Next**.

## **Link WABA**

- Select your existing WhatsApp Business Account. If creating a new one, choose **Create a new WhatsApp Business Profile** and click **Next**.
    
    ![FB 2.jpeg](../../Channels/WhatsApp%20Business%20API/How%20to%20Migrate%20a%20Whatsapp%20Business%20API%20Account/FB_2.jpeg)
    

## **Configure New WABA (if applicable)**

- If creating a new WABA, enter your desired display name, select your business category, and click **Next**.
    
    ![FB.jpeg](../../Channels/WhatsApp%20Business%20API/How%20to%20Migrate%20a%20Whatsapp%20Business%20API%20Account/FB.jpeg)
    

## **Verify Phone Number**

- Enter your WABA phone number to receive a verification code.

## **Complete Connection**

- Once you receive the code, enter it to finalize the connection between Messcatand your WABA.

<aside>
❗ **Important Notes:**

- Message history and chat data cannot be migrated during this process.
- Billing transitions with the migration. Old messages are charged by the previous BSP, while new messages are billed by Messcat.
- Sometimes Meta's OTP via SMS may not be received, and robot calls may not provide the OTP. It is preferable to request the OTP via text message rather than a call.
</aside>