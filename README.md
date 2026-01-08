# Calendly to ClickUp Integration Workflow (Make.com)

## 🛠️ Workflow Logic
The automation follows a strict trigger-action sequence:
1.  **Trigger (Calendly):** Activates immediately when a new invitee books an appointment.
2.  **Data Fetching:** Retrieves all attendee information, including custom questions (like Phone Number).
3.  **Action (ClickUp):** Creates a new task in the **"Meetings"** list within the **"Testing"** space.
![Uploading image.png…]()

## 📊 Data Mapping & Configuration
I have configured the following fields to be dynamically populated:
- **Task Name:** Concatenated `Invitee First Name` and `Invitee Last Name`.
- **Email:** Mapped to a dedicated ClickUp Email field.
- **Phone Number:** Captured from Calendly’s custom question fields.
- **Meeting Date:** Synchronized with ClickUp’s Date field (Asia/Karachi Timezone).
- **Appointment Time:** Detailed in the task metadata for precise scheduling.

## 📋 Features
- **Zero Latency:** Uses Webhook logic for instant task creation.
- **Data Integrity:** Ensures all custom fields are validated before being pushed to ClickUp.
- **Scalable:** Can be easily extended to include multiple team members or different meeting types.

---
