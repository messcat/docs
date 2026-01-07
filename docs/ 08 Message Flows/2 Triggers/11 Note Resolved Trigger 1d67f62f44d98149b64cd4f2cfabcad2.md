# Note Resolved Trigger

Article Description: Learn how to use the “Note Resolved” Trigger!


<aside>
💡

The Note Resolved trigger is activated every time any note has been resolved

</aside>

## Overview

![Screenshot 2025-03-11 at 1.06.30 PM.png](Note%20Resolved%20Trigger/Screenshot_2025-03-11_at_1.06.30_PM.png)

The **Note Resolved** trigger activates when a previously added note is marked as resolved. This is useful for tracking completed tasks, notifying team members, and updating external systems based on note resolutions.

## Use Cases

- **Internal Alerts**: Notify relevant team members when a note is resolved.
- **Task Management**: Mark tasks as complete in external project management tools.
- **CRM Updates**: Change the status of CRM entries based on note resolution.
- **Automated Follow-Ups**: Trigger a follow-up message or email when a note is resolved.

## Trigger Conditions

Customize the trigger using the following conditions:

- **Resolved by**: Activate when a specific user or role resolves the note.
- **Related Item Status**: Trigger only if the associated conversation, ticket, or CRM entry is in a certain state (e.g., open, pending, closed).
- **Resolution Tags**: Only trigger for notes marked with a particular tag upon resolution.
- **Resolved At**: Trigger based on the timestamp of when the note was resolved.

## Example workflow

### Scenario: Notify a Supervisor When a Critical Note Is Resolved

1. **Trigger**: A note is marked as resolved.
2. **Condition**: If the note contains “urgent” or “high priority.”
3. **Action**: Send an email notification to the supervisor.