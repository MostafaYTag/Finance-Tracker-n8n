# 💰 Finance Tracker — n8n

An automated personal finance tracker built with n8n, Telegram, Notion, and AI.

Simply send a message to your Telegram bot describing an income or expense. AI extracts the transaction details, classifies them, and automatically saves everything to Notion.

## 🎯 Project Goal

Make daily finance tracking simple and effortless through natural-language messages.

Examples:

- دفعت 150 جنيه مواصلات كاش
- قبضت 12000 جنيه من الشغل

## ⚙️ How It Works

The workflow follows this process:

1. **Telegram Trigger:** Receives financial transactions.
2. **AI Information Extraction:** Extracts amount, date, transaction type, category, and payment method.
3. **Transaction Classification:** Determines whether the transaction is Income or Expense.
4. **Expense Categorization:** Classifies expenses into four categories.
5. **Notion Database:** Saves transactions into separate Income and Expenses databases.

The AI supports Arabic and English numbers, including common Egyptian Arabic date expressions.

## Workflow Preview

![Finance Tracker Workflow](./Workflow.png)

## Expense Categories

- **Essential:** Food, transportation, rent, bills, and healthcare.
- **Luxury:** Restaurants, entertainment, games, vacations, and personal shopping.
- **Savings:** Money intentionally set aside for savings.
- **Investment:** Investments, professional courses, certifications, and career education.

## 🛠️ Technologies Used

- **n8n** — Workflow automation.
- **Telegram** — User interaction.
- **OpenRouter** — AI model integration.
- **Notion** — Financial data storage.
- **AI Information Extraction** — Converts natural-language messages into structured data.

## ✨ Features

- Natural-language transaction input.
- Arabic and English number recognition.
- Automatic date extraction.
- Income and expense classification.
- Automatic expense categorization.
- Payment method detection.
- Telegram integration.
- Notion database integration.
- AI-powered information extraction.
- No manual data entry required.

## 📌 Example

**User Input:**

    دفعت 400 جنيه أكل فيزا

**Extracted Data:**

    Amount: 400
    Date: Current Date
    Transaction Type: Expense
    Category: Essential
    Payment Method: Visa

The transaction is automatically saved to the Expenses database in Notion.

## 📥 Installation

### 1. Get the Notion Template

[Open Notion Template](https://www.notion.com/templates/budget-planning)

Duplicate the template into your Notion workspace.

### 2. Import the Workflow

1. Download `Finance_Tracker_notion.json`.
2. Open your n8n instance.
3. Import the workflow JSON file.
4. Configure your Telegram credentials.
5. Configure your OpenRouter credentials.
6. Connect your Notion account and select the required databases.
7. Activate the workflow.
8. Send a transaction through your Telegram bot.

> **Note:** Credentials are not included in this repository. You must configure your own credentials inside n8n.

## 📄 Project Structure

    Finance-Tracker-n8n/
    │
    ├── Finance_Tracker_notion.json
    ├── Workflow.png
    └── README.md

## 🚀 Future Improvements

- Monthly financial summaries.
- Spending analytics and charts.
- Budget tracking.
- Telegram financial reports.
- Multi-currency support.
- Recurring transaction detection.
- Financial goals tracking.

## 👨‍💻 About

This project explores how AI and workflow automation can simplify personal finance management by combining natural-language processing with Telegram and Notion.
