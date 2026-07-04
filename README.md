# Entity Relationship (ER) Diagram

## Description

The **RK Health ER Diagram** serves as the structural foundation of the system by illustrating how the major healthcare entities interact with one another. The core entities include **Patients, Appointments, Medications, Health Reports, AI Summaries, and Reminder Logs**. These entities work together to provide an efficient and centralized healthcare management platform.

The **Patient** entity is the primary component of the system. Each patient can have multiple **Appointments**, allowing users to schedule and manage doctor visits. Every appointment stores details such as the doctor's name, appointment date, time, visit notes, and appointment status.

The **Medication** entity manages prescribed medicines for each patient. It stores medication names, dosage information, reminder schedules, and associated contact details. Medication records are linked to patients, enabling the system to generate timely reminders through the Twilio SMS service.

The **AI Summary** entity stores patient-friendly healthcare summaries generated using the **Groq API** with the **Llama 3.3 70B Versatile** model. These summaries are created from appointment notes and visit information, helping patients better understand their medical conditions and follow-up recommendations.

The **Health Report** entity consolidates appointment history, medication schedules, reminder status, AI-generated summaries, and patient information into a comprehensive report. These reports provide users with an organized overview of their healthcare records.

The **Reminder Log** entity tracks all SMS reminders sent for appointments and medications. It records reminder status, delivery information, timestamps, and notification history, ensuring effective reminder management.

The relationships among these entities closely represent real-world healthcare workflows. A single patient can have multiple appointments, multiple medications, several AI-generated summaries, and multiple reminder records. Each appointment may generate one AI summary and contribute to one or more health reports. Medication schedules are connected to reminder logs to ensure timely notifications.

Overall, the ER diagram demonstrates the complete healthcare management workflow of RK Health by connecting patient records, appointments, medication management, AI-powered health summaries, cloud storage, SMS notifications, and reporting into a unified and scalable cloud-based system.
