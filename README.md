# AI Lead Capture & Nurture (n8n)

AI-powered lead capture for real estate agents. Filters spam, scores leads as hot, warm, or cold, sends a personalized reply within seconds, and follows up after 1 day.

![Workflow](workflow.png)

## How it works

1. **Form submission:** a lead submits their name, email, and message
2. **AI Agent:** OpenAI checks for spam, scores the lead, summarizes their request, and drafts a personalized reply
3. **Spam filter:** junk goes to a separate spam sheet, real leads continue
4. **Save lead:** saved to Google Sheets with score and summary
5. **Notify me:** instant email alert to the agent
6. **Auto-reply:** personalized AI reply sent to the lead within seconds
7. **Follow-up:** friendly nudge sent after 1 day

## Built with

n8n · OpenAI · Google Sheets · Gmail

## Setup

1. Import `Lead Capture & Nurture.json` into n8n
2. Connect your own OpenAI, Google Sheets, and Gmail credentials
3. Create a Google Sheet with columns: Name, email, message, lead_score, intent
4. Publish the workflow and use the production form URL
