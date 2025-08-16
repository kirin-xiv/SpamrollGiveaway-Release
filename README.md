# Spamroll Giveaway Plugin

> ## 🔄 **REPOSITORY MIGRATION NOTICE**
> 
> **This plugin has moved to a centralized repository!**
> 
> **New Installation URL:** 
> ```
> https://raw.githubusercontent.com/kirin-xiv/KirinPlugins/main/pluginmaster.json
> ```
> 
> **Please update your Dalamud settings** to use the new central repository for better updates and access to all Kirin plugins.
> 
> [📋 View Migration Guide](./MIGRATION_NOTICE.md) | [🏠 Central Repository](https://github.com/kirin-xiv/KirinPlugins)

---

Run giveaways, Brain off!

Automates spamroll giveaway games in FFXIV by tracking rolls and determining winners automatically. No more manual counting or forgetting who won what numbers!

## 🎯 What It Does

- Automatically detects `/random` rolls during your giveaway games
- Configurable winning numbers (default: 111, 222, 333, 444, 555, 666, 777, 888, 999)
- Smart multiple winner support - one winner per winning number
- Prevents duplicate winners across numbers (configurable)
- Announces winners automatically to chat
- Rate-limited chat messages to avoid FFXIV spam detection
- Chat channel selection (Say, Party, Yell, Shout, Echo)
- Custom announcement templates

## 📥 Installation

### ✅ Recommended: Central Repository
1. Add this repository URL to your Dalamud plugin sources:
   ```
   https://raw.githubusercontent.com/kirin-xiv/KirinPlugins/main/pluginmaster.json
   ```

### ⚠️ Legacy: Individual Repository (Deprecated)
1. Add this repository URL to your Dalamud plugin sources:
   ```
   https://raw.githubusercontent.com/kirin-xiv/SpamrollGiveaway-Release/main/repo.json
   ```

2. Install "Spamroll Giveaway" from the plugin installer

3. Type `/spamroll` to open the plugin window

## 🎮 How to Use

1. **Start a game**: Use `/spamstart` or click "Start Game" in the plugin window
2. **Watch for rolls**: The plugin automatically detects winning rolls
3. **Winners announced**: Winners are automatically announced to your chosen chat channel
4. **Game ends**: Automatically or manually with `/spamstop`

### Example Flow
```
[Spamroll] Game started! Winning numbers: 111, 222, 333 - Type /random to participate!
WINNER: PlayerName rolled 222!
WINNER: AnotherPlayer rolled 111!
[Spamroll] Game stopped. 2 winners.
```

## 🔧 Commands

- `/spamroll` - Open the main plugin window
- `/spamroll config` - Open configuration directly  
- `/spamstart` - Start collecting rolls
- `/spamstop` - Stop the current game
- `/spamconfig` - Open configuration window

## 📋 Features

### Smart Winner Detection
- Only processes configured winning numbers
- First come, first served for each number
- Optional: Same player can win multiple numbers
- Automatic game completion when all numbers claimed

### Rate-Limited Messaging
- 2-second delays between chat messages
- Prevents FFXIV chat spam detection
- Queued announcements for multiple winners
- "Clear Queue" button to cancel pending messages

### Flexible Configuration
- 1-9 winning numbers supported
- Multiple winner modes
- Custom chat templates with placeholders
- Game timeout settings
- Sound notifications

## 🎭 Perfect for FFXIV Events!

This plugin was designed for FFXIV event organizers running giveaway games. It eliminates manual work and ensures fair, consistent games every time. The rate limiting system means your messages won't get blocked, and the flexible winning number system works for any type of giveaway!

**Made with ❤️ by Kirin**