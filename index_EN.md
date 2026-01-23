# DDS - DanceDanceShuffle
[Japanese](index.md) | [English](index_EN.md) | [GitHub](https://github.com/stakiran/dds)

A new music game concept that blends step-based gameplay with shuffle dance

![](images/demo.gif)

## 📍Overview
DDS is an idea for a new music game.

### 1: A full 2D field on the ground
![](images/260124_053608.png)

**Notes are displayed and processed on the ground**. Like Osu! or Synchronica, it uses the entire two-dimensional field.

![](images/leftright.gif)

The field is wide horizontally, and you move back and forth from left to right as shown. This is because shuffle-dance-style movement is placed at the core.

![](images/updown.gif)

The field also has depth, to add variety to where you place your feet.

### 2: Dynamic but easy movements
The movements used in DDS are based on shuffle dance. They're dynamic, and fun both for the player and for anyone watching.

Main movements include:

![](images/skill_rm.gif)

Running Man. Pull each foot back twice.

![](images/skill_ts.gif)  

T-step. Move while swinging your pivot foot like a pendulum.

![](images/skill_shufflestomp.gif)

Shuffle stomp. Essentially stomping in place (alternating steps), but you keep your center of gravity on the pivot foot and "scatter" the other foot to create variations in how you step and move.

![](images/skill_slide.gif)

Slide. Keep the pivot foot fixed while sliding the other foot at regular intervals.

![](images/skill_crossturn.gif)

Cross turn. Cross both feet, then spin using centrifugal force.

They may look difficult, but they're easy to learn. DDS is a game, not dance, so **as long as you can move your feet, that's enough**. None of the "dance craft" like upper-body styling or isolation is required.

Also, these movements are strictly rhythmic, and the subdivisions are either quarter notes (the speed of clapping) or eighth notes (twice the speed of clapping). In most rhythm games, sixteenth notes or thirty-second notes are common, and handling them requires aptitude and training in terms of mental processing capacity. As a result, rhythm games have a high barrier to entry and only appeal to a niche audience, mostly younger enthusiasts.

I want to change this. Like a batting cage, I want to make a rhythm game that anyone can enjoy. If it's no faster than eighth notes, you can process it without special aptitude or training. (Unless you have serious issues with rhythm.) It's the same reason anyone can clap along.

### 3: It won't be nonstop
For example, if a song is 2 minutes long, conventional rhythm games basically make you process notes for the full 2 minutes without rest. It demands not "game" effort but athletic effort, like endurance running. To do this consistently, you have to stay highly relaxed, which takes years of training.

DDS is different. If a song is 2 minutes long, the actual processing time will be less than half. For example, only the chorus, or only three parts: the intro, the chorus, and the final section. DDS is based on shuffle-dance-style movement, and these movements are explosive and can't be sustained for long. So we boldly include more breaks.

DANCERUSH gave a hint here. DANCERUSH STARDOM is an innovative rhythm game based on shuffle dance, but it makes you process continuously for 2 minutes. That raised the psychological hurdle for players. DDS won't repeat the same mistake.

## 📍Chart structure

### Waiting, low-effort, processing
In DDS, there are three types of player movement. These are separated into parts.

- Waiting part: A period where you do not process any notes at all. A break.
- Low-effort part: A period where you process very simple notes without using shuffle dance movements.
- Processing part: A period where you process notes using shuffle dance movements.

In other words, a **chart (all notes for a song)** is made up of three parts: waiting, low-effort, and processing. For example, a 2-minute song might be:

- 15 seconds of waiting part
- 30 seconds of processing part
- 15 seconds of waiting part
- 30 seconds of processing part
- 15 seconds of low-effort part

Of course, you can't keep going if you chain processing parts, so a typical structure is to sandwich processing parts between waiting or low-effort parts.

### Four processing lengths
There are four types: 15 seconds (Short), 30 seconds (Middle), 45 seconds (Long), and 60 seconds (Super Long). If something falls between these 기준, round up to the one above. So 17 seconds becomes Middle, and 35 seconds becomes Long.

DDS uses shuffle dance movements, which are explosive, so normally it uses up to Middle. But for advanced players, Long and Super Long can also be used. With these, your stamina typically won't last if you just move normally, so deliberate rest and energy-saving strategies are required. In other words, Long and Super Long are for advanced players.

This way, DDS can adjust difficulty based on the length of the processing part.

Examples:

- Short
    - [Burn!!! #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=69Zq67DkCCQ)
- Middle
    - [We Are Us(IOSYS TRAX Remix) Running Man chart #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=j_mkKaCoEiY)
- Long
    - [Gargoyle #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/shorts/xFyMxRwRw28)
- Super Long
    - [Restart #Double-sided #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=zt7vZzEetUU)

## 📍Notes and judgment
First is "step judgment." You could also call it **position judgment**. Like Osu! or Synchronica, it's the judgment of stepping on notes displayed on the screen (on the ground). However, the notes will be large enough that even beginners won't easily miss them.

Next is **shuffle (shuffling-step) judgment**. DDS is shuffle-dance-like, and shuffle means shuffling your feet, so that needs to be judged. This checks whether, "at quarter-note or eighth-note subdivisions, the position of the foot is changing **while remaining in contact with the ground**."

Additionally, there is **facing-direction judgment**. This judges which direction the player is facing. There are up, down, left, and right. Whether to judge by torso/face or by toes will need to be tested.

So the balance is:

- Judge by position
- But make the position judgment range wider so it's easy for beginners to step on
- In exchange, add shuffle judgment and facing-direction judgment as shuffle-dance elements

This makes it possible to achieve both uniqueness as a game and a difficulty level that beginners can process.

## 📍Feasibility
I'm not a specialist engineer or planner, so I can't guarantee feasibility at the level of a formal report. However, I feel the pieces are already on the table.

Even looking at [Feasibility considerations by ChatGPT 5.2Pro](https://chatgpt.com/share/6973e68f-ea10-8007-b609-a518a466bc1a), it seems fully workable with enough trial and error.

Personally, I think as follows:

- The conceptual and technical feasibility as a rhythm game is already covered by Osu!, DANCERUSH, and motion capture
- As for the business model:
    - It should be installed in arcades (game centers) and amusement facilities, targeting people who want to move their bodies rather than core rhythm-game users
    - Whether it's better for adults or kids can't be known without testing. Personally, it feels like it would resonate more with kids, but licensing songs would be stricter and more expensive. For adults, people can still enjoy non-licensed original tracks, so it can be cheaper (major rhythm games already do this)
    - Embarrassment can be avoided depending on presentation. Nobody is embarrassed by batting cages or bowling. More important is avoiding the situation where "there are lots of advanced players, so beginners feel unwelcome." We need an idea here, such as separating cabinets into "beginner-rate only" and "intermediate-and-up only (after you graduate from the beginner bracket)"
    - Pricing and play time can only be determined by testing. To start, 1 credit = 100 yen and 2-3 songs seems fine. Or a time-based model like "play all you can for n minutes" might be better
    - If possible, provide a recording feature or motion feature for intermediate-to-advanced players. It would be great if light users (not just core rhythm-game players) could share on social media. Not necessarily "social-media-worthy," but sharing on social media becomes word of mouth

## Closing
I introduced DDS, a new rhythm game idea.

What do you think? Please give it a try. Or you can hire me.

Contact me here: [Contact - stao](https://scrapbox.io/stao/%E3%81%8A%E5%95%8F%E3%81%84%E5%90%88%E3%82%8F%E3%81%9B)