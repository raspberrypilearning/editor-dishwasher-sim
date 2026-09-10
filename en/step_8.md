## Show a hand for clean dishes

Show the hand costume when a dish is ready to move.

<h2 class="c-project-heading--explainer">What you need to do</h2>

Add a `switch costume to ()`{:class="block3looks"} block inside the first branch to show the hand when the dish is clean.

<img src="images/cloth-thumb.png" alt="The cloth sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when green flag clicked
forever
if <(clean) = [true]> then
+switch costume to (hand v)
else
switch costume to (cloth1 v)
end
end
```

## Now run your code

Click the green flag. The dry cloth should still appear because `clean`{:class="block3variables"} starts as `false`. The hand will appear when your scrubbing code sets it to `true`.
