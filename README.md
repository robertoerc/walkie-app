# Walkie for Claude Code

**Show your AI what you mean. For a fraction of the tokens.**

Walkie is a Mac app for reviewing what your AI coding agent built. Record your screen, talk through what's wrong and point
at it. Walkie turns that into a short written review — a transcript plus the frames where you pointed — that Claude Code
reads instead of a stack of screenshots.

- **Any window on your Mac**: the iOS Simulator, native apps, Electron apps, Figma, the browser.
- **Your voice and your pointer decide what the agent looks at.**
- **About 3,500 tokens for a typical review** (measured). One 1080p screenshot is 2,691 tokens on Claude 4.7 and later.
- **Runs on your Mac.** No uploads. Your recordings stay on your Mac until you send them.
- **$39 once.** Free to try: 7 screen recordings + 10 screenshots, no account, no card.

## Download

**[Download the latest Walkie for Mac (Apple silicon)](https://usewalkie.com/download/mac)** · or grab the `.dmg` from
[Releases](https://github.com/robertoerc/walkie-app/releases). Signed and notarized by Apple.

Setup guide: https://usewalkie.com/docs/

## Claude Code connection (MCP)

Walkie ships a local MCP server, so Claude Code can drive it with native tool calls:

| Tool | What it does |
|---|---|
| `walkie_start_recording` | Start a recording |
| `walkie_stop_recording` | Stop and build the review |
| `walkie_recording_status` | Is Walkie recording right now? |
| `walkie_list_recordings` | Recent reviews |
| `walkie_get_review` | Read a review (REVIEW.md + key frames) |
| `walkie_list_screenshots` | Recent screenshots |
| `walkie_get_screenshot` | Read one screenshot and its note |

The app connects Claude Code in one click during setup. The server needs Walkie.app running for recording tools; the
screenshot tools read files on disk.

## Not this Walkie

Walkie (usewalkie.com) is not affiliated with the Walkie dictation app at trywalkie.com.

## Support

support@usewalkie.com · Licence: the Walkie EULA (https://usewalkie.com/terms/). This repository hosts release downloads
and documentation; it is not open source.
