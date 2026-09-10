## Complete the playlist

Play the third song and move to the next track after each song finishes.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

In the final `else`{:class="block3control"} branch, add a block that plays `song3` until it finishes.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when I receive (play music v)
forever
if <(song) > (3)> then
set [song v] to (1)
end
if <(song) = (1)> then
play sound (song1 v) until done
else
if <(song) = (2)> then
play sound (song2 v) until done
else
+play sound (song3 v) until done
end
end
end
```

## Step 2

At the bottom of the `forever`{:class="block3control"} loop, add a `change () by ()`{:class="block3variables"} block. This moves to the next song after one finishes.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when I receive (play music v)
forever
if <(song) > (3)> then
set [song v] to (1)
end
if <(song) = (1)> then
play sound (song1 v) until done
else
if <(song) = (2)> then
play sound (song2 v) until done
else
play sound (song3 v) until done
end
end
+change [song v] by (1)
end
```

## Now run your code

Click the green flag. One of the three songs should start. When it finishes, the next song should play; after song three, the playlist should return to song one.
