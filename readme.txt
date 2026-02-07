# GPS Module Interfacing using NEO-7M (Serial Monitor)

## Overview
This project demonstrates real-time GPS data acquisition using the NEO-7M GPS module.
Raw NMEA sentences are received over UART and monitored using the Arduino IDE Serial Monitor.

## Hardware Used
- GPS NEO-7M Module
- GPS Antenna
- FTDI (USB–Serial Converter)
- Jumper Wires

## Working Principle
The GPS module continuously transmits NMEA sentences over UART.
These sentences are viewed directly on the Arduino IDE Serial Monitor without any
microcontroller-based processing.

## NMEA Sentences
- `$GPGGA` – Fix quality, number of satellites, HDOP, altitude
- `$GPRMC` – Time, latitude, longitude, data validity

## Output
The serial monitor displays live NMEA sentences from the GPS module.
Latitude and longitude values were extracted manually and verified using Google Maps.

## Result
The decoded GPS coordinates accurately matched the real-world location,
confirming correct GPS operation and satellite fix.

## Future Improvements
- Interface GPS with Arduino for automated parsing
- Use TinyGPS++ library for coordinate decoding
- Display data on LCD / OLED
- Transmit coordinates using GSM or LoRa
