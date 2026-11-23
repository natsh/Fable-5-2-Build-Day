# Example: Captcha2030 — Are You a Robot?

A browser game built entirely with Claude Code on **Fable 5.2** as the host's demo for this Build Day. One HTML file, no libraries, no image files: everything you see is drawn in code.

**[▶ Play it online](https://natsh.github.io/Fable-5-2-Build-Day/examples/captcha2030/)**, or download [`index.html`](index.html) and open it in a browser. No server needed.

It's 2030. Robots have taken over Kiryat Ono, a Tel Aviv suburb, and it's permanently night. The few survivors hide in homemade robot costumes; to win them over you have to pass their "are you human?" tests (fail one and it's a mini-game duel: rock paper scissors, tic-tac-toe, quick draw), hide from patrolling androids, then put your crew to work rebuilding the city, collecting scrap, food, power and know-how until you can fire up the City Hall transmitter.

| Controls | |
|---|---|
| Move | WASD or arrow keys (on-screen joystick on touch) |
| Talk, scavenge, use | E or Space |
| Answer a humanity test | 1 / 2 / 3 |
| Command panel: orders, tech, city | Tab |
| Mute | M, or the 🔊 button on the minimap |

## How it was built: the prompts, verbatim

This is the point of the example: it's a loose brief, then short follow-ups in plain language, including typos. Nothing was planned up front.

**Session 1: the one-shot build** (one pasted brief, ~26 min of model time)

> Build me a game, with no libraries and no image files.
> It's 2030 and AI robots have taken over Qiryat Ono (my city, a tel aviv suburb)
> village from above, cute and cozy style with day and night cycle.
> humans have no way of knowing if you are a robot or not, and they ask you 'are you a robot?' type of questions, to test your humanity, as a challange.
> if you answer right, they will let you pass. if not, they will fight you a mini game of a classic game, like rock paper scissors or something. there are robots patrolling the streets that you need to hide from.
> your goal is to gather humans as your ally, to re-build the city and save earth.

Then four small tweaks in the same session:

> I don't like the other humans following me. Let's instead have them stand next to some building or something that once we unlock them with the test, they start building it. And after a while, it's renovated and now functioning. What do you think?

> I want to change guys question to what is a better game, Roblox, Minecraft, or I don't know, I just play both.

> And the answer is I don't know, I play both.

> If you're born, it's tic-tac-toe. *(dictated: "if you're wrong")*

**Session 2: the restyle** (fresh context, one prompt)

> Okay, I want to keep building on the game. I want to add like a post-apocalyptic kind of vibe. So make it maybe that it's only nighttime and it's like very futuristic. And make the robots more like humanoids maybe. And make the characters look like as if they are pretending to be robots.

**Session 3: the strategy layer** (fresh context, one prompt)

> I want to make some changes to the game. I want it to become more of a strategy game. Think StarCraft, World of Warcraft, Dune. So I want to be gathering people for the task using the human check. And then once I have them, I can decide where I want them to invest. That means to like assign them to like a property to fix, and then it will help me like collect values some kind. So I want to have like kind of an inventory or stats about what am I collecting and how big is my current status and city, and just to add more gaming to it.

## What it cost

**About $30 in total**, rough estimates at API prices (Fable 5.2, effort high):

| Session | What | Cost (approx.) | Result |
|---|---|---:|---|
| 1 | The initial one-shot build | ~$10 | 1,027 lines |
| 2–3 | Two adjustment sessions: post-apocalyptic restyle, then the strategy layer | ~$20 | 1,436 lines |

Small one-line tweaks cost cents; almost all of that is re-reading the cached context, which is why each new direction starts with `/clear` and a fresh session.

## Tips you can steal for tonight

- **Start with a vibe, not a spec.** Setting, goal, one twist, and the constraint ("no libraries, no image files") is enough for a first playable version.
- **Make it personal.** A real place and real people (the neighbors here are the host's family and local spots) make a demo land.
- **One direction per session.** When the next change is a new idea rather than a tweak, `/clear` and describe it fresh.
- **Keep a backup before big changes.** Copy the working file before a restyle or a new game layer, so you can always demo the last good version.
