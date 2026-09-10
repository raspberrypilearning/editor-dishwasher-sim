## Bring the bowl out of the sink

Animate the dirty bowl, then wait for the player to clean it.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Add a loop to the same script to make the bowl rise out of the sink.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when I receive (bowl v)
switch costume to (1)
set [clean v] to [false]
set size to (0) %
go to x: (0) y: (-120)
show
set drag mode [not draggable v]
+repeat (20)
+change y by (6)
+change size by (6)
end
```

## Step 2

Add blocks to the bottom of the same script to wait until the bowl is clean. In the `broadcast ()`{:class="block3events"} block, choose **New message** and create a broadcast called `clean`.

<img src="images/bowl-thumb.png" alt="The bowl sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when I receive (bowl v)
switch costume to (1)
set [clean v] to [false]
set size to (0) %
go to x: (0) y: (-120)
show
set drag mode [not draggable v]
repeat (20)
change y by (6)
change size by (6)
end
+wait until <(clean) = [true]>
+broadcast (clean v)
```

## Tip

The bowl starts tiny and grows as it rises out of the sink.

## Now run your code

<img src="images/bowl-costume-1.png" alt="The dirty bowl sprite." width="138" height="105" style="object-fit: contain;">

Click the green flag. The dirty bowl should appear in the middle of the sink.
