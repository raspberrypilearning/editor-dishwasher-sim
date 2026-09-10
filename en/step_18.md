## Bring out the next dish

Choose another dirty dish after the player puts a clean one away.

<h2 class="c-project-heading--explainer">What you need to do</h2>

At the bottom of the script, broadcast a random item from the `stuff`{:class="block3variables"} list. Using the list's length means this block will keep working after you add more dishes.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when I receive (clean v)
start sound (Coin v)
set [soap v] to [false]
set drag mode [draggable v]
wait until <touching (rack v)?>
repeat (60)
change size by (-2)
end
change [clean plates v] by (1)
hide
set size to (0) %
go to x: (0) y: (-140)
set [clean v] to [false]
+broadcast (item (pick random (1) to (length of [stuff v])) of [stuff v])
```

## Now run your code

Click the green flag. Use the soap, scrub the bowl, then drag it into the rack. The score should increase and a new dirty bowl should rise from the sink.

<img src="images/bowl-costume-1.png" alt="The dirty bowl sprite." width="138" height="105" style="object-fit: contain;">
