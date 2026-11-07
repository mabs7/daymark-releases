# Daymark Desktop — Official Downloads & Releases

[![Latest Release](https://img.shields.io/github/v/release/mabs7/daymark-releases?color=237a53&label=Latest%20Release)](https://github.com/mabs7/daymark-releases/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-blue?color=1d1d1f)](https://github.com/mabs7/daymark-releases/releases/latest)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](https://github.com/mabs7/daymark-releases/blob/main/LICENSE)

> **A quiet, personal Windows desktop publishing agent for keeping a steady daily X (Twitter) presence without the daily scramble.**

---

## What is Daymark?

Daymark is a free Windows desktop application designed to keep your X queue full, original, and consistent. It works quietly in the background: checking your queue, writing new posts in your authentic voice using your preferred AI provider, and scheduling them through Buffer.

Once scheduled in Buffer, posts publish to X at your specified times—even when your computer is off or asleep.

---

## Key Features

- **Quiet Automation:** Runs a quick check at Windows sign-in and twice daily (default: 09:00 and 18:00 local time). Each background check completes its work and exits immediately.
- **Flexible Posting Routine:** Choose to post 1, 2, or 3 times per day with custom times and a rolling horizon from 1 to 7 days ahead.
- **Respects Existing Posts:** Automatically detects any manual posts in Buffer and fills only the empty slots.
- **Your Choice of AI Writer:**
  - **ChatGPT Plan Sign-In:** Official browser sign-in using your eligible ChatGPT Plus / Team plan usage sharing.
  - **OpenAI API:** Direct connection with your own OpenAI API key.
  - **Google Gemini API:** Fast generation using your Google AI Studio Gemini key.
  - **Anthropic Claude API:** Quality writing using your Claude Console key.
- **Strict Quality & Batch Validation:** Checks every generated post for character count, mention limits, and duplicates before scheduling. Never schedules incomplete or cut-off text.
- **Private & Secure by Design:**
  - **DPAPI Credential Vault:** API keys and OAuth tokens are encrypted using Windows DPAPI via Electron `safeStorage`.
  - **Encrypted Local Storage:** Writing profiles, journals, and queue history are protected at rest with authenticated AES-256-GCM encryption.
  - **No Web Scraping or Bots:** No browser automation, no X password collection, and no scraping of ChatGPT chat history.
- **Built-in Auto-Updates:** Silently downloads new releases in the background and prompts you with a clean "Restart to update" banner.

---

## How to Download & Install

### Step 1: Download the Installer
Download the latest Windows installer:
👉 **[Download Daymark-Setup.exe (Latest Release)](https://github.com/mabs7/daymark-releases/releases/latest/download/Daymark-Setup.exe)**

*(You can also browse all past releases on the [Releases Page](https://github.com/mabs7/daymark-releases/releases).)*

### Step 2: Install Daymark
1. Double-click `Daymark-Setup.exe`.
2. The installer will install Daymark per-user to `%LOCALAPPDATA%\Programs\Daymark` (no administrator privileges or UAC elevation required).
3. Shortcuts will be created on your **Desktop** and in your **Start Menu**.

> [!NOTE]
> **Windows SmartScreen Note:**  
> Because Daymark is an independent release without an expensive corporate signing certificate, Windows Defender SmartScreen may display:  
> *"Windows protected your PC — Microsoft Defender SmartScreen prevented an unrecognized app from starting."*  
> Simply click **"More info"** → **"Run anyway"** to complete the setup.

---

## 3-Step Quick Start Guide

1. **Connect Buffer:**
   - In Daymark → **Accounts**, authorize your dedicated Buffer account (with 1 connected X channel).
   - Select your X channel.
2. **Choose Your AI Writer:**
   - Sign in with your ChatGPT plan or paste your OpenAI, Gemini, or Claude API key.
   - Click **Load models** and select your preferred writing model.
3. **Set Your Routine:**
   - In **Writing profile**, define your topics, voice/tone, real facts, and things to avoid.
   - In **Automation**, set your posting frequency, posting times, and toggle **Generate and publish automatically** and **Run at sign-in and twice daily**.
   - Click **Save routine**, then click **Check queue now** in Overview to create your first scheduled batch!

---

## System Requirements

- **Operating System:** Windows 10 or Windows 11 (64-bit)
- **Dependencies:** None (Electron runtime, Python worker, and all dependencies are fully self-contained)
- **Account Requirements:**
  - One dedicated [Buffer](https://buffer.com/) account connected to your X account.
  - An eligible ChatGPT plan or an API key from OpenAI, Google Gemini, or Anthropic.

---

## License

Daymark Desktop is free, open-source software released under the [MIT License](https://opensource.org/licenses/MIT).
