# kms-salemgmt-n8n
KMsCompany Sales Analytics and Management Automation - a personal venture for agrivet supplies and rice business 

# Sales Automation with n8n

## 📊 Overview
Automated sales logging system using n8n, Telegram Bot, and Google Sheets.

## 🤖 Workflows

### 1. Sales Logger (`workflows/sales-logger.json`)
- **Trigger:** Telegram message
- **Function:** Parse sales data, validate, log to Google Sheets
- **Frequency:** On-demand (daily ~6-8 PM)
- **Status:** ✅ Active

### 2. Weekly Analytics (Coming Soon)
- **Trigger:** Every Sunday 6 PM
- **Function:** Generate weekly sales report
- **Status:** 🚧 In Development

### 3. Monthly Analytics (Coming Soon)
- **Trigger:** 1st of each month, 6 PM
- **Function:** Generate monthly sales report
- **Status:** 📋 Planned

## 🔧 Setup

### Prerequisites
- n8n Cloud account
- Telegram Bot Token
- Google Sheets access
- OpenAI API key

### How to Restore Workflows
1. Download the workflow JSON file
2. Go to n8n Cloud → Settings → Import/Export
3. Click "Import from File"
4. Select the JSON file
5. Configure credentials

## 📅 Backup Schedule
Backups are created weekly (every Sunday) and stored in `backups/YYYY-MM-DD/`

## 🔒 Security
- Never commit credentials or API keys
- All sensitive data is stored in n8n Cloud credentials
- Use environment variables for configuration

## 📝 Last Updated
- **Date:** 2025-11-06
- **Version:** v1.0
- **By:** Ace Monte