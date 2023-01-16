
# ChiTu : Intelligent Car

A MakeCode extensions for programming educational intelligent car.

## Wiring Diagram
Diagram will be displayed soon.

## Motor
Control the Chitu to Forward, backward, turn left and turn right.

* Control the car forward

```blocks
 chitu.motorRun(chitu.Motors.M1, chitu.Dir.CW, 120)
 chitu.motorRun(chitu.Motors.M2, chitu.Dir.CW, 120)
```

* Control the car backward

```blocks
 chitu.motorRun(chitu.Motors.M1, chitu.Dir.CCW, 120)
 chitu.motorRun(chitu.Motors.M2, chitu.Dir.CCW, 120)
```

* Control the car to turn left

```blocks
 chitu.motorRun(chitu.Motors.M1, chitu.Dir.CCW, 80)
 chitu.motorRun(chitu.Motors.M2, chitu.Dir.CW, 120)
```

* Control the car to turn right

```blocks
 chitu.motorRun(chitu.Motors.M1, chitu.Dir.CW, 120)
 chitu.motorRun(chitu.Motors.M2, chitu.Dir.CCW, 80)
```

* Stop the Chitu left motor

```blocks
chitu.motorStop(chitu,Motors.M1)
```

* Stop the Chitu right motor

```blocks
chitu.motorStop(chitu,Motors.M2)
```

* Stop the Chitu left and right motor

```blocks
chitu.motorStop(chitu,Motors.All)
```

## servo

* Set the Chitu servo1 to 90°

```blocks
chitu.servoRun(chitu.Servos.S1, 90)
```

* Set the Chitu servo2 to 120°

```blocks
chitu.servoRun(chitu.Servos.S2, 120)
```


## Read line tracking sensor

* Read the left line tracking sensor

```blocks
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolLeft))
```

* Read the middle line tracking sensor

```blocks
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolMiddle))
```

* Read the right line tracking sensor

```blocks
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolRight))
```

## Line tracking sensor event

* On left line tracking sensor is high

```blocks
chitu.ltEvent(chitu.Patrol1.PatrolRight, chitu.Voltage.High, function () {
    serial.writeNumber(1)
})
```

* On left line tracking sensor is low

```blocks
chitu.ltEvent(chitu.Patrol1.PatrolRight, chitu.Voltage.Low, function () {
    serial.writeNumber(0)
})
```

## LED Lights

* Turn on the left LED light

```blocks
chitu.writeLED(chitu.LED.LEDLeft, chitu.LEDswitch.turnOn)
```

* Turn off the left LED light

```blocks
chitu.writeLED(chitu.LED.LEDLeft, chitu.LEDswitch.turnOff)
```

* Turn on the right LED light

```blocks
chitu.writeLED(chitu.LED.LEDRight, chitu.LEDswitch.turnOn)
```

* Turn off the right LED light

```blocks
chitu.writeLED(chitu.LED.LEDRight, chitu.LEDswitch.turnOff)
```

## License

MIT

## Supported targets

* for PXT/microbit


## Footnotes

1.  More information about PPW intelligent electronic building blocks https://www.yuque.com/ppwdocs