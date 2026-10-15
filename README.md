# SejalxBomber Bot

A Python Telegram bot built with **aiogram 3** and **aiohttp**, featuring user management, admin controls, a credit system, referrals, and Firebase integration.

## Features

- Telegram bot interface using inline keyboards
- User registration and management
- Admin and super-admin controls
- User credits and credit transfers
- Referral rewards
- Pricing and payment-link configuration
- Firebase endpoint management
- Activity statistics and history
- Asynchronous operation using Python's `asyncio`

## Requirements

- Python 3.11 or newer
- A Telegram bot token from [@BotFather](https://t.me/BotFather)
- Authorized access to any Firebase projects used by the application

## Dependencies

Create a file named `req.txt` containing:

```text
aiogram
aiohttp
```

Install the dependencies:

```bash
python3 -m pip install -r req.txt
```

A virtual environment is recommended.

## Installation

1. Download or clone the project.
2. Open a terminal in the project directory.
3. Install the dependencies listed in `req.txt`.
4. Review the configuration values in the Python source code.
5. Configure the Telegram bot token, owner identifiers, and other required settings.
6. Verify that Firebase endpoints are authorized and configured correctly.
7. Run the application in a controlled test environment.

## Running the Bot

Run the Python file using the Python interpreter:

```bash
python3 "@SejalxBomber_Bot.py"
```

The bot uses Telegram long polling to receive updates.

## Configuration and Data

Review the source code for the required configuration constants and data-file paths before launching the application. Keep bot tokens and other credentials private.

Back up persistent data files regularly, and verify file permissions on the hosting server.

## Security and Responsible Use

- Use the bot only with systems and phone numbers you are authorized to test.
- Obtain consent before sending messages to recipients.
- Do not use the application for unsolicited bulk messaging, harassment, or service disruption.
- Restrict administrative access to trusted Telegram user IDs.
- Never commit bot tokens, private Firebase credentials, or other secrets to a public repository.
- Apply rate limits and monitor activity to prevent misuse.

## Hosting

The bot can run in a Python-compatible Linux environment. For continuous operation, use a persistent VPS or container platform with a suitable process manager and persistent storage.

An SSHX terminal session alone does not guarantee continuous uptime.

## Troubleshooting

**Missing module**

```bash
python3 -m pip install -r req.txt
```

**Invalid Telegram token**

Verify the token in the bot's configuration and regenerate it through BotFather if it has been exposed.

**Firebase connection issues**

Check the endpoint URL, access permissions, network connectivity, and Firebase rules.

**Bot stops after disconnecting**

Check whether the hosting environment terminates its container when the session ends.

## License

Add a license before redistributing this project.
