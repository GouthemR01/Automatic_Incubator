# Automatic_Incubator
This is a design  for an Automatic Incubator based on Pic16f877a. This differs from my previously done Incubator project as this board has a MCU in it making the design standalone and combat.

## Features

- **Microcontroller:** PIC16F877A for core processing and control.
- **Real-Time Clock:** DS1307 keeps accurate time to manage incubation schedules.
- **Egg Rotation:** Stepper motor automatically rotates eggs at constant time intervals.
- **Temperature Control:** 
  - **NTC Analog Temperature Sensor:** Monitors and regulates temperature.
  - **Relay:** Controls the heating element based on temperature readings.
- **Humidity Monitoring:** DHT11 sensor monitors and displays humidity levels.
- **LCD Display:** Shows current temperature and humidity for easy monitoring.

## Components

- **PIC16F877A:** Central microcontroller.
- **DS1307 RTC:** Real-time clock for timekeeping.
- **NTC Thermistor:** Analog temperature sensor.
- **Relay:** Controls the heating element.
- **DHT11:** Humidity sensor.
- **Stepper Motor:** Rotates eggs at set intervals.
- **LCD Display:** Shows temperature and humidity readings.

## Functionality

1. **Time Management:** The DS1307 RTC keeps track of the incubation time and ensures that eggs are rotated at precise intervals.
2. **Temperature Control:** The NTC thermistor continuously monitors the temperature. The PIC16F877A processes this data and controls the relay to maintain the desired temperature.
3. **Humidity Monitoring:** The DHT11 sensor checks humidity levels, and the data is displayed on the LCD.
4. **Egg Rotation:** The stepper motor rotates the eggs automatically at set intervals to ensure even incubation.

## How It Works

1. **Initialization:** The system initializes the microcontroller, sensors, and display.
2. **Timekeeping:** The DS1307 RTC module provides the current time to manage egg rotation schedules.
3. **Temperature Regulation:** The NTC thermistor sends temperature readings to the PIC16F877A, which controls the relay to maintain the set temperature.
4. **Humidity Monitoring:** The DHT11 sensor continuously checks humidity levels and sends the data to be displayed on the LCD.
5. **Egg Rotation:** The stepper motor is activated at regular intervals to rotate the eggs, ensuring even heating.

