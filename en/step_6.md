## Make the soap pulse

Return the soap to its starting size after each growing movement.

<h2 class="c-project-heading--explainer">What you need to do</h2>

Beneath the first `repeat ()`{:class="block3control"} loop, add another loop that returns the soap to `30` percent.

Together, the two loops make the soap gently grow and shrink. This draws the player's attention and makes it clear that they can interact with the soap.

<img src="images/soap-thumb.png" alt="The soap sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when green flag clicked
set size to (30) %
forever
repeat (15)
change size by (0.2)
end
+repeat (15)
+change size by (-0.2)
end
end
```

## Tip

To save time, right-click the top block in a group and choose **Duplicate** to copy the whole group. Try this with the `repeat ()` and `change size by ()` blocks, or with an `if () then else` block that already contains its operator and variable. Then change only what needs to be different.

## Now run your code

Click the green flag. The soap should grow and shrink gently instead of getting larger forever.
