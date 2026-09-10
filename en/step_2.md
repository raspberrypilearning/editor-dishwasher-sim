## Start with a random dish

Reset the game state, then choose the first dish from your list.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Add the script below to the Stage to reset the game. In this project, the `clean`{:class="block3variables"} and `soap`{:class="block3variables"} variables only store `true` or `false`, so initialise both with the Boolean value `false`.

From the menu in the `broadcast ()`{:class="block3events"} block, choose **New message**. Name the new broadcast `bowl`.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
+when green flag clicked
+set [clean plates v] to (0)
+set [clean v] to [false]
+set [soap v] to [false]
+broadcast (bowl v)
```

## Step 2

Replace `bowl` in the `broadcast ()`{:class="block3events"} block with blocks that select a random item from `stuff`{:class="block3variables"}.

There is only one item in the list for now, so this script will always broadcast `bowl`. When you add more items later, the same code will choose between them.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
when green flag clicked
set [clean plates v] to (0)
set [clean v] to [false]
set [soap v] to [false]
+broadcast (item (pick random (1) to (length of [stuff v])) of [stuff v])
```

## Tip

To **initialise** a variable means to give it a starting value. Here, the game starts with a score of `0`, and `clean` and `soap` set to `false`.

## Now run your code

Click the green flag. The `clean plates`{:class="block3variables"} score should start at `0`. The list only contains `bowl`, but the bowl will not respond to its message until you add its scripts.
