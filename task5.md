# Raise Tower Bridge

### @hideDone true

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

## Introduction @showdialog

# Task 5: Upgrade Your Bridge

Your bridge can now react to a ship.

Now make it safer, clearer, or smarter.

You do not need to finish every upgrade.

Choose one upgrade first. If you finish early, try another challenge.

## Choose Your Upgrade @showdialog

# Choose your upgrade

Start with **A** if you are not sure.

Try **B** to make the bridge safer.

Try **C** or **D** only if you have extra time.

<img src="https://raw.githubusercontent.com/hisi741/raise-tower-bridge-tutorial/main/pics/example_upgrade_cards.png" height="220px">

## Start

Start from your Task 4 code.

Change one thing at a time.

## Upgrade A @showdialog

# Upgrade A: Tower Lights

When a ship is passing, turn the tower lights on.

When there is no ship, turn the tower lights off.

Use brightness **100** for on and **0** for off.

## Build A

Add light blocks.

Ship: lights on. No ship: lights off.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 100)
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 100)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
    } else {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 0)
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
    }
})
```

## Upgrade B @showdialog

# Upgrade B: Wait for the Ship

A safe bridge should not close too early.

Open the bridge, wait while the ship is passing, then close it.

The **while** block means: keep waiting while this is true.

## Build B

Try the wait upgrade.

The bridge waits, then closes.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        basculeMotors.raiseLowerBascule(BridgeSide.Left, BasculeDirection.Raise)
        basculeMotors.raiseLowerBascule(BridgeSide.Right, BasculeDirection.Raise)
        while (bridgeSensors.isShipPresent()) {
            basic.pause(100)
        }
        basculeMotors.raiseLowerBascule(BridgeSide.Left, BasculeDirection.Lower)
        basculeMotors.raiseLowerBascule(BridgeSide.Right, BasculeDirection.Lower)
    }
    basic.pause(100)
})
```

## Challenge C @showdialog

# Challenge C: Boat Colour

Only try this if you have extra time.

Use the colour sensor to change the tower lights.

Red boat: red lights. Other boats: blue lights.

## Build C

Try the colour challenge.

Red boat: red lights.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 100)
        if (bridgeSensors.checkColor(ColorSensorColor.Red)) {
            bridgeLighting.setTowerLightingColorHex(BridgeSide.Left, 0xff0000)
        } else {
            bridgeLighting.setTowerLightingColorHex(BridgeSide.Left, 0x0066ff)
        }
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
    } else {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
    }
})
```

## Challenge D @showdialog

# Challenge D: Ship Direction

Only try this if you have extra time.

Use the ship direction to change the tower lights.

Upriver: green. Downriver: orange.

## Build D

Try the direction challenge.

Upriver: green. Downriver: orange.

```blocks
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 100)
        if (bridgeSensors.checkShipSailingDirection(ShipSailingDirection.Upriver)) {
            bridgeLighting.setTowerLightingColorHex(BridgeSide.Right, 0x00ff00)
        } else {
            bridgeLighting.setTowerLightingColorHex(BridgeSide.Right, 0xff9900)
        }
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
    } else {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
    }
})
```

## Your Design @showdialog

# Your Best Bridge

Now choose your best idea.

You can combine upgrades.

Change one thing at a time and test after each change.

If something breaks, go back to the last version that worked.

## Test and Share

Build, test, and fix.

Show another team.

## Finish @showdialog

Great work, engineer!

[Task 1: Move the Bridge](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task1)

[Task 2: Stop the Bridge](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task2)

[Task 3: Choose the Height](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task3)

[Task 4: Automatic Bridge](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task4)


```template
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


```ghost
basic.forever(function () {
    if (bridgeSensors.isShipPresent()) {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 100)
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 100)
        bridgeLighting.setTowerLightingColorHex(BridgeSide.Left, 0xff0000)
        bridgeLighting.setTowerLightingColorHex(BridgeSide.Right, 0x00ff00)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 60)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 60)
        basculeMotors.raiseLowerBascule(BridgeSide.Left, BasculeDirection.Raise)
        basculeMotors.raiseLowerBascule(BridgeSide.Right, BasculeDirection.Raise)
        while (bridgeSensors.isShipPresent()) {
            basic.pause(100)
        }
        basculeMotors.raiseLowerBascule(BridgeSide.Left, BasculeDirection.Lower)
        basculeMotors.raiseLowerBascule(BridgeSide.Right, BasculeDirection.Lower)
    } else {
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Left, 0)
        bridgeLighting.setTowerLightingBrightness(BridgeSide.Right, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Left, 0)
        basculeMotors.moveBasculeTo(BridgeSide.Right, 0)
    }
    basic.pause(100)
})

if (bridgeSensors.checkColor(ColorSensorColor.Red)) {
    bridgeLighting.setTowerLightingColorHex(BridgeSide.Left, 0xff0000)
} else {
    bridgeLighting.setTowerLightingColorHex(BridgeSide.Left, 0x0066ff)
}

if (bridgeSensors.checkShipSailingDirection(ShipSailingDirection.Upriver)) {
    bridgeLighting.setTowerLightingColorHex(BridgeSide.Right, 0x00ff00)
} else {
    bridgeLighting.setTowerLightingColorHex(BridgeSide.Right, 0xff9900)
}
```