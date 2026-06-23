# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Introduction @showdialog

# Task 1: Move the Bridge

You are an engineer at Tower Bridge.

Press the micro:bit buttons and watch what happens.

Your first job is to make both sides of the bridge move.

<!-- ## Task 1 Video @showdialog

Watch the video for Task 1.

How to show video:
<video src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/video/rand_vid1.mp4" controls width="20%" muted playsinline autoplay preload="auto"></video> 
To show image:
<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/rand_pic1.JPG" width="30%"> -->

## Step 1:
Press **A** or **B** on the micro:bit.

What moves?

## Step 2:

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_add.JPG" height="10%"> -->
<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/edample_edit.JPG" height="10%"> -->

Add and edit block to raise the **right** bascule.

## Step 3:

Find the code for **button B**.

## Step 4:

Press **A** and **B** to test the bridge.

```blocks
input.onButtonPressed(Button.A, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Raise)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
    towerBridge.setBasculeMoveDirection(BridgeSide.Right, BasculeDirection.Lower)
})
```

## Finish @showdialog

Great work, engineer!

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task2)

```template
input.onButtonPressed(Button.A, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Raise)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setBasculeMoveDirection(BridgeSide.Left, BasculeDirection.Lower)
})
```
