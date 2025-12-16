# Flow Cloud Pass Changer - Discord Bot

## Overview
A Discord bot for automated Microsoft account password changes. The bot allows authorized users to change passwords through Discord commands, with captcha verification and success notifications.

## Commands

### User Commands (Authorized Users Only)
- `+passchange email:password` - Start a password change for the specified account

### Owner Commands Only
- `+auth @user` - Authorize a user to use passchange
- `+unauth @user` - Remove authorization from a user
- `+setlog #channel` - Set the channel for bot activity logs
- `+setcaptcha #channel` - Set the channel for captcha images and solutions
- `+setsuccess #channel` - Set the channel for successful password change notifications

## Configuration Files
- `config.json` - Discord bot token and webhook settings
- `authdb.json` - List of authorized user IDs
- `settings.json` - Channel configurations

## Owner ID
The owner ID is set to: `1383641747913183256`

## Setup
1. Add your Discord bot token to `config.json`
2. Run the bot with `python bot.py`
3. Use `+setcaptcha`, `+setlog`, and `+setsuccess` to configure channels
4. Use `+auth @user` to authorize users

## Technical Details
- Built with discord.py
- Uses Selenium for browser automation
- Supports headless Chrome/Chromium
- Temporary email generation for verification

## Recent Changes
- December 16, 2025: Initial consolidated bot implementation
