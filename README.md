# Posty extension for Gemini CLI

Write, schedule and publish social media posts from Gemini CLI with
[Posty](https://posty.hu): Facebook, Instagram, X, LinkedIn, TikTok, YouTube,
Threads, Bluesky, Telegram, Discord and Slack. Posty previews every post per
account (name, @handle, local publish time, character count) and creates it
only after you confirm.

## Install

```bash
gemini extensions install https://github.com/norbertlevente/posty-gemini
```

On first use Gemini CLI opens Posty's sign-in page in your browser. Approve
access for the workspace you want to use.

## What it adds

- MCP server `posty` at `https://api.posty.hu/mcp-oauth` (streamable HTTP,
  OAuth 2.1 with dynamic client registration).
- Context file `GEMINI.md` and the skill `posty`: the posting workflow and
  its rules.
- Commands:
  - `/posty:announce-release`: posts about your latest release, from the
    changelog.
  - `/posty:schedule-post <what and when>`: one post, at the time you name.

## Requirements

- A Posty account at [posty.hu](https://posty.hu) with your social channels
  connected, on a workspace whose plan includes API access.
- A browser on the machine, for the sign-in.

## Try it

- `/posty:announce-release LinkedIn and X, tomorrow 9:00`
- "What is scheduled on my social channels this week?"
- "Cancel the LinkedIn post for Friday."

## Links

- Documentation: https://posty.hu/en/docs/mcp
- Privacy: https://posty.hu/privacy
- Support: norbert@posty.hu

License: AGPL-3.0
