# SoundCloud Auth Site

Simple Vercel deployment for SoundCloud OAuth callback.

## Setup

1. Deploy this folder to Vercel
2. Set `SOUNDCLOUD_REDIRECT_URI` in your bot's `.env` to your Vercel URL (e.g., `https://your-app.vercel.app/soundcloud/callback`)
3. Add the redirect URI in your SoundCloud app settings

## How it works

1. User runs `/soundcloud link` in Discord
2. Bot DMs the user a link to SoundCloud's auth page (with `redirect_uri` pointing to this site)
3. User authorizes and gets redirected here
4. This page displays the authorization code
5. User copies the code and pastes it in Discord
6. Bot exchanges the code for tokens and links their SoundCloud account
