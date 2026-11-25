# Status: Quiet Crossing

Last updated: 2026-11-25. Playable prototype, first release.

## What exists
- A complete loop: title, intro, eight crossings with eight passengers, stars per crossing, a Ferry log at the end.
- One file, `index.html`. Canvas 2D, procedural WebAudio sound, art drawn by code.
- Public on GitHub (this repo, with Pages) and itch.io. Code is MIT. Screenshots, cover and trailer are CC BY-NC-SA 4.0.

## Tested
- Scripted bot, stepped deterministically through all eight crossings: every crossing is completable, results vary (one failure and several 1-star results appeared), each crossing lasted 7 to 21 seconds of game time. This was used to raise some later currents and enlarge the boat. It says nothing about how it feels.
- Real browser input in headless Chrome: real keyboard (Space to advance, arrow keys to row) finished a crossing with calm 84 and 3 stars. Real mouse (click to advance, taps on the left and right half) finished a crossing with calm 100 and 3 stars. No page errors in either run.

## Hosted check (GitHub Pages)
- Opened https://maficonstruct.github.io/quiet-crossing/ in a remote desktop Chrome, advanced with real taps, rowed with alternating taps on the left and right half: crossing 1 completed (0 stars, my taps were not tuned) and crossing 2 started.
- In a 390x844 phone-sized viewport the title screen renders, but the 16:9 canvas is letterboxed small in portrait. Landscape is recommended. Not fixed.

## Not tested
- Fun, difficulty and pacing with a human player.
- Sound on a real device (the audio code runs, nobody has listened).
- Touch on a phone or tablet.
- Other browsers than Chrome.

## Retake signal
A report of where it feels too hard, too easy or broken, with device and browser. Nothing else is planned.
