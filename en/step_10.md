## Prepare the first dish

Code the bowl first so you can test one working dish before copying its scripts.

<h2 class="c-project-heading--explainer">What you need to do</h2>

The starter project names this sprite `bowl` and its costumes `bowl 1` to `bowl 6`. The dirty bowl is costume number `1`, and the sparkling-clean bowl is costume number `6`.

![The bowl costumes from filthy to sparkling clean.](images/bowl-cleaning-states.png)

## Step 1

Select the `bowl` sprite in the Sprite pane. Add a `when green flag clicked`{:class="block3events"} block with a `hide`{:class="block3looks"} block.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
+when green flag clicked
+hide
```

## Step 2

Start another script on the `bowl` sprite with a `when I receive ()`{:class="block3events"} block. Choose the `bowl` broadcast that you created earlier.

Switch the sprite to costume number `1` so that the dirty bowl appears in the sink.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
+when I receive (bowl v)
+switch costume to (1)
+set [clean v] to [false]
+set size to (0) %
+go to x: (0) y: (-120)
+show
+set drag mode [not draggable v]
```

## Check your code

Check that the bowl message switches to costume `1`, resets `clean`, and starts the bowl at size `0` and position `(0, -120)`. You will make it grow and rise out of the sink next.
