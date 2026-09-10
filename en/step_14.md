## Scrub through the costumes

Use the mouse button to move through the dirty-to-clean costumes with cleaning sounds.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Inside the new loop, wait until the player is pressing the mouse button.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when this sprite clicked
if <(clean) = [false]> then
if <(soap) = [true]> then
repeat until <(costume [number v]) = (6)>
+wait until <mouse down?>
end
else
end
end
```

## Step 2

Under the `wait until ()`{:class="block3control"} block, play a random cleaning sound, move to the next costume, and add a short delay.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when this sprite clicked
if <(clean) = [false]> then
if <(soap) = [true]> then
repeat until <(costume [number v]) = (6)>
wait until <mouse down?>
+start sound (pick random (1) to (4))
+next costume
+wait (0.2) seconds
end
else
end
end
```

## Now run your code

Click the green flag, click the soap, then click and hold the bowl. It should play cleaning sounds and stop on costume `6`. The hand will not appear until you mark the dish as clean in the next step.
