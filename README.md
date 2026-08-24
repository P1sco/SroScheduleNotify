#  Silkroad Schedule Manager

![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## Features

- **Event Management** - Add, edit, and delete scheduled events with ease
- **Real-time Countdown** - Live countdown timer showing time until the next event(s)
- **Smart Notifications** - Get reminded 10, 5, and 1 minute before each event
- **Multi-Timezone Support** - View all events in your local timezone
- **System Tray Integration** - Minimize to tray and keep running in background
- **Sound Alerts** - Text to speech alerts.
- **Persistent Storage** - All events saved automatically to `schedule.json`

## Quick Start

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/silkroad-schedule-manager.git
cd silkroad-schedule-manager
```
2. **Install dependencies**
```bash
pip install PyQt6 plyer playsound
```
3. Run **the application**
```bash
python SroScheduleNotify.py
```

## How to Use

### Managing Events

#### Add an Event
1. Click the **"Add"** button in the Actions panel
2. Enter the event name in the "Event Name" field
3. Set the event time using the time picker
4. Toggle "Enable Notifications" if you want reminders
5. Click **"Confirm"** to save the event

> **Tip:** The application automatically sorts events by their upcoming time, with the earliest event appearing at the top.

#### Edit an Event
1. Select an event from the list by clicking on it
2. Click the **"Edit"** button
3. Modify the name, time, or notification settings
4. Click **"Confirm"** to save your changes

#### Delete an Event
1. Select an event from the list
2. Click the **"Delete"** button
3. Confirm the deletion when prompted

### Notification Controls

#### Individual Event Notifications
- **Notify** - Enable notifications for a selected event
- **Unnotify** - Disable notifications for a selected event

> **Visual Indicators:**
> - 🟢 Green indicator = Notifications are enabled
> - 🔴 Red indicator = Notifications are disabled

#### Bulk Notification Controls
- **Notify All** - Enable notifications for all events at once
- **Unnotify All** - Disable notifications for all events at once

### Countdown Display

#### Real-time Countdown Timer
- The **⏱️** icon appears next to the next upcoming event(s)
- Countdown updates every second in real-time
- Displays time remaining in the format:
  - **Hours, Minutes, Seconds**: `2h 30m 15s`
  - **Minutes, Seconds**: `45m 10s`
  - **Seconds Only**: `30s`
  - **Event Reached**: `NOW!`

> **Note:** If multiple events occur at the same time, all of them will display the countdown timer simultaneously.

### Timezone Settings

#### Changing Timezone
1. Locate the "Timezone" dropdown in the top-right corner
2. Select your timezone (e.g., GMT+3, GMT-5)
3. All event times will automatically adjust to your selected timezone
4. The status indicator will briefly flash orange to confirm the change

> **Default Timezone:** GMT+3 (Silkroad Online server time)

### System Tray Integration

#### Minimize to Tray
- Click the minimize button on the window
- The application will hide to the system tray
- Continues running in the background

#### Status Text
- Shows current action status
- Displays selected event details
- Confirms completed actions

### Data Storage

#### Schedule File
- Events are automatically saved to `schedule.json`
- Located in the same directory as the application
- Can be backed up or transferred to other installations
- JSON format for easy editing if needed

> **Warning:** Manual editing of the JSON file is not recommended unless you're familiar with JSON syntax.

### Tips & Tricks

1. **Planning Multiple Events**
   - Add all your daily events at once
   - Use the "Notify All" feature for quick setup

2. **Cross-Time Zone Playing**
   - Set the timezone to your local time
   - Events will display in your timezone automatically
