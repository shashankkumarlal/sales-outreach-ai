# Sales Outreach AI Agent

An AI-powered agent to automate personalized cold emails and follow-ups for sales outreach.  
Built using LangChain with Groq-hosted LLaMA 3, it sends personalized emails, schedules follow-ups, tracks progress, and updates leads in a CSV file.

## Features

- Reads leads from a CSV file (`leads.csv`)
- Sends personalized cold emails based on lead info (name, company, pain points, product)
- Schedules and sends polite follow-up emails automatically
- Tracks email progress with step, last_email, followup_date columns
- Logs last replies for manual or AI-based customer support follow-up
- Supports different tones for emails (friendly, professional, casual)
- Easy to run on Google Colab or local machine

## How to Use

1. Prepare `leads.csv` with columns: `name,email,company,product,pain_points,tone`
2. Run the main Python script or notebook
3. Enter your Groq API key and Gmail credentials
4. The agent sends emails and updates the CSV with progress and follow-up dates
5. Run a reply-checker script (optional) to update replies in CSV

## Requirements

- Python 3.8+
- Packages: `langchain`, `langchain_groq`, `pandas`, `python-dotenv`
- Gmail App Password for SMTP email sending

## Setup

```bash
pip install langchain langchain_groq pandas python-dotenv
