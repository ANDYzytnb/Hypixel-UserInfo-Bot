# Hypixel User Info Bot

## Project Overview

This bot operates on the Tencent QQ platform, providing Hypixel server game information to users. It offers a convenient way for players to access their stats and performance data across various Hypixel game modes. This project is not affiliated with or endorsed by Hypixel.

## Key Features

- Player level and general Hypixel information
- Detailed game mode statistics (Bedwars, Skywars, Duels, Skyblock)
- Multilingual support (currently Chinese, with plans for expansion)
- Real-time data retrieval and display

## API Usage and Compliance

- Estimated daily API requests: Approximately 3,000
- Strict adherence to Hypixel's API terms of service and usage guidelines
- Implementation of robust caching to minimize API calls:
  - Player data cached for 30 minutes
  - Game mode specific data cached for 15 minutes
  - Server status updates cached for 5 minutes
- Rate limiting to prevent API abuse
- No continuous polling or automated data collection at scale
- No commercial use or monetization of API data
- Single API key used for this project only

## Data Handling and Privacy

- User data is processed in real-time and not stored permanently
- No de-anonymization of players using Hypixel's nick feature
- No tracking of specific players or ranks

## Usage

The bot responds to the following commands:

- `/hyp [username]`: Retrieves general Hypixel player information
- `/bw [username]`: Displays Bedwars statistics
- `/sw [username]`: Shows Skywars data
- `/duel [username]`: Provides Duels information
- `/sb [username]`: Fetches Skyblock details

## Usage Examples

Here are some examples of the bot's output (translated to English for clarity):

```
/hyp Dream

Hypixel Player Data:
Player Name: Dream
Level: 80.06
Karma: 4017370
Player Language: Query Failed
First Login: 2013-07-22T13:42:36
Last Login: 2023-06-04T01:29:59.436
Last Logout: 2023-06-04T01:46:35.044
Current Status: Offline

/bw Dream

Bedwars Information:
Level: 51.1
Coins: 264964
Beds Broken: 1039
Total Games: 1311
Wins/Losses: 408/874 WLR: 0.47
Kills/Deaths: 6785/3738 KDR: 1.82
Final Kills: 2100
```

## Technical Implementation

- Developed using Python, leveraging the Hypixel API for data retrieval
- Integrates with the Tencent QQ platform using appropriate SDKs
- Asynchronous programming for efficient handling of multiple requests
- Robust error handling and logging for stability
- API key securely stored and not shared or distributed

## Compliance and Ethics

- Designed to comply with all Hypixel API policies and terms of service
- Does not provide any unfair advantages to players
- Enhances the Hypixel gaming experience without compromising game integrity
- Regular updates to ensure continued compliance with evolving API policies

## Future Development Plans

- Expansion to other messaging platforms
- Addition of more game modes and detailed statistics
- Implementation of leaderboards and comparative player stats
- Continuous improvement based on user feedback and Hypixel community needs

This project aims to provide a useful tool for Hypixel players while respecting the game's integrity and API usage guidelines. We are committed to responsible API usage and will promptly adapt to any policy changes to ensure ongoing compliance.
