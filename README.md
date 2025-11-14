# n8n-lead-generation
An n8n automation that qualifies new leads from Gmail using a Gemini AI model. It categorizes leads by intent and either adds them to a Google Sheet CRM or sends an automated follow-up email.
# n8n Lead Qualification Workflow

This workflow automates the process of qualifying new leads that arrive via email. It uses an AI model to categorize the lead's intent and takes different actions based on the result.

## Features

-   Triggers on new Gmail messages.
-   Uses Gemini AI to extract lead details (name, email, company).
-   Uses Gemini AI in a subflow to categorize intent (High, Medium, Low).
-   Adds High-Intent leads to a Google Sheet.
-   Sends an automated reply to Medium/Low-Intent leads.
-   Logs all leads to a master Google Sheet.
-   Sends a Slack notification for every new lead.

## How to Use

1.  Download the `workflow.json` file from this repository.
2.  In your n8n instance, import the workflow from the file.
3.  Create new credentials for Gmail, Google Sheets, Gemini AI, and Slack.
4.  Update the nodes in the workflow to use your new credentials.

## 🚀 Demo Video

Click the image below to watch a full demo of the lead-generation in action:

[![Demo Video](https://github.com/Ayyankidwai/n8n-lead-generation/blob/e7c92adb8b683191990b9c8909b3511686028cb1/n8n-workflow.png)]
