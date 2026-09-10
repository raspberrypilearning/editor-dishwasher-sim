## Set up the music

Choose a starting song and volume when the game begins.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Select the Stage, then make these variables **for all sprites** from the `Variables`{:class="block3variables"} blocks menu:

- `song`{:class="block3variables"} — this stores which song is playing. **Untick this variable.**
- `music volume`{:class="block3variables"} — this stores how loud the music should be. Leave this variable ticked so it appears on the Stage.

<p align="center"><img src="images/music-volume.png" alt="The music volume variable ticked in the Variables menu." width="240" height="66" style="object-fit: contain;"></p>

## Step 2

Keep the Stage selected. Add the music setup blocks near the start of its `when green flag clicked`{:class="block3events"} script, before the random dish broadcast.

In the `broadcast ()`{:class="block3events"} block, choose **New message** and create a broadcast called `play music`.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when green flag clicked
set [clean plates v] to (0)
set [clean v] to [false]
set [soap v] to [false]
+set [song v] to (pick random (1) to (3))
+set [music volume v] to (25)
+broadcast (play music v)
broadcast (item (pick random (1) to (length of [stuff v])) of [stuff v])
```

## Now run your code

Click the green flag. The `music volume`{:class="block3variables"} readout should show `25`, and the dishwashing game should still work. You will add the music player next.
