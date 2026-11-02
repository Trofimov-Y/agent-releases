# Agent

Agent is a work assistant that lives on your Mac. It keeps one chat with you, in its own window and on your iPhone, and reads what you connect: Slack, your work calendar and mail, GitHub and the Google Meet calls you choose to record.

This repository holds Agent's releases and nothing else: each one is the Mac app, signed by the team and checked by Apple.

## What you need

- A Mac with macOS 27 or later.
- A home folder whose name holds only Latin letters, digits and `. _ + @ -`, with no spaces (in Finder, Go → Home shows it). Agent does not start otherwise.
- A paid Claude plan: Pro, Max, Team or Enterprise. Everything Agent does counts against your plan's usage limits, including what it does by itself: two briefings a day, a look back over each day at night, and looking into Slack messages once Slack is connected. The briefings and the look back each have a switch; looking into Slack stops with Slack's own.
- Only for what you will use: your work Slack and Google accounts; a GitHub account; Google Chrome for calls; an [ElevenLabs](https://elevenlabs.io) account of your own, which you pay for, for calls and for dictation on the iPhone; an iPhone with iOS 27 for the iPhone app.

## Download

Open [the latest release](../../releases/latest) and, under **Assets**, download `Agent-<version>.dmg`. The `.zip` beside it is for Agent's own updates: you do not need it.

## Install

1. Open the `.dmg` and drag **Agent** onto **Applications**. If macOS asks for an administrator's password, your Mac account is a standard one: cancel, and drag Agent into the **Applications** folder of your home folder instead (in Finder, Go → Home; make the folder if it is not there). Agent can update itself only in a folder your account may change.
2. Open Agent, and choose **Open** when macOS asks about an app downloaded from the internet. Its window says what it waits for, with a button for each:
   - **Apple's command line tools**, if your Mac has none: **Install the Tools…**, then **Install** in Apple's window. It takes a few minutes.
   - **Login Items**: if asked, **Open Login Items…** and turn Agent on.
   - **The Keychain**: macOS asks whether Agent may use what is stored in “workagent”. Type the password you log in to your Mac with, and choose **Always Allow**.
3. Agent's first page asks for the agent's name and language, has you **Sign in** to Claude in your browser, and lets you turn off what you will not use. **Finish** opens the chat.
4. Connect what you use, each on its own page in Agent's window, whenever you want:
   - **Slack:** Agent fills in a Slack app for you to create. Your Slack administrators may have to approve it.
   - **Google:** sign in with your work account. Google says it has not verified the app: choose **Advanced**, then go on to it, and leave every box ticked. If your organization does not allow the app, its Google administrator has to allow it first.
   - **GitHub:** sign in with your GitHub account and type the code Agent shows.
   - **Calls:** set your ElevenLabs key on the Calls page, and choose **Open in Chrome Web Store** there to add the Chrome extension. Then press the extension's button in Chrome's toolbar and **Connect to Agent**: it shows a short code, and the Calls page shows a request with the same code. Choose **Allow** for that one.
   - **iPhone:** send the email address of your Apple ID to whoever maintains Agent in your team. Accept Apple's invitation, install **TestFlight** from the App Store, and install Agent from the TestFlight email. Then choose **Pair a phone** on the Phone page and scan the code with the iPhone app.

## Updates

Agent looks for a new release every hour, downloads it and checks it, and asks before it restarts: **Restart Now**, or **When Idle**, which waits until nothing is going on and you are away from it. Your chats, memory and connections stay.

## What it does with your data

Agent runs on your Mac as you, and keeps what it reads there. What it reads goes to Anthropic, as part of your Claude plan's turns; the sound of calls and dictation goes to ElevenLabs; the phone reaches your Mac through the team's relay, which cannot read what they say to each other. Agent posts in Slack as its own bot, never in your name.

## Help

Agent's window says what is wrong and what to do about it. If that does not help, ask whoever maintains Agent in your team.
