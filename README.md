# Slack Channel Message Statistics Notebook

This Jupyter notebook provides comprehensive statistical analysis of messages from a specific Slack channel.

## Features

- **Message Volume Analysis**: Daily, hourly, and weekly activity patterns
- **User Activity Analysis**: Most active users, engagement metrics, and contribution patterns
- **Content Analysis**: Word clouds, message length distribution, and content characteristics
- **Engagement Metrics**: Reaction analysis, thread participation, and interaction patterns
- **Interactive Visualizations**: Plotly-powered interactive charts and dashboards
- **Data Export**: Export processed data to CSV files for further analysis

## Prerequisites

1. **Slack Bot Token**: You need a Slack bot token with the following permissions:
   - `groups:history` - Read message history
   - `groups:read` - Read channel information  
   - `users:read` - Read user profiles

2. **Channel ID**: The ID of the Slack channel you want to analyze (format: `C1234567890`)

## Setup

1. **Install Dependencies**:
   ```bash
   uv sync
   ```

2. **Get Your Slack Bot Token**:
   - Go to your Slack workspace settings
   - Create a new app or use an existing one
   - Add the required bot token scopes mentioned above
   - Install the app to your workspace
   - Copy the bot token (starts with `xoxb-`)

3. **Find Your Channel ID**:
   - Right-click on the channel name in Slack
   - Select "Copy Link"
   - The channel ID is the last part of the URL (e.g., `C1234567890`)

## Usage

1. **Configure Environment Variables**:
   Create a `.env` file in the project root:
   ```
   SLACK_BOT_TOKEN=your-slack-bot-token-here
   CHANNEL_ID=your-channel-id-here
   ```

2. **Run the Analysis**:
   - Execute all cells in order
   - The notebook will fetch messages and generate comprehensive statistics
   - Interactive visualizations will be displayed inline

3. **Customize Analysis**:
   - Adjust `DAYS_TO_ANALYZE` to change the time window
   - Modify visualization parameters as needed
   - Add custom analysis in new cells

## Output

The notebook generates:
- Basic channel statistics and metrics
- Activity timeline and pattern visualizations
- User engagement and contribution analysis
- Word clouds and content insights
- Interactive dashboards with Plotly
- Optional CSV exports for further analysis

## Extending the Analysis

The notebook provides a foundation for more advanced analysis:
- Sentiment analysis of messages
- Topic modeling and trend analysis
- Network analysis of user interactions
- Seasonal pattern detection
- Custom engagement scoring 