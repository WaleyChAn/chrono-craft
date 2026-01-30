# ChronoCraft Deployment Guide

> Deploy to Raspberry Pi in Kiosk Mode

## Prerequisites
- OS: Raspberry Pi OS (64-bit)
- Node.js 18+
- PM2 process manager

## Installation Steps

```bash
# 1. Clone repository
git clone <repo-url>
cd chrono-craft

# 2. Install dependencies
npm install

# 3. Build application
npm run build

# 4. Configure PM2
pm2 start npm --name "chronocraft" -- start
pm2 save
pm2 startup
```

## Kiosk Mode Setup

<!-- TODO: Add Chromium kiosk mode configuration -->

## Auto-Start on Boot

<!-- TODO: Add systemd/PM2 auto-start configuration -->
