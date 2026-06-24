# Raise Tower Bridge

### @hideDone true

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

## Introduction @showdialog

# Task 3: Choose the Height

Different ships need different bridge heights.

A small ship only needs a small opening.

A taller ship needs a bigger opening.

## Step 1 @showdialog

# Bridge angles

The bridge is closed at **0°**.

It opens higher at **30°** and **60°**.

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_0deg.JPG" height="160px">
<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_30deg.JPG" height="160px">
<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_60deg.JPG" height="160px">

## Step 2

Press **A**.

The bridge opens to **30°**.

## Step 3

Find the code for button **B**.

Change **0°** to **60°**.

## Step 4

Press **B**.

The bridge should open higher.

## Step 5

Add code for **A+B**.

Close the bridge to **0°**.

## Step 6

Test all buttons.

A: 30°, B: 60°, A+B: 0°.

```blocks
input.onButtonPressed(Button.A, function () {
    basculeMotors.moveBasculeTo(BridgeSide.Left, 30)
    basculeMotors.moveBasculeTo(BridgeSide.Right, 30)
})
input.onButtonPressed(Button.B, function () {
    basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
    basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
})
input.onButtonPressed(Button.AB, function () {
    basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
    basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
})
```

## Finish @showdialog

Great work, engineer!

Now your bridge can open to different heights.

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task4)

```template
input.onButtonPressed(Button.A, function () {
    basculeMotors.moveBasculeTo(BridgeSide.Left, 30)
    basculeMotors.moveBasculeTo(BridgeSide.Right, 30)
})
input.onButtonPressed(Button.B, function () {
    basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
    basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
})
input.onButtonPressed(Button.AB, function () {
})
```
