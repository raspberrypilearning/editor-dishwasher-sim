## Make the skip button clickable

Keep the skip button in place and send a message when the player clicks it.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Select the `skip` sprite in the Sprite pane. Add a script that prevents the player from dragging the button.

<img src="images/skip-thumb.png" alt="The skip sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
+when green flag clicked
+set drag mode [not draggable v]
```

## Step 2

Keep the `skip` sprite selected. Add another script that broadcasts the `skip` message when the player clicks the button on the Stage.

<img src="images/skip-thumb.png" alt="The skip sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
+when this sprite clicked
+broadcast (skip v)
```

## Now run your code

Click the green flag and try the skip button. It should stay in place when dragged. It will change the song after you add the message receiver next.
