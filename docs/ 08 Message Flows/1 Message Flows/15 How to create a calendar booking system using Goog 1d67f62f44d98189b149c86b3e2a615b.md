# How to create a calendar booking system using Google Calendar

Use “Generate Calendar slots” and “Calendar” to create your own booking system


[[https://drive.google.com/file/d/16yTYklpwQIyl8babAw_nGTNr7EyTEBAQ/view?usp=sharing](https://drive.google.com/file/d/16yTYklpwQIyl8babAw_nGTNr7EyTEBAQ/view?usp=sharing)](https://drive.google.com/file/d/16yTYklpwQIyl8babAw_nGTNr7EyTEBAQ/view?usp=sharing)

The Calendar apps allow you to integrate a Google Calendar booking system for your business through message flows. There are 2 nodes available to help you achieve this:

1. **Generate Calendar Slots -** The Generate Calendar Slots app will return a list of available time slots on the date your client wants to book an appointment
2. **Calendar -** The Calendar app will create the booking and send you and your client a google invite based on the date and time they select for the booking

These apps allows you to:

- Integrate your google account with Messcat to
- Set the days when you want to accept bookings. Ex: Monday to Friday
- Set what time you want to start and end your bookings. Ex: 9:00 to 18:00
- Set the duration of your bookings. Ex: 1 hour
- Add a location of your meeting(if any). If no location is added it will automatically create and schedule a google meet

---

### Steps to create the booking system:

Step 1: Go to Automations > Message Flows > Create new flow

Step 2:  Create a starting message requesting your client to specify the date when they want to setup an appointment. Ex: “Please enter the date in DD MM format. For example, 2 September.”

> The date The date **MUST** be in **DD MM** format. The flow will not work otherwise
> 

Step 3: Add a “User Input” and save the response to a “Date” type custom field

Step 4 (Optional): Ask your user to input their email ID if you want to send them an invite to the appointment

Step 5 (Optional):  Add a “User Input” and save the response to a “Text” type custom field

Step 6: Add and setup your “General Calendar Slots” app 

1. Click on “Add Integration”(if you don’t already have one) or select the calendar account you want to use 
2. In the “Date” input,  add the custom field where you saved your Date in Step 3 by typing {{**field_name**}}
    
    > Replace **field_name** with the name of your custom field
    > 
3. Input the start and end timings of your booking system, along with the duration of each appointment
4. Select the the days when you want to take in bookings

Step 7: Click on “Choose next step” and select message. You can use the output of the General Calendar Slots app by using this variable: {{Formatted Slots}} 

Ex: 

> Select your appointment timings from these slots:
{{Formatted Slots}}
> 

Step 8: Add a “User Input” and save the response to a “Text” type custom field

Step 9: Add and setup your “Calendar” app

1. Click on “Add Integration”(if you don’t already have one) or select the calendar account you want to use 
2. Setup the Date, Bookings Start, Bookings End, and Booking Duration with the same details as you did in Step 6
    
    > Make sure the details match in both the calendar nodes
    > 
3. In the “Contact Name”, add the name of your client by typing {name}
4. In the “Contact Email”, add the custom field where you saved your Email in Step 5 by typing {{**field_name**}}
5. (Optional) Add a location for your meeting if it is a physical appointment

Step 10: Send a confirmation message with the Google Calendar link using the variable {{Message}}