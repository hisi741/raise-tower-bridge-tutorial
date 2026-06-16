# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Task 3 Video @showdialog

Watch the video for Task 3.

![Random Video 3](youtube:65ivoafQnzw)

## Task 3: Use the ship sensor

Now make the bridge work automatically.

If the sensor detects a ship, the bridge should go **up**.

## Step 1: Edit your code

Please set it so that when a ship is detected, both sides of the bridge go **up**.

When there is no ship, both sides of the bridge should go **down**.

## Step 2: Test your code

Use the ship sensor to test your bridge.

Check that the bridge rises and lowers automatically.

```blocks
basic.forever(function () {
    if (towerBridge.shipComing()) {
        towerBridge.raiseLeftBascule()
        towerBridge.raiseRightBascule()
    } else {
        towerBridge.lowerLeftBascule()
        towerBridge.lowerRightBascule()
    }
})
```

## Finish @showdialog

Great work, engineer!

You have programmed Tower Bridge to:

* move with buttons
* move to chosen angles
* react automatically to a ship sensor

Now test your final program on the bridge model.

Can your team make the bridge move smoothly and safely?

[Prev task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task2)

```template
basic.forever(function () {
    if (towerBridge.shipComing()) {
    } else {
    }
})
```
