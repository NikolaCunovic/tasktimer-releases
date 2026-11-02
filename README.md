# Task Timer

A small Windows app for tracking time on tasks and logging it to Redmine.

**[Download TaskTimer.exe](https://github.com/NikolaCunovic/tasktimer-releases/releases/latest/download/TaskTimer.exe)** (Windows 10 and 11, always the newest version)

## What it does

- Start and stop a timer on a task. It lives in the tray, has global hotkeys (Ctrl+Alt+Space start/stop, Ctrl+Alt+T show/hide) and a small always-on-top bar (Ctrl+Alt+M).
- Pulls the Redmine issues assigned to you into a backlog.
- **Log time** turns a day's tracked time into Redmine time entries: rounded to half hours, filled up to 8 hours, with comments taken from your notes. You review everything before it's sent.
- Marking an issue Done can close it in Redmine and log the time in one step.
- A week strip shows which days are logged. Croatian public holidays and your own days off are left out.
- Optional daily and weekly reports into Joplin.

## Install

1. Download **TaskTimer.exe**. If your browser says the file "isn't commonly downloaded", choose **Keep**.
2. Put it in a folder where it can stay, for example `C:\Users\<you>\Apps\TaskTimer\`. "Start with Windows" remembers this location.
3. Run it. Windows may show **"Windows protected your PC"**: click **More info**, then **Run anyway**. This appears because the app isn't signed with a paid certificate.
4. Open **Settings › Redmine**, enter your Redmine address and your API key (in Redmine: **My account › API access key**), and click **Test connection**.

## Your data stays on your PC

- Tasks, time and notes: `%APPDATA%\TaskTimer\`, with a daily backup kept for 14 days.
- Your Redmine API key: Windows Credential Manager, never in a file.
- The app talks only to your Redmine and, if you connect it, to Joplin on your own PC. There's no account, cloud or tracking.

## Updating

Right-click the tray icon and choose **Quit**, replace `TaskTimer.exe` with the new download, and start it again. Your data is kept. Your version is shown at the bottom left of **Settings**.

## Requirements

Windows 10 or 11 with the Microsoft Edge WebView2 Runtime, which Windows 11 and up-to-date Windows 10 already include.
