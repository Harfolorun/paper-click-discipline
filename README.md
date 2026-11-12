# Paper Click-Discipline

An **aim trainer** for your **sense of rhythm**, built as a browser game for PC. A metronome ticks, and your job is to click the target **on the beat**. Not faster, not slower. Accurate clicks at the wrong moment don't count, and neither do clicks in time that miss the target.

Everything is in one HTML file: the art, the font and the sounds.

---

## How to play

1. **Sync!** Calibrate your audio first (see [Calibration](#calibration)).
2. **Pick your options** on the left: metronome sound, volume, target size and click timing.
3. **Start a game** in one of two ways:
   - **Play!** Type a BPM in the box and press Play!. The button counts down 4 beats (one bar of 4/4), then the game starts.
   - **Tap!** Put on any song and click Tap! 10 times along with its beat. The game measures the tempo from your taps and starts right on the next beat, with the metronome locked to your music.

A game lasts **60 seconds**. Each time you hit a target on the beat, a new one appears somewhere else on the paper. Press **Esc** to quit a game early.

### What the marks mean

| Mark | Meaning |
|---|---|
| Green dot with points | On the beat and on the target |
| Red **×** with penalty | On the beat, but you missed the target |
| Red **o** with "early" / "late" | You clicked out of tempo |

## Scoring

| | Points |
|---|---|
| Base hit | **+100** |
| Base miss | **−25** |

Both are multiplied by your current modifiers:

**Target size**

| Huge | Medium | Small | Tiny |
|---|---|---|---|
| ×1 | ×1.25 | ×1.5 | ×1.75 |

**Streak.** Every 5 on-time hits in a row add +0.25 to your streak bonus. The total multiplier is *size × (1 + streak bonus)*: on Small with 10 hits in a row, that's 1.5 × 1.5 = ×2.25. The Streak display shows this total.

A miss, an out-of-tempo click or a skipped beat breaks the streak and costs a penalty at your multiplier just before the break. Losing a big streak hurts!

## Options

- **Metronome:** Classic, Digital, Clock or Sticks. Click one to hear a preview.
- **Volume:** the slider under the metronome sounds.
- **Target Size:** Huge, Medium, Small or Tiny.
- **Click Timing:** how close to the beat a click must be to count as on time: **±100 ms**, **±70 ms** or **±40 ms**.

Your settings, your highest score and your last games are saved in your browser on your computer.

## Statistics

The **Score screen** after each game shows:

- **Score** and **Top Streak:** the highest multiplier you reached.
- **Tempo:** what share of your clicks were Early, Perfect or Late.
- **Targets:** Accuracy, the share of clicks that landed on the target.
- **Misses:** how your misses split into **Under** (stopped short), **Over** (flicked too far) and **Side** (off to the side). Each miss is measured along the line from your previous click to the target.

The note on the right shows the same numbers **averaged over your last 10 games**, and the bottom of the page shows your **Highest Score**.

## Calibration

Headphones, speakers and screens all add small delays, and so does your own habit of clicking a little early or late. **Sync!** measures this so the game judges your timing fairly:

1. Click **Sync!**. The game says **Listen!** while the metronome plays 4 clicks.
2. When it says **Click to the beat!**, click along with the metronome 16 times. The button counts down.
3. Your offset appears under the button, for example `-42ms`.

Redo it whenever you change headphones or speakers. Bluetooth headphones add a lot of delay, so wired ones give the most stable timing.

**Audio debug readout:** press **D** to show or hide audio timing details: reported latency, clock jitter, drift over the last 10 seconds, and clicks that played too late. Useful for comparing headphones or troubleshooting.

## Requirements

- A **PC with a mouse**. The game isn't made for touchscreens.
- A modern desktop browser: Chrome, Edge or Firefox.
- Sound on. Headphones are recommended.

## Running it

- **Online:** at https://harfolorun.github.io/paper-click-discipline
- **Locally:** download `index.html` and open it in your browser. That's it.

## Credits

- **Idea, design and art:** made by Harfo L'Orun.
- **Metronome sounds (Classic, Clock, Sticks):** edited and processed by Harfo L'Orun, based on sounds by **freesound community** and **Dragon Studio** via [Pixabay](https://pixabay.com/), used under the [Pixabay Content License](https://pixabay.com/service/license-summary/).
- **Code and the Digital metronome sound:** made by AI (Anthropic's Claude).
- **Font:** [Nunito](https://github.com/googlefonts/nunito) by Vernon Adams and the Nunito Project Authors, under the SIL Open Font License 1.1.

## License

© 2026 Harfo L'Orun. **All rights reserved.**

**Paper Click-Discipline is free to play.** Anyone may play it for free, online or from a downloaded copy, for personal use.

Except for viewing and forking on GitHub as allowed by GitHub's Terms of Service, you may not copy, modify, redistribute or sell the game or any part of it, including its art and sounds, without the author's permission.

Third-party parts keep their own licenses:

- **Nunito font:** SIL Open Font License 1.1.
- **Original sounds** behind the edited metronome sounds: Pixabay Content License.
