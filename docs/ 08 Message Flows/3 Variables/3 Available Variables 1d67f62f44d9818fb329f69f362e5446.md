# Available Variables

Article Description: What variables are available to me?


The list is constantly growing! However, this document will cover the variables  available at the time of writing, and how to access them.

Note: the variables available to you vary with whether you’re using an app/conditions or sending a message

## Variables in Messages

1. From the contact, you can use the:
    - name
    - phone number
    - custom fields
2. If the message follows a trigger, or an app — you can use the data outputted from there as well. In the example below, we use the output from the AI chatbot app to power the response message
    
    ![Screenshot 2024-07-03 at 1.30.36 PM.png](Available%20Variables/Screenshot_2024-07-03_at_1.30.36_PM.png)
    

## Variables in Apps/Conditions

1. Apps & conditions can access the following properties in the contact:
    1. Name
    2. Phone number
    3. Messages sent/received
    4. Assignee
    5. Tags
    6. Ticket stages, details
    7. Custom fields 
2. Can also access the output from the previous app. Here you see the output of the AI chatbot feeding into a condition node to check whether the chatbot successfully answered the question & then conditionally changing the answer it returns.
    
    ![Screenshot 2024-07-03 at 3.05.24 PM.png](Available%20Variables/Screenshot_2024-07-03_at_3.05.24_PM.png)
    
    ![Screenshot 2024-07-03 at 3.05.40 PM.png](Available%20Variables/Screenshot_2024-07-03_at_3.05.40_PM.png)
    
3. Can also access flow variables. You can read about flow variables here. In the example below we check if the assignee messaging us has been assigned to the person referenced in the flow variable “CS Member1”
    
    ![Screenshot 2024-07-03 at 3.06.53 PM.png](Available%20Variables/Screenshot_2024-07-03_at_3.06.53_PM.png)