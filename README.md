# n8n WelcomeBot

Welcome to the **n8n WelcomeBot** project!  

This automation system captures user data from a contact form, processes it using an AI model, and then automatically sends a personalized welcome email to the user’s Gmail account.

This project leverages **n8n**, an open-source automation tool, and **Google Gemini Chat**, an AI model, to create a seamless experience for new users who submit a form.

---

## ✨ Features

- **Contact Form Integration**: Users can submit a contact form with their details.
- **AI-Generated Welcome Message**: The AI agent processes the form data and generates a personalized welcome email.
- **Automated Email Sending**: The system sends the welcome message to the user's Gmail using the Gmail API.

---

## 🔁 Workflow Overview

This workflow consists of several key stages that automate the process of sending a welcome email:

### 1. Webhook Listener
- A **Webhook node** captures data submitted via the contact form (name, email, age, gender, country).

### 2. AI Agent
- The data is processed by an **AI agent**, which uses **Google Gemini Chat** to generate a personalized welcome message based on the form data.

### 3. Send Email via Gmail
- Once the AI generates the response, a **Gmail node** sends the personalized message directly to the user’s Gmail account.

### Workflow Diagram:
![Workflow Diagram](https://github.com/Sonu-kumawat-ai/n8n-WelcomeBot/blob/main/images/image2.JPG)

---

## 📝 Contact Form Submission

The contact form includes the following fields:

- **Name**: The user's full name (e.g., `Sonu Kumawat`)
- **Email**: The user’s email address (e.g., `kumawatsonu086@gmail.com`)
- **Age**: User’s age
- **Gender**: "Male" or "Female"
- **Country**: Country dropdown (e.g., "India")

### Example Form UI:
![Contact Form](https://github.com/Sonu-kumawat-ai/n8n-WelcomeBot/blob/main/images/image1.JPG)

When the user submits the form, the data is sent via POST to the webhook endpoint in n8n.

---

## 📧 Automated Welcome Email

After the form is submitted:
- The AI agent generates a message.
- The message is sent to the user via the **Gmail API**.

### Example Email Content:

![Email](https://github.com/Sonu-kumawat-ai/n8n-WelcomeBot/blob/main/images/image3.jpg)

---

## How to Run

- Clone the repository:
```bash
git clone https://github.com/Sonu-kumawat-ai/n8n-WelcomeBot.git
```

- **Set up n8n**: Follow the n8n documentation to install and configure n8n on your local machine or server.

- **Configure Webhook**: Set up the webhook URL to capture form submissions and trigger the workflow.

- **Set up Gmail API**: Connect the Gmail API in n8n to send automated emails.

- **Run the Workflow**: Once everything is set up, execute the workflow and test the form submission to see the automated email being sent.

---

## Technologies Used

- **n8n**: Open-source workflow automation tool.

- **Google Gemini Chat**: AI model to generate personalized messages.

- **Gmail API**: To send automated emails.
