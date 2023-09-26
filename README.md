# Twitter Auto-Tweet Script

This script is designed to automate tweets on Twitter using the Twitter API. It sends out daily tweets at 9:00 AM, incrementing a counter in the message each day, and requests Elon Musk to gift the bot a new Tesla.

## Prerequisites

Before using this script, make sure you have the following:

1. **Node.js**: This script is written in JavaScript and requires Node.js to run. You can download it [here](https://nodejs.org/).

2. **Twitter API Credentials**: You'll need Twitter API credentials, including API keys and access tokens, to interact with Twitter.

3. **Twitter Developer Portal**: These API credentials are created in the [Twitter Developer App](https://developer.twitter.com/en/portal/dashboard) and are tailored to your account. 

4. **Twitter Developer Portal Tutorial**: [Timestamps: 0:00 - 4:30](https://www.youtube.com/watch?v=fBFQMp0m41E).

## Installation

1. Clone this repository to your local machine.

2. Install the required npm packages by running the following command: npm install

3. Create a `.env` file in the same directory as the script and add your Twitter API credentials. You can use the provided `.env.example` as a template:

TWITTER_API_KEY=your_api_key

TWITTER_API_SECRET_KEY=your_api_secret_key

TWITTER_ACCESS_TOKEN=your_access_token

TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret


## Usage

To use the script, follow these steps:

1. Run the script with Node.js using the following command: node script.js

2. The script will automatically send a tweet at 9:00 AM each day, starting with "Day 1 asking for @elonmusk to gift me a new Tesla!" and incrementing the day counter in the message each day.

## Cron Job Schedule

The script uses a Cron Job with the following schedule: 0 0 9 * * *

This schedule translates to running the script at 9:00 AM every day.

This schedule can be easily changed by changing the expression. 

A good website that makes it easier to choose the right time expression is [crontab.guru](https://crontab.guru/).

## Troubleshooting

If you encounter any issues or errors while running the script, check the following:

- Ensure that your Twitter API credentials are correctly set in the `.env` file.

- Make sure you have the required dependencies installed by running `npm install`.

- Check your internet connection, as the script requires an internet connection to access the Twitter API.
