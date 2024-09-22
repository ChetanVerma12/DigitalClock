# Digital Clock

This is a simple **Digital Clock** Java application that displays the current time and date in a graphical window using `JFrame` and `JLabel`. The time is updated every second, and the display format is customizable.

## Features

- **Current Time**: Displays the current time in hours, minutes, seconds, and AM/PM format.
- **Current Date**: Displays the current date in `dd:MM:yyyy` format.
- **Real-Time Update**: The time is updated every second to display the current time accurately.
- **Customizable Fonts and Colors**: The time and date labels use bold fonts and customizable colors.

## Screenshot

*(You can add a screenshot here if you'd like)*

## Code Overview

The code consists of a class `DigitalClock` that extends `JFrame`. The class contains two `JLabel` components for showing the time and date. The time and date are formatted using `SimpleDateFormat` and updated every second using a `while` loop with `Thread.sleep(1000)`.

### Components

- `JLabel l1`: Displays the current time.
- `JLabel l2`: Displays the current date.
- `SimpleDateFormat d1`: Formats the time as `hh:mm:ss a`.
- `SimpleDateFormat d2`: Formats the date as `dd:MM:yyyy`.

### Main Functionality

1. **GUI Setup**: 
   - The time and date are displayed using `JLabel` components.
   - Fonts, colors, and layout are customized.
   
2. **Time and Date Update**: 
   - The time and date are updated every second inside an infinite loop.
   - `Thread.sleep(1000)` is used to pause the update for 1 second.

### Example Usage

```java
public static void main(String[] args) {
    DigitalClock d1 = new DigitalClock();
    d1.setVisible(true);
    d1.setSize(500, 500);
    d1.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    d1.setComponents();
}
