## Check whether the dish is clean

Start the cloth costume script with a check for a clean dish.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Select the `cloth1` sprite in the Sprite pane. Add another script that starts by showing the dry cloth.

<img src="images/cloth-thumb.png" alt="The cloth sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
+when green flag clicked
+forever
+switch costume to (cloth1 v)
end
```

## Step 2

Replace the `switch costume to (cloth1 v)`{:class="block3looks"} block with an `if () then else`{:class="block3control"} block. Keep the dry cloth in the `else`{:class="block3control"} branch.

<img src="images/cloth-thumb.png" alt="The cloth sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when green flag clicked
forever
+if <(clean) = [true]> then
else
switch costume to (cloth1 v)
end
end
```

## Now run your code

Click the green flag. The cloth should follow the mouse pointer in its dry costume. The clean-dish branch is empty for now.
