This is a laravel demo app for using telegram-git-notifier package.

## Requirements

- PHP ^8.1
- Laravel ^9.0
- [laravel-telegram-git-notifier](https://github.com/cslant/laravel-telegram-git-notifier) ^1.0

## Installation

### Clone the repository

```bash
git clone git@github.com:tanhongit/laravel-telegram-git-notifier-demo.git
```
### Composer install

```bash
composer install
```

### Copy .env file

```bash
cp .env.example .env
```

### Generate key

```bash
php artisan key:generate
```

### Set your telegram bot token

```bash
TELEGRAM_BOT_TOKEN=your-telegram-bot-token
```

### Set your telegram chat id

```bash
TELEGRAM_BOT_CHAT_ID=your-telegram-chat-id
```

### Set your github webhook url

```bash
TGN_APP_URL=your-github-webhook-url
```

For this package, the webhook URL will be defined in config. So the default value will be http://localhost:8000/telegram-git-notifier

So you can set your webhook URL like this:

```bash
TGN_APP_URL=https://your-domain/telegram-git-notifier
```

### Set chat ID or topic ID to notify

```bash
TELEGRAM_NOTIFY_CHAT_IDS="your-chat-id-1;your-chat-id-2"
```

