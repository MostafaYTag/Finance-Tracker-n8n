💰 Finance Tracker — n8n

An automated personal finance tracking workflow built with n8n, Telegram, Notion, and AI.

The goal of this project is to make recording daily financial transactions simple: instead of manually entering every transaction into a spreadsheet or database, the user can simply send a message through Telegram, and the workflow automatically extracts the transaction details, classifies the transaction, and stores it in the appropriate Notion database.

🎯 Project Goal

The workflow is designed to automate personal finance tracking using natural language.

For example, the user can send messages such as:

دفعت 150 جنيه مواصلات كاش

or:

قبضت 12000 جنيه من الشغل

The workflow analyzes the message and automatically determines the relevant financial information before saving the transaction to Notion.

⚙️ How It Works
Telegram Message
       ↓
Telegram Trigger
       ↓
AI Information Extraction
       ↓
Transaction Type
   ↙           ↘
Expense        Income
   ↓              ↓
Categorization   Income Database
   ↓
Expenses Database
       ↓
      Notion

1. Telegram Trigger

The workflow receives the user's financial transaction through a Telegram bot.

2. Information Extraction

The AI extracts structured information from the natural-language message, including:

Amount

Transaction date

Transaction type

Category

Payment method

The workflow also understands Arabic and English numbers and common Egyptian Arabic date expressions.

3. Transaction Classification

The transaction is classified as either:

Income

Expenses

The workflow then routes the transaction to the appropriate path.

4. Expense Categorization

Expenses are automatically classified into:

Essential — food, transportation, rent, bills, healthcare, etc.

Luxury — restaurants, entertainment, games, vacations, personal shopping, etc.

Savings — money intentionally set aside as savings.

Investment — investments, professional courses, certifications, career education, and similar future-oriented spending.

5. Notion Database

The transaction is finally stored in the appropriate Notion database.

Income and expenses are maintained separately, making it easier to organize and analyze financial activity.

🧩 Workflow

🛠️ Technologies Used

n8n — Workflow automation

Telegram — User interface for sending transactions

OpenRouter — AI model connection

Notion — Financial data storage

AI Information Extraction — Converts natural-language messages into structured financial data

✨ Features

Natural-language transaction input

Arabic and English number recognition

Automatic date extraction

Automatic income/expense classification

Automatic expense categorization

Payment method detection

Telegram integration

Notion database integration

AI-powered information extraction

No manual data entry required

📌 Example
User Input

دفعت 400 جنيه أكل فيزا

Extracted Data
Amount: 400
Date: Current Date
Transaction Type: Expenses
Category: Essential
Payment Method: Visa


The workflow then automatically saves the transaction to the Expenses database in Notion.

📥 Installation

Download Finance_Tracker_notion.json.

Open your n8n instance.

Import the JSON workflow.

Configure your Telegram credentials.

Configure your OpenRouter credentials.

Connect your Notion account and select the required databases.

Activate the workflow.

Send a transaction through your Telegram bot.

Note: Credentials are not included in this repository. You must configure your own credentials inside n8n.

📄 Project Structure
Finance-Tracker-n8n/
│
├── Finance_Tracker_notion.json
├── workflow.png
└── README.md

🚀 Future Improvements

Possible future improvements include:

Monthly financial summaries

Spending analytics

Budget tracking

Telegram reports

Automatic monthly reports

Charts and dashboards

Multi-currency support

Recurring transaction detection

Financial goals tracking

👨‍💻 Project

Built as an automation project using n8n + AI + Telegram + Notion to simplify personal finance tracking.
