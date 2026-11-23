# Fable 5.2 Build Day @ JLL · Field Guide

**Monday 23 November 2026 · JLL offices, Tel Aviv · doors 17:00**

Everything you need tonight is on this page: your API credits, the challenge, how to enter the competition, how judging works and where to demo. Keep it open. You will come back to it when build time ends.

Wi-Fi details are on the screen in the room.

## Tonight in seven steps

| # | What you do | When | Link |
|---|---|---|---|
| 1 | [Redeem your $100 API credits](#redeem-your-api-credits) | As soon as you sit down | [Credit redemption link](https://platform.claude.com/offers/2d4dc8a4-4f1d-4806-9b63-e443b2ad684c) |
| 2 | [Point Claude Code at the credits](#use-the-credits-in-claude-code) | Right after step 1 | |
| 3 | [Hear the secret topic and pick a lane](#the-challenge) | 17:55 | 🤫 revealed in the room |
| 4 | [Build](#rules) | 90 minutes | |
| 5 | [Register for the competition](#register-for-the-competition) | During build time | [Registration form](https://docs.google.com/forms/d/e/1FAIpQLSdOlFV5gV-LIeMh_WrWW8F0rVcKN1MKb9vbu6dWTEr09kg9NA/viewform) |
| 6 | [Join the judging session and demo](#join-the-judging-session) | When build time ends | [Teams judging meeting](https://teams.microsoft.com/meet/245641779597856?p=JmTa6aewDO6IAnk9P5) |
| 7 | [Share your build with Anthropic](#before-you-leave) | Before you leave | [Build submission form](https://form.typeform.com/to/SygLMeAD) |

---

## Redeem your API credits

Every attendee gets **$100 in Claude API credits**. Do this before build time starts: it takes two minutes now and ten minutes of frustration later.

<p align="center"><a href="https://platform.claude.com/offers/2d4dc8a4-4f1d-4806-9b63-e443b2ad684c"><img src="assets/credits-qr.png" alt="QR code for the API credit redemption link" width="240"></a></p>

**Redemption link: [platform.claude.com/offers/2d4dc8a4-…](https://platform.claude.com/offers/2d4dc8a4-4f1d-4806-9b63-e443b2ad684c)** (or scan the QR)

1. **Sign in at [console.anthropic.com](https://console.anthropic.com).** Create an account first if you don't have one. It is free and takes a minute.
2. **Copy your Org ID from the console.** Credits attach to an Organization, never to a personal Claude.ai login. The form wants the console `Org ID`; **a Claude.ai UUID is rejected.**
3. **Open the redemption link and submit that Org ID.** One claim per person, so check it before you hit submit.
4. **Give it a couple of minutes.** Credits are issued almost instantly, but systems need a moment.
5. **Create an API key for tonight.** Console → API Keys → Create Key. Give it a name you will recognise, for example `build-day-tlv`.
6. **Confirm the balance.** Console → Billing → Credits should show your $100.

> **API only.** The credits work with the Claude API, not on Claude.ai. That's why Claude Code needs the API key (next section).
>
> **Claim once, from one account.** Automated fraud checks block anyone who submits from several profiles, and a wrong submission can't be fixed afterwards. Not sure which ID to paste? Raise a hand before you submit.

## Use the credits in Claude Code

Claude Code will happily run on your personal Claude.ai login all night, but it won't touch the $100 unless you point it at the API key from step 5 above.

```bash
# paste the API key from step 5, once, in this terminal
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
- **Your demo: show us the prompt you used, then demo your build live.** It doesn't need to be perfect, but it must be live.
- **Zero slides.** No presentations and no recordings. Just the thing, running.

## Register for the competition

Registering is what puts you on the list for demos and judging. If you don't register, you don't get called up.

**[Register your project →](https://docs.google.com/forms/d/e/1FAIpQLSdOlFV5gV-LIeMh_WrWW8F0rVcKN1MKb9vbu6dWTEr09kg9NA/viewform)**

- The form asks for your name or team name, a short description, and a link to your project (GitHub or a published site). The link is optional.
- One registration per team. Solo builders register too.
- Register during build time, before demos start.

## Join the judging session

Demos happen in one shared Microsoft Teams meeting. Everyone who registered joins it, and teams are called up one by one to share their screen and present: **2 minutes, live, no slides**.

**Judging meeting: [Join on Microsoft Teams](https://teams.microsoft.com/meet/245641779597856?p=JmTa6aewDO6IAnk9P5)**

1. Join the meeting from your browser when build time ends. You don't need to install Teams.
2. Wait for your name.
3. Share your screen.
4. Show your prompt, then give your 2-minute live demo.

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
| 25% | **Clarity of Demo** | How your build connects to the secret topic, which lane you chose, and what the model did were all obvious in two minutes. |

🏆 **One winner.** First place gets a special gift, sent by Anthropic.

## Before you leave

Submit what you built to Anthropic, so the Community can feature what you made and your build counts toward the global Build Day roll-up. This is separate from registering for tonight's competition.

**[Submit your build →](https://form.typeform.com/to/SygLMeAD)**

## Need inspiration?

See [**Captcha2030**](examples/captcha2030/), the host's demo: a robot-takeover strategy game built on Fable 5.2 from one loose prompt and a few follow-ups, in one HTML file with no libraries. [▶ Play it online](https://natsh.github.io/Fable-5-2-Build-Day/examples/captcha2030/). Its README has every prompt verbatim and what each session cost.

## Stuck?

Raise a hand. Helpers are walking the room during build time, and credit or login problems are much quicker to fix in the first ten minutes than in the last ten.

---

Fable 5.2 Build Day · Tel Aviv · hosted by Natali Shtulman, Claude Community Tel Aviv. Thanks to JLL for having us at their Tel Aviv offices.
