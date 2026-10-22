# WhatsApp Activity Dashboard

A local dashboard for exploring activity from one WhatsApp account. It summarizes counts and timing across conversations while making gaps in collection visible. It does not send WhatsApp messages.

The application runs on the owner's computer with Docker Compose and SQLite. Collection uses a linked WhatsApp Web session. The owner controls whether each conversation retains message text locally, keeps only activity metadata, or is excluded.

## Main views

These screenshots use invented names and activity data. They were captured with synthetic API responses, not from a live account.

### Overview

See message totals, active conversations, activity periods, response time, weekly trends, and a weekday-by-hour heatmap. A coverage notice warns when collection may be incomplete.

![Synthetic dashboard overview with activity totals, weekly chart, top conversations, and heatmap](images/overview.png)

### Conversation detail

Choose a conversation to see its trend. Group detail separates participants and shows message, word-count, and voice-duration totals, including activity after a chosen local time.

![Synthetic group detail with participant table, activity trends, and voice-duration charts](images/group-detail.png)

### Time patterns

Compare sent and received activity by local weekday and hour. The dashboard also provides voice activity and collector-health views.

![Synthetic sent and received weekday-by-hour heatmaps](images/time-patterns.png)

### Ask Activity

Ask for rankings and other numeric summaries within a selected group or participant scope. Exact filtering and calculations run locally; the screen shows how it interpreted the question.

![Synthetic Ask Activity result with selected scope, interpreted filters, ranking, and exact values](images/ask-activity.png)

## About this public repository

It contains only this README and four synthetic screenshots. Application source, configuration, development history, and personal data stay private. This repository is an overview, not an installable release.
