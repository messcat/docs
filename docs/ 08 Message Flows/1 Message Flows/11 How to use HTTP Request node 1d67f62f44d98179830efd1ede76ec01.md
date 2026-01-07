# How to use HTTP Request node



Using this node, you can send HTTP(S) requests to external services or APIs. It allows you to connect Messcat with other systems and softwares

Ex: When a form is submitted in Messcat, you want to create a Google Calendar event

## How to use the HTTP request node

There are two ways to send a HTTP request in Messcat:

<aside>
💡

We suggest users to use the **HTTP Request Node** as it has lesser limitations compared to the **Action Node**

</aside>

### Through the **HTTP Request Node**

Step 1: Select “Choose next step” where you want use your HTTP request

![Screenshot 2024-11-01 at 1.12.30 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.12.30_PM.png)

Step 2: Select “HTTP Request” from the list

![Screenshot 2024-11-01 at 1.11.26 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.11.26_PM.png)

Step 3: Fill in the details of your HTTP Request

![Screenshot 2024-11-01 at 1.12.57 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.12.57_PM.png)

### Through the **Action Node**

Step 1: Select “Add Action” where you want use your HTTP request

![Screenshot 2024-11-01 at 1.08.43 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.08.43_PM.png)

Step 2: Within the Action Node, select the “HTTP Request” option

![Screenshot 2024-11-01 at 1.09.26 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.09.26_PM.png)

Step 3: Fill in the details of your HTTP Request, fire a test request, and click save after receiving a successful response

![Screenshot 2024-11-01 at 1.10.34 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.10.34_PM.png)

They both essentially perform the same tasks, but there are some slight differences as to how you can perform them:

| **HTTP Request Node** | **Action Node** |
| --- | --- |
| Can be edited once created | Cannot be edited once the test is successful and you leave the node (If you want to make changes later. you will have to delete this node and create a new one with the changes) |
| Can only be used after Triggers, buttons, and lists | Can be used after regular messages |
| Can be saved without passing any tests | HTTP Request can only be saved once you “Fire test request” and there is a successful response |

## How to fill the HTTP Request details?

Step 1: Input the URL of the API endpoint you want to send your HTTP Request to. You can insert any variables related to the contact or custom field data by inputting a { (curly bracket) and selecting your property

Step 2: Select a method. Currently, we only support **POST** and **GET** methods

![Screenshot 2024-11-01 at 1.15.51 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.15.51_PM.png)

Step 3: Enter your headers (Name and Values). You can use any variables here as well

<aside>
💡

We do not automatically add any headers such as “Content-Type” or “Accept”. If your API requires these, please add them manually in the headers section

</aside>

![Screenshot 2024-11-01 at 1.20.27 PM.png](How%20to%20use%20HTTP%20Request%20node/Screenshot_2024-11-01_at_1.20.27_PM.png)

Step 4: Fill in the body of your API request according to the third party’s documentation. You may use variables if you wish

Step 5(Only for Action Node): After setting up your HTTP Node, click “Fire Test Request”. Only once you receive a successful response, you can save your message flow