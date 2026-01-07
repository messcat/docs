# What are triggers?



## What are Triggers?

Triggers are a powerful functionality within message flows that enable automated responses and workflows, streamlining communication and operational processes. By setting specific conditions or events as triggers, you can automatically send messages or initiate complex workflows without manual intervention.

Triggers have the power to replace all automation modules (broadcasts, keyword replies, offline bot, shop notifications) and much more

![Untitled](What%20are%20triggers/Untitled.png)

## Types of triggers

- **Incoming Message**: Activated whenever a new message is received.
- **Outgoing Message**: Activated whenever there is a new message sent.
- **New Chat**: Activated whenever the first message is sent or received in a new chat.
- **Contact Updated**: Triggered when contact information is modified.
- **Contact Added**: Initiated upon the addition of a new contact.
- **Ticket Updated**: Activated whenever there is a change in a ticket.
- **Ticket Created**: Activated whenever there is a new ticket created.
- **Broadcast**: Facilitates sending broadcast messages to multiple contacts simultaneously.

## What is Trigger Frequency?

![Screenshot 2025-04-09 at 1.26.50 PM.png](What%20are%20triggers/Screenshot_2025-04-09_at_1.26.50_PM.png)

**Trigger Frequency** lets you control how often an automation (like an Incoming Message flow) can be triggered **per contact** within a set time window.

This helps prevent spammy behavior or repeated automation responses when a contact sends multiple messages in a short period.

For example:

> If you set it to “Once per 30 seconds”, each contact can only trigger this automation once every 30 seconds—no matter how many messages they send during that time.
>