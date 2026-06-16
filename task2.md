# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Task 2 Video @showdialog

Watch the video for Task 2.

![Random video 2](youtube:65ivoafQnzw)

## Task 2: Choose the bridge height
Now you can choose the angle of the bridge.

Button **A** should raise both sides to the same height.

## Step 1: Edit your code
Please set it so that pressing “A” **raises** both bridges, and pressing “B” **lowers** both bridges.

## Step 2: Test your code
Press **A** to raise the bridge.

Press **B** to lower the bridge.

```blocks
input.onButtonPressed(Button.A, function () {
    towerBridge.setLeftBasculeTo(70)
    towerBridge.setRightBasculeTo(70)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setLeftBasculeTo(0)
    towerBridge.setRightBasculeTo(0)
})
```

## Finish @showdialog

Great work, engineer!

Can your team make the bridge move smoothly and safely?

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task3)

[Prev Task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task1)


```template
input.onButtonPressed(Button.A, function () {
    towerBridge.setLeftBasculeTo(20)
    towerBridge.setRightBasculeTo(50)
})
input.onButtonPressed(Button.B, function () {
    towerBridge.setLeftBasculeTo(-10)
})
```
