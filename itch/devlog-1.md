# Devlog 1: one mechanic, eight passengers

I wanted to make something small and quiet after a prototype full of physics. The idea: you row a boat, and the only thing that matters is how calmly you do it.

## The mechanic

You alternate left and right strokes. Each stroke pushes the boat forward and turns it a little to the other side. If you stroke the same side twice, you mostly just turn. A river current pushes you sideways, and it gets stronger in the later crossings. Rocks and floating logs get in the way, and from the sixth crossing there is fog.

## Calm

Every crossing has one passenger with one thing they mind. Each trait is a small rule on top of the same boat:
- bumps cost calm (the baker takes double),
- sharp turns cost calm (the goat),
- speed costs calm (the cellist),
- same-side strokes cost calm (the twins),
- slow trips cost calm (the courier),
- the last two passengers count everything.

Calm recovers slowly when nothing upsets anyone. The stars at the end of a crossing come from the calm you arrive with.

## Everything is generated

There are no image or sound files. The boat, water, rocks, dock lamps, fog and passengers are drawn with canvas calls, and the water sound and strokes are synthesized with WebAudio. The whole game is one HTML file of about 25 KB.

## How I checked it

A scripted bot rows all eight crossings with the game stepped by hand, so every run is the same. It found that the later currents were too weak and the boat too small to read, so I raised the currents and drew the boat larger. After that every crossing was completable and results still varied: some one-star crossings, one failure.

Then I ran real key presses and real mouse clicks in headless Chrome: Space moved from the title to the intro to the crossing, arrow keys finished one crossing with 3 stars, and clicks finished another. No page errors. I keep these two kinds of test apart, because a bot says whether the rules work, not whether rowing feels good.

## Not tested

No human has played it. I have not heard the sound on a real device, and touch on a phone is untested. If it feels too hard or too easy, that is the useful report.

## Next

Depends on what people say. Possible: more passengers, a calmer first level, a way to see the current.
