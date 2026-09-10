## Check for soap before scrubbing

Allow scrubbing only when the player has soap, and stop at the clean costume.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Inside the `if () then`{:class="block3control"} block, add an `if () then else`{:class="block3control"} block. Check whether the player has picked up soap. Leave both branches empty for now.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when this sprite clicked
if <(clean) = [false]> then
+if <(soap) = [true]> then
else
end
end
```

## Step 2

In the soap branch, add a `repeat until ()`{:class="block3control"} loop. Make it stop when the bowl reaches costume number `6`.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when this sprite clicked
if <(clean) = [false]> then
if <(soap) = [true]> then
+repeat until <(costume [number v]) = (6)>
end
else
end
end
```

## Check your code

Keep the project stopped while this loop is incomplete. Check that the `repeat until`{:class="block3control"} loop is inside the `soap = true` branch and checks for costume `6`. The next step adds the blocks that let it finish.
