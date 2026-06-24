# Raise Tower Bridge

### @hideDone true

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

## Introduction @showdialog

# Task 4: Automatic Bridge

Great work! Your bridge can open to different angles.

Now make the bridge use a sensor.

If a ship is sailing through, the bridge should open.

If there is no ship, the bridge should close.

## Step 1 @showdialog

# The ship sensor

The bridge can check if a ship is sailing through.

This block asks a question: **is there a ship?**

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_ship_sensor.png" height="200px">

## Step 2

Look at the **if** block.

It asks if a ship is sailing through.

## Step 3

Inside **if**, open both bascules to **60°**.

This lets the ship pass.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
    } else {
    	
    }
})
```

## Step 4

Inside **else**, close both bascules to **0°**.

This happens when there is no ship.

## Step 5

Test with the ship.

Ship present: open. No ship: close.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
    } else {
        basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
    }
})
```

## Finish @showdialog

Great work, engineer!

Now your bridge can react to a ship by itself.

[Next task](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task5)

```template
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
    	
    } else {
    	
    }
})
```
