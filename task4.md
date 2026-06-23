# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Introduction @showdialog

# Task 4: Emergency Stop

Engineers must think about safety.

A real machine needs a way to stop quickly.

In this task, make **A+B** stop the bridge.

<!-- ## Task 4 Video @showdialog

Watch the video for Task 4.  -->

## Step 1 @showdialog

# Emergency stop

An emergency stop stops a machine quickly.

Press **A+B** to stop both bascules.

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_emergency_stop.JPG" height="220px">

## Step 2

Press **A** to start opening.

Then press **A+B**.

## Step 3

Add a stop block inside **A+B**.

Stop the **left** bascule.

## Step 4

Add another stop block.

Stop the **right** bascule.

## Step 5

Show a warning icon.

Use it after the stop blocks.

## Step 6

Test your emergency stop.

Can you stop the bridge quickly?

```blocks
input.onButtonPressed(Button.A, function () {
    basculeMotors.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
    basculeMotors.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Raise)
})
input.onButtonPressed(Button.B, function () {
    basculeMotors.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
    basculeMotors.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Lower)
})
input.onButtonPressed(Button.AB, function () {
    basculeMotors.stopBasculeMoving(BridgeSide.Left)
    basculeMotors.stopBasculeMoving(BridgeSide.Right)
    basic.showIcon(IconNames.No)
})
```

## Finish @showdialog

Great work, engineer!

Now your bridge has an emergency stop.

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task5)

```template
input.onButtonPressed(Button.A, function () {
    basculeMotors.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
    basculeMotors.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Raise)
})
input.onButtonPressed(Button.B, function () {
    basculeMotors.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
    basculeMotors.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Lower)
})
input.onButtonPressed(Button.AB, function () {
})
```
