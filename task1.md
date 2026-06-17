# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Introduction @showdialog

# Raise Tower Bridge Workshop

You are an engineer working at **Tower Bridge**.

Large ships need to pass safely along the River Thames.

Your job is to program the bridge so the bascules can rise and lower at the right time.

Work carefully, test your code, and talk with your team.

## Task 1 Video @showdialog

Watch the video for Task 1.

![Random Video 1](youtube:65ivoafQnzw)

## Task 1: Raise and lower the bridge

![Random picture 1](https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/rand_pic1.JPG)

Make the bridge respond to the micro:bit buttons.

Button **A** should raise the bridge.

## Step 1: Look at button A

Find the code for **button A**.

It already raises the **left** side of the bridge.

## Step 2: Raise the right side

Add a block under it.

Make **button A** raise the **right** side too.

## Step 3: Look at button B

Find the code for **button B**.

It already lowers the **left** side of the bridge.

## Step 4: Lower the right side

Add a block under it.

Make **button B** lower the **right** side too.

## Step 5: Test your code

Press **A** and **B** to test the bridge.

```blocks
input.onButtonPressed(Button.A, function () {
    towerBridge.raiseLeftBascule()
    towerBridge.raiseRightBascule()
})
input.onButtonPressed(Button.B, function () {
    towerBridge.lowerLeftBascule()
    towerBridge.lowerRightBascule()
})
```

## Finish @showdialog

Great work, engineer!

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task2)

```template
input.onButtonPressed(Button.A, function () {
    towerBridge.raiseLeftBascule()
})
input.onButtonPressed(Button.B, function () {
    towerBridge.lowerLeftBascule()
})
```
