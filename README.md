# News Monitoring Automation

An n8n workflow that periodically reads an RSS news feed, filters out previously recorded links, uses AI to classify and summarize new articles in Arabic, saves records to Google Sheets, and sends Telegram alerts.

## How it works

1. A schedule trigger runs every three hours.
2. The workflow fetches articles from an RSS feed and retrieves previously recorded news links from Google Sheets.
3. JavaScript filters out articles that have already been stored.
4. An AI agent classifies each new article and writes a short Arabic summary.
5. The processed article information is saved to Google Sheets and sent through Telegram.

## Technologies

- n8n
- RSS feeds
- Google Sheets
- Anthropic Claude
- JavaScript
- Telegram

## Setup

1. Import workflow.json into n8n.
2. Configure Google Sheets, Anthropic, and Telegram credentials.
3. Choose the RSS source and connect your own news log sheet.
4. Test the workflow with a small batch before enabling the schedule.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
