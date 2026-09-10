## Put away the bowl and score

Shrink the bowl when it touches the rack, then count it as a clean plate.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Continue the same script. Wait until the bowl touches the `rack` sprite, then shrink the bowl so it looks as though it has been put away.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when I receive (clean v)
start sound (Coin v)
set [soap v] to [false]
set drag mode [draggable v]
+wait until <touching (rack v)?>
+repeat (60)
+change size by (-2)
end
```

## Step 2

Add blocks to score the clean bowl, hide it, and reset it ready for another round.

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
+change [clean plates v] by (1)
+hide
+set size to (0) %
+go to x: (0) y: (-140)
+set [clean v] to [false]
```

## Now run your code

Click the green flag, use the soap, scrub the bowl, and drag it into the rack. The bowl should shrink and disappear, and the `clean plates`{:class="block3variables"} score should increase by `1`.

The bowl will not reappear until you add the next-dish broadcast in the following step.
