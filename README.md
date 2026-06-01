# Agentic Ai management system (n8n)

An AI-powered management system, The assistant understands natural language requests and automatically uses the appropriate tools to manage calendars, emails, expenses, notes, tasks, and research.

---

## Features

### AI Agent

* Powered by Gemini 2.5 Flash
* Natural language understanding
* Multi-step reasoning
* Automatic tool selection
* Workflow orchestration

### Google Calendar Tool

* Create Events
* Get Event
* Get Multiple Events

Examples:

* Schedule a meeting tomorrow at 10 AM
* Show my upcoming meetings
* Get today's calendar events

### Gmail Tool

* Send Email
* Get Email
* Get Multiple Emails

Examples:

* Send an email to [example@gmail.com](mailto:example@gmail.com)
* Show my latest emails
* Get emails from a specific sender

### Expense Tracking Tool

* Create Expense Entry
* Get Expense Records
* Expense Calculator

Examples:

* Add ₹500 spent on groceries
* Show my expenses
* Calculate total monthly expenses

### Notes Tool

* Create Notes
* Get Notes

Examples:

* Save a note about startup ideas
* Show my saved notes

### Task Management Tool

* Create Tasks
* Get Tasks
* Delete Tasks

Examples:

* Create a task to complete project documentation
* Show all pending tasks
* Delete completed tasks

### Google Tool

* Google information retrieval
* Research assistance
* Knowledge gathering


### Webhook Interface

* Receives user requests
* Triggers workflow execution
* Connects external applications

### Local Storage

* Stores workflow data
* Maintains assistant context
* Saves notes, tasks, and records

---

## Architecture

```text
User Request
      │
      ▼
Webhook Trigger
      │
      ▼
Gemini 2.5 Flash AI Agent
      │
      ├── Calendar Tool
      │     ├── Create Event
      │     ├── Get Event
      │     └── Get Many Events
      │
      ├── Gmail Tool
      │     ├── Send Email
      │     ├── Get Email
      │     └── Get Many Emails
      │
      ├── Expense Tool
      │     ├── Create Expense
      │     ├── Get Expenses
      │     └── Calculator
      │
      ├── Notes Tool
      │     ├── Create Note
      │     └── Get Notes
      │
      ├── Task Tool
      │     ├── Create Task
      │     ├── Get Tasks
      │     └── Delete Task
      │
      └── Google Search
              │
              ▼
        Local Storage
              │
              ▼
        Response to User
```

---

## Technology Stack

* n8n
* Gemini 2.5 Flash
* Google Calendar API
* Gmail API
* Google Sheets API
* Google OAuth 2.0
* Webhooks
* Local Storage

---

## Available Operations

| Tool     | Operations                     |
| -------- | ------------------------------ |
| Calendar | Create, Get, Get Many          |
| Gmail    | Send, Get, Get Many            |
| Expenses | Create, Get, Calculator        |
| Notes    | Create, Get                    |
| Tasks    | Create, Get, Delete            |
| Research | Search & Information Retrieval |

---

## Setup

### Prerequisites

* Docker
* n8n
* Google Cloud Project
* Gemini API Key
* Gmail API Enabled
* Google Calendar API Enabled
* Google Sheets API Enabled

### Environment Variables

```env
GEMINI_API_KEY=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
N8N_HOST=
N8N_PORT=
```


## Future Enhancements

* Voice Assistant Integration
* WhatsApp Integration
* Slack Integration
* Vector Database Memory
* Multi-Agent System
* Analytics Dashboard
* Document Processing

---


## License

MIT License

## Author

Dhiti Varma 
