# pricetools.space

Simple, real-time Bitcoin price tools: USD to BTC/Sats converter, historical purchase price tracker, and price projection tool. 100% static site, no trackers or personal data collected.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Features
- **USD to BTC/Sats Converter**: Instant conversions with live prices.
- **Price History Tool**: Track current values of past BTC purchases over time.
- **Price Projection Tool**: Model future prices based on historical trends.

## Setup
1. Download all files/folders from this repo.  
2. Upload to your FTP server root (e.g., via FileZilla: connect to host, drag files to `/public_html/` or equivalent).  
3. Edit `update.sh`: Replace `YOURUSERNAMEHERE` with your server username (e.g., `ubuntu`) and `ROOTFOLDERNAMEHERE` with your site root path (e.g., `pricetools.space`).  
4. Add to cron for auto-updates: Run `crontab -e`, add `0 1 * * * PATH=/usr/local/bin:/usr/bin:/bin /bin/bash /home/YOURUSERNAMEHERE/ROOTFOLDERNAMEHERE/update.sh > /dev/null 2>&1` (daily refresh at 1am UTC). Test with `./update.sh`.

## License
MIT © pricetools-space — free to use, modify, and distribute.
