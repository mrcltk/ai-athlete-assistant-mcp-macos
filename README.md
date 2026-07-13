# 🏃‍♂️ AI Athlete Assistant: Garmin, Strava & Google Calendar MCP Integration (macOS)

Turn Claude Desktop into a personalized, data-driven sports and recovery coach. This repository provides the complete Model Context Protocol (MCP) configuration to bridge your **Garmin Connect** (biometrics, sleep, HRV), **Strava** (activities, load), and **Google Calendar** (schedule, availability) directly into Claude.

## 🚀 Ecosystem Overview
- **Garmin Connect:** Tracks physiological recovery (Sleep Score, Body Battery, HRV Status).
- **Strava:** Analyzes training volume, past activities, and fitness trends.
- **Google Calendar:** Maps your daily workspace, meetings, and free slots.

---

## ⚙️ Setup Instructions (macOS)

### 1. Prerequisites
Ensure you have **Claude Desktop** and **Node.js** (v18 or higher) installed on your Mac.

### 2. Configure Claude Desktop
Open your Mac Terminal and run this command to navigate to the Claude configuration directory:
```bash
open ~/Library/Application\ Support/Claude/
```
Open `claude_desktop_config.json` (create it if it doesn't exist) and merge the structure provided in `claude_desktop_config.example.json` into it.

### 3. API & Credentials Authorization
- **Garmin:** Replace with your actual Garmin Connect credentials.
- **Strava:** Fetch your `CLIENT_ID`, `CLIENT_SECRET`, and `REFRESH_TOKEN` from the Strava.
- **Google Calendar:** No tokens needed. Upon restarting Claude, a secure OAuth browser window will automatically trigger for Google sign-in.

---

## 🔄 Final Step: Restart Claude
Completely quit Claude Desktop (`Cmd + Q`) and reopen it. You will see the tools/plug icons illuminated under the chat bar, signaling all 3 servers are live!

## 💡 Example Prompt to Test
> "Analyze my Garmin HRV and sleep scores for the last 3 days against my recent Strava training load. Cross-reference my Google Calendar availability for tomorrow and suggest if I should push hard or take a recovery day."
