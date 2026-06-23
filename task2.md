# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Introduction @showdialog

# Task 2: Stop the Bridge

Great work! Your bridge can open and close.

But a real bridge should not move forever.

In this task, make the bridge move for a short time, then stop.

## Step 1

Press **A** or **B**.

Does the bridge stop by itself?

## Step 2 @showdialog

# Add a pause

A pause makes the program wait.

This block waits for **2000 ms**, which is **2 seconds**.

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_pause.png" height="200px">

## Step 3

Add a **pause** after the bridge starts moving.

Use **2000 ms**.

## Step 4 @showdialog

# Stop the motors

To stop a bascule, set its speed to **0**.

Do this for both the left and right bascules.

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_stop.png" height="200px">

## Step 5

After the pause, set both speeds to **0**.

This stops the bridge.

## Step 6

Do the same for button **B**.

Then test both buttons.

```blocks
input.onButtonPressed(Button.A, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Raise)
    basic.pause(2000)
    towerBridge.setBasculeMotorSpeed(BridgeSide.Left, 0)
    towerBridge.setBasculeMotorSpeed(BridgeSide.Right, 0)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Lower)
    basic.pause(2000)
    towerBridge.setBasculeMotorSpeed(BridgeSide.Left, 0)
    towerBridge.setBasculeMotorSpeed(BridgeSide.Right, 0)
})
```

## Finish @showdialog

Great work, engineer!

Now your bridge can move and stop safely.

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task3)

```template
input.onButtonPressed(Button.A, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Raise)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Lower)
})
```
