# Traffic Light Simulation

## {Project Description @unplugged}

Have you ever wondered how traffic lights work? In this project, you'll build your very own traffic light system using just three colored LEDs: red, yellow, and green! You'll learn how to set up a timer to automatically control the lights, just like at road intersections. You'll also add a button to control the lights manually, allowing you to decide when cars stop and go. This project will teach you about timing, automation, and the importance of traffic rules. Ready to become a traffic light engineer? Let's go!

## {Input-Process-Output (IPO) @unplugged}

![Traffic light output](https://i.postimg.cc/v860FsrR/traffic-light-manual-gif.gif)

The project has three main parts: input, processing, and output. Here's the breakdown:
- **Processing**: Microbit
- **Input**: Push button
- **Output**: LEDs

## Components Needed
- Microbit
- LEDs (Red, Yellow, Green)
- Breadboard
- Jumper wires
- Resistors

## Input Components
### Inbuilt Pushbutton on Microbit
The pushbutton acts as a switch that makes or breaks an electrical connection. When pressed, it completes the circuit and sends a signal to the Microbit.

## Output Components
### LEDs (Red, Yellow, Green)
LEDs will act as the traffic lights. Connecting the positive terminal of the LED to a Microbit pin will allow you to control it.

## Code to Turn On an LED
Connect the positive leg of an LED to the Microbit's P0 pin and the negative to GND. Use this code:
1. Go to `Advanced` > `Pins`.
2. Drag `digital write pin` block to `on start` or `forever` and set the pin to `P0` with a value of `1`.

To turn off the LED, set the value to `0`. Try making the LED blink continuously using a `pause` block.

```blocks
basic.forever(function () {
    pins.digitalWritePin(DigitalPin.P0, 1)
    pins.digitalWritePin(DigitalPin.P1, 0)
    pins.digitalWritePin(DigitalPin.P2, 0)
})
```
