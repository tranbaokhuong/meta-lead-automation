# Meta Lead Automation

Automatically receives Facebook messages and comments, uses AI (Gemini) to classify customers,
saves them to a Notion CRM, and notifies the sales team via Telegram.

## Workflows
| # | Name | Function |
|---|------|----------|
| 02 | Meta Messenger Intake | Receives Messenger messages, merges consecutive messages, reads images, classifies the lead and replies |
| 03 | Meta Sale Actions | Sales taps "Take lead" on Telegram, and the bot pauses |
| 04 | Meta Comment Polling | Scans comments every minute, records leads, and replies to comments |

## Tech Stack
n8n, Meta Graph API, Google Gemini, Notion API, Telegram Bot

## Setup
1. In n8n, choose Import from file and load each file in the `workflows/` folder.
2. Create credentials: Notion, Telegram, Google Gemini, Meta Page Access Token.
3. Replace the `YOUR_...` placeholders with your own values.
4. Create the Notion database with the columns the workflows use.
