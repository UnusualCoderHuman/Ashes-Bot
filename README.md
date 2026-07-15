# England Ashes Tracker Bot
A Twitter bot that tweets daily updates on England's Ashes drought.

## Origin
As an England cricket fan, I have actually never had the privilege of seeing England beat Australia/win the ashes. The last time they won was in 2015, nearly a dozen years ago! Having observed this I thought it would be fun to create a bot that tweets every day how many days it's been with the idea being if and when Eng ever do win the Ashes I can set it back to 0!

## What it tracks
Days since England last held the Ashes
Days since England last regained the Ashes

## How it works
Built in Python using Tweepy (Twitter API wrapper). A scheduled script runs daily, calculates the number of days elapsed since two hardcoded dates and posts the update automatically. A timestamp is included in each tweet to ensure uniqueness and avoid spam detection. API credentials are stored as environment variables for security.

## Scheduling
Runs daily via a GitHub Actions cron job, scheduled for 07:50 UTC. 
Note: GitHub Actions cron jobs can experience delays of several hours due to queue times on shared infrastructure.

## Limitations
Dates are hardcoded and will need updating if and when England win the Ashes
Tweet timing may vary due to GitHub Actions queue delays

## Follow the bot
https://x.com/englands_urn
