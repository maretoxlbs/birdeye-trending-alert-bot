Birdeye Real-Time Trending Token Alert Bot
🚀 Overview
This repository contains an autonomous monitoring tool built with n8n that interfaces with the Birdeye Intelligence API. The bot tracks the most "Trending" tokens on the Solana blockchain in real-time and dispatches high-signal alerts to a private Telegram channel.

🧠 Intelligence & Data Strategy
The workflow is engineered to filter through thousands of on-chain data points to surface only the highest-momentum assets.

Endpoint Utilization: Primarily utilizes the /defi/token_trending endpoint to fetch assets with the highest search and price momentum.

Data Formatting: The bot processes raw JSON payloads to extract key financial metrics: Name, Symbol, Liquidity, and 24h Volume.

Dynamic Linking: Every alert includes an automated deep link to the Birdeye token terminal using the specific contract address.

🛠️ Technical Stack
Orchestration: n8n (Advanced Workflow Automation).

Data Source: Birdeye Data Service (BDS) API.

Network focus: Solana (Low latency, high frequency).

Notification Layer: Telegram Bot API (Markdown-formatted alerts).

💡 Key Features
Automated Polling: Configured with a cron-schedule to ensure 24/7 market surveillance.

Signal-to-Noise Optimization: Limited to the Top 5 trending assets to avoid information overload.

Infrastructure Ready: Designed to be deployed on a server or locally for immediate alpha discovery.
