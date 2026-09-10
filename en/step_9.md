## Show the soapy cloth

Use the soap variable to choose between the dry and soapy cloth costumes.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Inside the `else`{:class="block3control"}, add another `if () then else`{:class="block3control"} block to check whether the player has picked up soap. Keep the dry cloth in the new `else`{:class="block3control"} branch.

<img src="images/cloth-thumb.png" alt="The cloth sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when green flag clicked
forever
if <(clean) = [true]> then
switch costume to (hand v)
else
+if <(soap) = [true]> then
else
switch costume to (cloth1 v)
end
end
end
```

## Step 2

Add a `switch costume to ()`{:class="block3looks"} block inside the soap branch to show the soapy cloth.

<img src="images/cloth-thumb.png" alt="The cloth sprite thumbnail." width="138" height="105" style="object-fit: contain;">

```blocks3
when green flag clicked
forever
if <(clean) = [true]> then
switch costume to (hand v)
else
if <(soap) = [true]> then
+switch costume to (cloth2 v)
else
switch costume to (cloth1 v)
end
end
end
```

## Tip

**Visual feedback** shows the player that an action worked. Changing the cloth costume makes it clear when the player has picked up soap.

## Now run your code

<p align="center"><img src="images/soap.png" alt="The soap sprite." width="150" height="120" style="object-fit: contain;"></p>

Click the green flag, then click the soap on the Stage. The soap should pulse gently, and the cloth should change to the soapy costume.
