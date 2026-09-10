## Start the playlist loop

Keep the music player running and wrap back to the first song after song three.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Start another script on the Stage with a `when I receive ()`{:class="block3events"} block, and choose the `play music` message. Add an empty `forever`{:class="block3control"} loop.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
+when I receive (play music v)
+forever
end
```

## Step 2

At the top of the `forever`{:class="block3control"} loop, check whether the song number is greater than `3`. If it is, reset `song`{:class="block3variables"} to `1` so that the music starts again from the first song.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when I receive (play music v)
forever
+if <(song) > (3)> then
+set [song v] to (1)
end
end
```

## Tip

A **rollover check** looks for a number that has gone past the last option and sends it back to the start. Here, a song number greater than `3` rolls over to `1`.

## Check your code

Check that the song-number test sits inside the `forever`{:class="block3control"} loop and resets any value greater than `3` to `1`. Keep the project stopped while the loop has no sound blocks.
