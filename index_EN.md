# DDS - DanceDanceShuffle
[Japanese](index.md) | [English](index_EN.md) | [GitHub](https://github.com/stakiran/dds)

A new rhythm game concept that combines dance pad gameplay with shuffle dance

![](images/demo.gif)

## 📍Overview
DDS is an idea for a new rhythm game.

### 1: A full 2D field on the floor
![](images/260124_053608.png)

**Notes are displayed and processed on the floor**. Like Osu! and Synchronica, it uses the entire two-dimensional field.

![](images/leftright.gif)

The field is wide horizontally, and you move left and right across it as shown. This is because shuffle-dance-style movement is the core of the game.

![](images/updown.gif)

The field also has depth, to add variation in where you place your feet.

### 2: Dynamic, but easy moves
The moves used in DDS are based on shuffle dance. They're dynamic, and fun both for the person playing and for anyone watching.

Main moves include:

![](images/skill_rm.gif)

Running Man. Pull each foot back twice.

![](images/skill_ts.gif)  

T-step. Move while swinging your pivot foot like a pendulum.

![](images/skill_shufflestomp.gif)

Shuffle Stomp. Basically stomping in place (alternating steps), but you keep your center of gravity on the pivot foot and "scatter" the other foot, creating variety in both how you step and how you move.

![](images/skill_slide.gif)

Slide. Keep the pivot foot fixed while sliding the other foot at equal intervals.

![](images/skill_crossturn.gif)

Cross Turn. Cross your legs, then spin using centrifugal force.

They may look difficult, but they're easy to learn. DDS is a game, not dance, so **as long as you can move your feet, that's enough**. None of the "dance work" like upper-body styling or isolation is required.

Also, these moves are strictly rhythmic, and the subdivisions are either quarter notes (the speed of clapping) or eighth notes (twice the speed of clapping). Most rhythm games typically focus on speeds like 16th or 32nd notes, which require aptitude and training in terms of brain processing capacity to handle. As a result, rhythm games have a high barrier to entry and only appeal to a niche audience, mainly younger enthusiasts.

I want to change that. Like a batting cage, I want to make a rhythm game that everyone can enjoy. If it's no faster than eighth notes, you can process it without special aptitude or training. It's the same as how anyone can clap along (except people who have trouble with rhythm).

### 3: No nonstop play
For example, with a 2-minute song, conventional rhythm games basically make you keep processing continuously for the full 2 minutes without rest. It demands the kind of sustained suffering you'd expect from sports, like long-distance running. To do this consistently, you have to become highly relaxed, and that takes years of training.

DDS is different. With a 2-minute song, the time spent processing will be less than half. For example, only the chorus, or only three parts like the intro, chorus, and ending. DDS is based on shuffle-dance-style movement, which is explosive and can't be sustained for long. So we boldly include more breaks.

DANCERUSH STARDOM gave me an important hint here. It's an innovative rhythm game based on shuffle dance, but it makes you process constantly for 2 minutes. That raised the psychological hurdle for players. I won't make the same mistake.

## 📍Chart structure

### Idle, light, and processing
In DDS, there are three types of player movement. We distinguish them as parts.

- Idle part: A period where you do not process notes at all. Rest
- Light part: A period where you do very simple processing without using shuffle dance moves
- Processing part: A period where you process using shuffle dance moves

In other words, a **chart (the full set of notes for a song)** is made up of three parts: idle, light, and processing. For example, a 2-minute song might be structured like:

- 15 seconds of idle part
- 30 seconds of processing part
- 15 seconds of idle part
- 30 seconds of processing part
- 15 seconds of light part

Of course, you can't keep your stamina if processing parts continue back-to-back, so a typical structure is to sandwich processing parts between idle parts or light parts.

### Four types of processing by length
There are four types: 15 seconds (short), 30 seconds (middle), 45 seconds (long), and 60 seconds (super long). Anything that falls between these 기준 is rounded up to the next one. So 17 seconds of processing is middle, and 35 seconds is long.

DDS uses shuffle dance moves, but since they're explosive, normally we use up to middle. However, for advanced players, long and super long can also be used. With those, your stamina usually won't last if you just move normally, so intentional rest and energy-saving strategies are required. In other words, long and super long are for advanced players.

In this way, DDS can adjust difficulty according to the length of the processing parts.

Examples:

- Short
    - [Burn!!! #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=69Zq67DkCCQ)
- Middle
    - [We Are Us(IOSYS TRAX Remix) Running Man chart #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=j_mkKaCoEiY)
- Long
    - [Gargoyle #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/shorts/xFyMxRwRw28)
- Super long
    - [Restart #double-sided #DDS #DanceDanceShuffle - YouTube](https://www.youtube.com/watch?v=zt7vZzEetUU)

## 📍Notes and judgments
First is the "step judgment." You could also call it **position judgment**. Like Osu! and Synchronica, it's a judgment where you step on notes displayed on the screen (on the floor). However, the notes will be large enough that even beginners won't miss them.

Next is **shuffling judgment**. DDS is shuffle-dance-like, and shuffle means shuffling your feet, so this needs to be judged. Specifically, it checks whether "at quarter-note or eighth-note timing, the foot position is changing **while staying in contact with the floor**."

Additionally, there's **direction judgment**. This judges which way the player is facing: up, down, left, or right. Whether this should be judged by torso/face direction or by toe direction will require validation.

So the balance is as follows:

- Judge by position
- But make the position judgment window wide so it's easy to step correctly even for beginners
- In return, also add shuffling judgment and direction judgment to make it shuffle dance

This makes it possible to achieve both uniqueness as a game and a difficulty level that beginners can process.

## 📍Dominant foot
DDS has the concept of a **dominant foot**. In baseball batting there are left/right stances; in soccer, the kicking foot tends to be biased; and even in esports, your mouse hand has a preference. Similarly, DDS has a dominant foot.

The dominant foot is "the foot you step out with first." Or, "the foot that is not the pivot foot." In DDS, you will mainly step with your dominant foot. The opposite pivot foot is often used to support you. By splitting roles this way, you can move stably even when there's nothing else supporting you.

The dominant foot is an essential concept for DDS to work as a game. Therefore, DDS charts will also be built on the assumption of a dominant foot. Concretely, charts will be made for the more common right-dominant players (dominant foot is the right foot), and a mirror option will support left-dominant players (dominant foot is the left foot).

Here's an example. Shuffle Stomp makes the dominant foot easy to understand. Take a look:

![](images/stomps.gif)

This is a stomp chart at BPM 185, and the dominant foot is the right foot. You can see that the stepping is centered on the right foot, while the opposite left foot supports as the pivot foot.

## 📍Feasibility
I'm not a specialist engineer or planner, so I can't guarantee feasibility at the level of a formal report. However, I feel like the pieces are already on the table.

Even looking at [A feasibility discussion by ChatGPT 5.2Pro](https://chatgpt.com/share/6973e68f-ea10-8007-b609-a518a466bc1a), it seems fully workable depending on trial and error.

Personally, I think as follows:

- The conceptual and technical feasibility as a rhythm game is already covered by Osu!, DANCERUSH, and motion capture
- As for the business model:
    - It would be installed in arcades and amusement facilities, targeting people who want to move their bodies rather than core rhythm game users
    - Whether it's better for adults or children can't be known without testing. Personally, I feel it would resonate more with kids, but acquiring licensed songs would be difficult and costly in terms of rights. For adults, people can still enjoy it even with non-licensed songs, so it can be cheaper (major rhythm games already do this)
    - As for embarrassment, it can be avoided depending on the presentation. Nobody is embarrassed by batting cages or bowling. Rather, it's more important to avoid the situation where "there are lots of advanced players, so beginners feel unable to approach." We need to come up with measures for this, such as separating machines into "machines only usable by beginner-rated players" and "machines only usable by intermediate-and-above players who have graduated from the beginner range"
    - Pricing and play time can only be validated through testing. To start, 1 credit for 100 yen and 2-3 songs would be fine. Or a time-based model like "play all you want for n minutes" might be better
    - If possible, provide a recording feature or motion feature for intermediate-to-advanced players. It would be great if light users other than core rhythm game users could share on social media. Not necessarily "Instagrammable," but sharing on social media becomes word of mouth

## Closing
I introduced DDS, a new rhythm game idea.

How does it sound? Please give it a try. Or you can hire me, too.

Contact: [Contact - stao](https://scrapbox.io/stao/%E3%81%8A%E5%95%8F%E3%81%84%E5%90%88%E3%82%8F%E3%81%9B)

## Update history
- 2026-02-15 Added information about the dominant foot
- 2026-01-24 First edition