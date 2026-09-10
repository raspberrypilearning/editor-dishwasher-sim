## Play the first song

Play song one when its number is selected.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Beneath that check, add an `if () then else`{:class="block3control"} block. Check whether `song`{:class="block3variables"} is `1`. Leave both branches empty for now.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when I receive (play music v)
forever
if <(song) > (3)> then
set [song v] to (1)
end
+if <(song) = (1)> then
else
end
end
```

## Step 2

In the first branch, add a block that plays `song1` until it finishes.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when I receive (play music v)
forever
if <(song) > (3)> then
set [song v] to (1)
end
if <(song) = (1)> then
+play sound (song1 v) until done
else
end
end
```

## Now run your code

To test this branch, temporarily replace the random starting song in the Stage setup script with `1`. Click the green flag and listen for `song1`. Restore the random-number block after the test.
