## Control the music volume

Let the player adjust the music with a slider.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

On the Stage, double-click the `music volume`{:class="block3variables"} variable display until it changes into a slider, then move it to the bottom corner of the stage. The player will be able to drag the slider to change the music volume.

<p align="center"><img src="images/music-volume.png" alt="The music volume variable display on the Stage." width="240" height="66" style="object-fit: contain;"></p>

## Step 2

Keep the Stage selected. Add another script so its sound volume follows the `music volume`{:class="block3variables"} slider while the game runs.

<img src="images/stage.png" alt="The Stage in the Sprite pane." width="82" height="108" style="object-fit: contain;">

```blocks3
+when green flag clicked
+forever
+set volume to (music volume) %
end
```

## Tip

Balancing the volume of music and sound effects is called **audio mixing**. Quieter music leaves room for the cleaning and scoring sounds.

## Now run your code

Click the green flag and drag the volume slider. The music should get quieter or louder while the cleaning sound effects keep their own volume.
