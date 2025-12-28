EdenAI — Telegram Utility, Media & AI Bot

EdenAI is a multi-purpose Telegram bot that combines media downloading, AI features, and community/admin utilities into a single bot.

It supports:
- YouTube video & audio downloads (with interactive quality selection)
- TikTok video downloads
- Meme fetching from Reddit
- AI image generation
- AI chat replies when mentioned
- Admin moderation tools
- Scheduled posts, giveaways, announcements, and welcome media
- Usage statistics and rate-limiting
- Large-file handling with automatic fallbacks

==================================================

FEATURES

Media Downloading
- YouTube downloader (yt-dlp based)
  - /youtube <url> quick download
  - /download <url> interactive quality buttons (MP3, 480p, 720p, 1080p, Best)
  - Cookie support (cookies.txt)
  - EJS challenge support
  - Automatic compression for large files
  - Telethon fallback for files up to ~2GB
  - HLS streaming fallback

- TikTok downloader
  - /tiktok <url>
  - SnapTik scraping
  - No-watermark videos when available

AI & Content
- AI image generation
  - /image <prompt>
  - Cloudflare AI powered
- AI chat replies when bot is mentioned

Memes
- /meme random meme
- /meme <subreddit> meme from specific subreddit

Statistics
- SQLite usage tracking
- Per-user download counts
- Global stats for admins
- /stats and /adminstats commands

Admin & Community
- /mute and /unmute moderation
- Admin-only command enforcement
- Scheduled daily messages
- Welcome media
- Announcements and giveaways
- Rate limiting and abuse prevention

==================================================

QUICK START

1. Clone the repo
git clone https://github.com/joshb0ts/EdenAIbot.git
cd EdenAIbot

2. Create virtual environment
python3 -m venv .venv
source .venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

4. Create .env file

BOT_TOKEN=YOUR_TELEGRAM_BOT_TOKEN
CLOUDFLARE_API_TOKEN=YOUR_CLOUDFLARE_AI_TOKEN
ADMIN_USER_IDS=123456789,987654321
LOG_LEVEL=INFO

5. Run the bot
python3 memebot.py

==================================================

COMMANDS

User Commands
/start
/help
/download <url>
/youtube <url>
/tiktok <url>
/meme
/meme <subreddit>
/image <prompt>
/stats

Admin Commands
/adminstats
/mute <user>
/unmute <user>
/cookiestatus
/cookiehelp

==================================================

DEPLOYMENT

Designed for Linux / VPS environments.
Supports systemd for long-running deployments.

==================================================

LICENSE

MIT License
