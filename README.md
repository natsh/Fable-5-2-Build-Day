# Fable 5.2 Build Day @ JLL · Field Guide

**Monday 23 November 2026 · JLL offices, Tel Aviv · doors 17:00**

Everything you need tonight is on this page: your API credits, the challenge, how to enter the competition, how judging works and where to demo. Keep it open. You will come back to it when build time ends.

Wi-Fi details are on the screen in the room.

## Tonight in seven steps

| # | What you do | When | Link |
|---|---|---|---|
| 1 | [Redeem your $100 API credits](#redeem-your-api-credits) | As soon as you sit down | ⏳ coming soon |
| 2 | [Point Claude Code at the credits](#use-the-credits-in-claude-code) | Right after step 1 | |
| 3 | [Hear the secret topic and pick a lane](#the-challenge) | 17:55 | 🤫 revealed in the room |
| 4 | [Build](#rules) | 90 minutes | |
| 5 | [Register for the competition](#register-for-the-competition) | During build time | [Registration form](https://docs.google.com/forms/d/1JojzzI04iAFCkX3B-XKKn79CkC6b_AA-lFEX5y_QjoA/viewform) |
| 6 | [Join the judging session and demo](#join-the-judging-session) | When build time ends | ⏳ coming soon |
| 7 | [Share your build with Anthropic](#before-you-leave) | Before you leave | Shared at the end |

---

## Redeem your API credits

Every attendee gets **$100 in Claude API credits**. Do this before build time starts: it takes two minutes now and ten minutes of frustration later.

<!-- TODO(credits): add the QR image (assets/credits-qr.png) and the redemption link here -->
> ⏳ **The redemption link and its QR code will appear here on the day of the event.**

1. **Sign in at [console.anthropic.com](https://console.anthropic.com).** Create an account first if you don't have one. It is free and takes a minute.
2. **Create or select an Organization, not a personal account.** This is the step almost everyone gets wrong. Credits attach to an Organization, never to a personal Claude.ai login. Copy the `Org ID` while you are there.
3. **Open the redemption link on that Organization.**
4. **Create an API key for tonight.** Console → API Keys → Create Key. Give it a name you will recognise, for example `build-day-tlv`.
5. **Confirm the balance.** Console → Billing → Credits should show your $100.

> **Code won't apply?** It was almost always redeemed against a personal user instead of an Organization. Switch to your Organization (step 2) and open the link again. Don't create a second account.

## Use the credits in Claude Code

Claude Code will happily run on your personal Claude.ai login all night, but it won't touch the $100 unless you point it at the API key from step 4 above.

```bash
# paste the API key from step 4, once, in this terminal
export ANTHROPIC_API_KEY="sk-ant-api03-..."

# start Claude Code on Fable 5.2
claude --model claude-fable-5-2
```

- **Key set, key wins.** You don't need to log out of your personal account first. The API key takes priority the moment it is exported.
- **Already mid-session on your personal account?** Type `/login` inside Claude Code and choose the Console / API key option instead of Claude.ai.
- **Not sure which model you are on?** Type `/model` inside Claude Code and pick Fable 5.2.
- **Want it to survive a restart?** Add the `export` line to `~/.zshrc` and open a new terminal tab.

## The challenge

**One competition, one secret topic, one winner.**

<!-- TODO(topic): replace the line below with the topic once it is revealed -->
> 🤫 **The topic is revealed in the room at 17:55.** Nobody sees it earlier, so everyone starts from zero at the same moment.

The topic tells you *what* to build around. The lane you pick tells us *what kind of build* you are going for.

### Pick a lane

Build in whichever lane suits your idea. A lane describes the quality of what you build, never the domain. All three lanes compete for the same prize and are scored on the same criteria.

| Lane | The brief | What it tests |
|---|---|---|
| **Fun** (Delight) | "Build something surprising, or beautiful, or fun. The bar is that you could not have made it this good, this fast, before." | Creativity, taste, and how far the model runs with a loose brief. |
| **Smart** (Breakthrough) | "Build something you could not build before. Bring a problem the previous model could not handle. See how far the new one gets." | Reasoning, long context and agentic depth. The comparison to what came before is the point. |
| **Productive** (Everyday) | "Build something that solves a real problem in your life." | Reliability, tool use, and fit into real workflows. |

## Rules

- **90 minutes to build. 2 minutes to demo.**
- **Solo or in a team of two to four.**
- **Built tonight.** Everything you demo is made in the room, on tonight's topic.
- **Show us the prompt you used and what you built.**
- **Zero slides.** No presentations. Just the thing, running.

## Register for the competition

Registering is what puts you on the list for demos and judging. If you don't register, you don't get called up.

**[Register your project →](https://docs.google.com/forms/d/1JojzzI04iAFCkX3B-XKKn79CkC6b_AA-lFEX5y_QjoA/viewform)**

- The form asks for three things: your project's name, a short description, and a link to it.
- One registration per team. Solo builders register too.
- Register during build time, before demos start.

## Join the judging session

Demos happen in one shared Microsoft Teams meeting. Everyone who registered joins it, and teams are called up one by one to share their screen and present: **2 minutes, live, no slides**.

<!-- TODO(teams): replace with the Microsoft Teams meeting link -->
> ⏳ **The Teams meeting link will appear here.**

1. Join the meeting from your browser when build time ends. You don't need to install Teams.
2. Wait for your name.
3. Share your screen.
4. Give your 2-minute demo.

Before your slot:

- **Have your build already open** in a tab or terminal before your name is called.
- **Allow screen recording, or you can't share your screen.** On a Mac, open System Settings → Privacy & Security → Screen Recording and switch it on for your browser. On newer macOS versions it is called "Screen & System Audio Recording". Check Camera and Microphone there too.
- **Restart your browser after granting access.** A permission switched on while the browser is open usually doesn't take effect until you quit and reopen it.
- **Join a few minutes early and test your screen share.** Better to find out before your name is called than during.

## Judging criteria

Four criteria, weighted equally. The judges score every demo live.

| Weight | Criterion | What the judges look for |
|---|---|---|
| 25% | **New Capability** | Leans on something the new model does that the previous one could not, or could not do well. This is the reason the event exists. |
| 25% | **It Works** | Ran in front of the room and did what the team said it does. |
| 25% | **Keep or Share** | You would use it next week, bring it to a problem you had given up on, or send it to a friend, depending on your lane. |
| 25% | **Clarity of Demo** | The lane, the problem, and what the model did were obvious in two minutes. |

🏆 **One winner.** First place gets a special gift, sent by Anthropic.

## Before you leave

At the end of the event we will share a link to submit what you built to Anthropic. That is how your build counts toward the global Build Day roll-up. Keep an eye on the room and on this page.

## Stuck?

Raise a hand. Helpers are walking the room during build time, and credit or login problems are much quicker to fix in the first ten minutes than in the last ten.

---

Fable 5.2 Build Day · Tel Aviv · hosted by Natali Shtulman, Claude Community Tel Aviv. Thanks to JLL for having us at their Tel Aviv offices.
