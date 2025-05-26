# GokiteAI Chat Automation Bot

Automates interactions with GokiteAI agents to earn XP points automatically.

## Features

- Multi Account Support
- Auto Chat with AI Agents (Professor, Crypto Buddy, Sherlock)
- Automatic Receipt Submission
- Proxy Support to avoid rate limits
- Easy Configuration

## Requirements

- Node.js v18+ LTS [Download](https://nodejs.org/dist/v18.20.6/node-v18.20.6-x64.msi)
- GokiteAI wallet addresses
- Proxy (Optional). Recommended: [Cherry Proxy](https://center.cherryproxy.com/Login/Register?invite=029ad2d3)

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/0xSeijuro/gokiteai2-bot.git
   cd gokiteai2-bot
   ```

2. Install Dependencies:

   ```sh
   npm install
   ```

3. Create a `proxy.txt` file in the root directory and add your proxies (one per line) (Optional).

   ```
   http://user:pass@host:port
   http://user:pass@host:port
   http://user:pass@host:port
   ```

4. Create an `accounts.txt` file and add your GokiteAI wallet addresses (one per line):

   ```
   0x1234567890abcdef1234567890abcdef12345678
   0xabcdef1234567890abcdef1234567890abcdef12
   0x9876543210abcdef9876543210abcdef98765432
   ```

## How It Works

The bot automatically:

1. Logs into GokiteAI using your wallet addresses
2. Chats with three different AI agents:
   - **Professor** - Asks educational questions about blockchain technology
   - **Crypto Buddy** - Asks about cryptocurrency market information
   - **Sherlock** - Asks about blockchain transaction analysis
3. Submits receipts for each interaction to earn XP points
4. Tracks your points accumulation

## Usage

1. Run the bot:

```sh
node .
```

2. The bot will automatically:

   - Process each address in accounts.txt
   - Use proxies if available
   - Log in to each account
   - Chat with all three AI agents
   - Submit receipts for each interaction
   - Display earned XP points

3. Monitor the console for real-time progress updates including chat previews

## Configuration Options

You can customize the bot behavior by editing the following files:

- **src/main/gokiteV2bot.js** - Modify agent prompts and behavior
- **src/utils/logger.js** - Adjust logging format and verbosity
- **src/index.js** - Configure runtime parameters

## Stay Connected

- Channel Telegram : [Telegram](https://t.me/elpuqus)
- Channel WhatsApp : [Whatsapp](https://whatsapp.com/channel/0029VavBRhGBqbrEF9vxal1R)
- Discord : [Discord](https://discord.com/invite/uKM4UCAccY)

## Donation

If you would like to support the development of this project, you can make a donation using the following addresses:

- Solana: `FdHsx8He55QgRCSv6NMEpFfkjXFsXFEeWEpJpo7sUQZe`
- EVM: `0x406de5ec09201002c45fdd408ab23159cd12fa3e`
- BTC: `bc1prze475lgalevngrhwq6r9wyng3rl3zskyru4rn4k6j8kwzmmczmqcd7u7y`

## Troubleshooting

- **Authentication Issues**: If you encounter login problems, make sure your wallet addresses are correct
- **Rate Limiting**: If you see rate limit errors, try using proxies or increasing the delay between requests
- **Response Parsing Errors**: These usually resolve on retry; the bot has built-in retry mechanisms

## Disclaimer

This tool is for educational purposes only. Use it at your own risk. Using automation tools may be against the terms of service of some platforms. Please ensure you are compliant with GokiteAI's terms of service.
