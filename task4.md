# Raise Tower Bridge

```package
raise-tower-bridge=github:hisi741/pxt-raise-tower-bridge
```

### @hideDone true

## Free Build @showdialog

# Free Build: Design Your Own Bridge Program

You are now in control of Tower Bridge.

Design your own bridge program.

There is no single correct answer.

## Your challenge

Create a program that controls the bridge safely and clearly.

Think about how people can understand what your program is doing.

## Useful blocks

You can use any of the Tower Bridge blocks.

You can also use other blocks to control when and how the bridge moves.

```ghost
input.onButtonPressed(Button.A, function () {})
input.onButtonPressed(Button.B, function () {})
input.onButtonPressed(Button.AB, function () {})
input.onGesture(Gesture.Shake, function () {})
input.lightLevel()
input.temperature()
input.soundLevel()

basic.forever(function () {})
basic.pause(100)
basic.showIcon(IconNames.Yes)
basic.showIcon(IconNames.No)
basic.showNumber(0)
basic.showString("OPEN")
basic.clearScreen()

if (true) {} else {}
true
false
0 == 0
0 < 1
0 > 1
true && false
true || false
!true

for (let index = 0; index < 4; index++) {}
while (false) {}
for (let value of [0, 1, 2]) {}

let angle = 0
angle = 45
angle += 1
Math.randomRange(0, 86)

music.playTone(262, music.beat(BeatFraction.Whole))
music.rest(music.beat(BeatFraction.Whole))

towerBridge.raiseLeftBascule()
towerBridge.raiseRightBascule()
towerBridge.lowerLeftBascule()
towerBridge.lowerRightBascule()
towerBridge.setLeftBasculeTo(45)
towerBridge.setRightBasculeTo(45)
towerBridge.shipComing()
```

```template
basic.forever(function () {
    
})
```

## Improve your bridge

Once your first idea works, improve it.

Can you make it safer? clearer? more realistic? more creative?

## Finish @showdialog

Great work, engineer!

[Back to Task 3](https://makecode.microbit.org/#tutorial:https://github.com/hisi741/raise-tower-bridge-tutorial/task3)

