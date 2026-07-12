# Smart Weather Alert Bot

An automated weather notification system built using n8n that fetches real-time weather data and sends condition-based alerts through Telegram.

## Features

- Automated daily weather monitoring
- Real-time weather data using Open-Meteo API
- Conditional weather classification
- Detects rain, extreme heat, cold, and pleasant conditions
- Dynamic Telegram notifications
- No weather API key required

## Workflow

Schedule Trigger → Open-Meteo API → Switch Node → Telegram Alert

The workflow runs automatically every day at 8:00 AM, retrieves current weather data for Hyderabad, evaluates the weather conditions, and sends the appropriate Telegram notification.

## Weather Conditions

- Rain → Rain alert
- Temperature ≥ 35°C → Extreme heat alert
- Temperature ≤ 18°C → Cold weather alert
- Otherwise → Pleasant weather notification

## Tech Stack

- n8n
- Open-Meteo API
- Telegram Bot API
- REST API
- JSON
- Workflow Automation

## Project Structure

- `workflow/` — Exported n8n workflow JSON
- `screenshots/` — Workflow and Telegram output screenshots

## Setup

1. Import the workflow JSON into n8n.
2. Configure your Telegram Bot credentials.
3. Add your Telegram Chat ID.
4. Activate the workflow.

## Security

Telegram credentials and bot tokens are not included in this repository.