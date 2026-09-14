# DACC Race Engineer — Discord Activity MVP

This is a standalone-first race-control web app designed to run as a Discord Activity.

## What is included

- Current / next / following driver
- Editable stint order and lap targets
- IRL race clock and an independent server clock locked to 10:00
- Race time remaining
- Driver lap + driving-time totals
- Driver availability warnings
- Configurable average lap time, fuel/lap, tank size, pit loss and fuel margin
- Fuel calculator by laps or remaining minutes
- +1 / -1 lap, PIT NOW, advance stint and delay schedule controls
- Race notes and race log
- Local autosave via browser localStorage
- JSON import/export
- Push-to-talk voice commands using the browser SpeechRecognition API
- Optional Discord Embedded App SDK initialisation

## First run

1. Put these files on a simple HTTPS host. GitHub Pages is fine for testing.
2. Open `config.js`.
3. Paste your public Discord **Application ID** into `discordClientId`.
4. Do not put a bot token or client secret in this app.

You can test it outside Discord before doing any Discord setup.

## Voice examples

- “fuel 2.24, 47 minutes”
- “fuel 47 minutes”
- “add one lap”
- “remove one lap”
- “next driver”
- “delay 3 minutes”

Voice support depends on the browser/embedded client granting microphone and speech-recognition support.

## Current seed

The app is seeded with the current Round 9 Zolder schedule captured from the master workbook available to ChatGPT at rebuild time.
Edit the schedule in-app and Export JSON to preserve a race state outside localStorage.

## Important

The Excel workbook remains the archive/planning master. This app is intended to be the live race-day front-end.
