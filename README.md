# News Monitoring Automation

I built this n8n workflow to monitor an RSS news feed, detect new articles, and use AI to classify and summarize the news in Arabic before saving and sending updates.

<img width="762" height="216" alt="News Monitoring Automation workflow demo" src="https://github.com/user-attachments/assets/2386670c-5bff-43bd-b4b5-ea763f1734f8" />

## How it works

1. The workflow checks an RSS feed every three hours.
2. It retrieves the previously saved news links from Google Sheets.
3. JavaScript filters out articles that have already been recorded.
4. Claude summarizes each new article in Arabic and assigns it a suitable category.
5. The news information is saved to Google Sheets and a Telegram message is sent with the article title, category, summary, and link.

## Main features

- Scheduled RSS news monitoring.
- Duplicate article filtering.
- AI-generated Arabic summaries.
- Automatic news categorization.
- Google Sheets storage and Telegram notifications.

## Technologies

n8n, RSS Feed Read, Anthropic Claude, Google Sheets, JavaScript, and Telegram.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Anthropic, Google Sheets, and Telegram credentials, then add your preferred RSS feed and connect your news tracking sheet.
