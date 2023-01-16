
# ChiTu : Intelligent Car

A MakeCode entensions for programming educational intelligent car.

## Basic usage

* Control the direction and speed of Chitu motor

```blocks
 chitu.motorRun(chitu.Motors.M1, chitu.Dir.CW, 150)
 chitu.motorRun(chitu.Motors.M2, chitu.Dir.CCW, 150)
```

* Stop the Chitu motor

```blocks
chitu.motorStop(chitu,Motors.M1)
```

* Set the Chitu servos

```blocks
chitu.servoRun(chitu.Servos.S1, 90)
chitu.servoRun(chitu.Servos.S2, 120)
```

* Read line tracking sensor

```blocks
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolLeft))
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolMiddle))
serial.writeNumber(chitu.readPatrol(chitu.Patrol.PatrolRight))
```

* Turn on/off the LEDs

```blocks
chitu.writeLED(chitu.LED.LEDLeft, chitu.LEDswitch.turnOn)
chitu.writeLED(chitu.LED.LEDRight, chitu.LEDswitch.turnOn)
```

## License

MIT

## Supported targets

* for PXT/microbit


## Footnotes

1.  More information about PPW intelligent electronic building blocks https://www.yuque.com/ppwdocs