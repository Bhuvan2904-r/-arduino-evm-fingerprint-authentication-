# Arduino-Based EVM Voting Machine with Fingerprint Authentication

## Project Overview

This project presents an Arduino-based Electronic Voting Machine (EVM)
integrated with fingerprint authentication for voter verification.

The system uses a biometric fingerprint sensor to authenticate registered
voters before allowing them to cast a vote. After successful authentication,
the voter can select a candidate using push buttons. The selected vote is
recorded and the voting status is displayed on an LCD.

The project demonstrates the integration of biometric authentication with
an embedded voting system to improve voter verification and prevent
duplicate voting.

## Objectives

- Implement fingerprint-based voter authentication.
- Allow voting only for registered voters.
- Prevent duplicate voting.
- Provide real-time status information through an LCD.
- Record votes electronically.
- Demonstrate hardware-software integration using Arduino.

## Hardware Components

- Arduino Uno
- R307 Fingerprint Sensor
- 16x2 LCD Display
- Push Buttons
- Buzzer
- Regulated Power Supply (RPS)
- EEPROM / Non-volatile Memory
- Connecting Wires

## Software Requirements

- Arduino IDE
- Embedded C / Arduino C++
- Fingerprint Sensor Library
- LCD Library

## Technologies Used

- Arduino Uno
- Embedded Systems
- Fingerprint Authentication
- Biometric Security
- LCD Interfacing
- EEPROM
- Embedded C

## Working Principle

1. The system is powered using a regulated power supply.
2. The Arduino initializes the fingerprint sensor, LCD and other modules.
3. The voter places a finger on the fingerprint sensor.
4. The captured fingerprint is compared with the registered fingerprint data.
5. If the fingerprint is verified, the voter is allowed to proceed.
6. The voter selects a candidate using the corresponding push button.
7. The selected vote is recorded in memory.
8. The LCD displays the voting status.
9. The system prevents a voter who has already voted from voting again.

## System Architecture

The Arduino Uno acts as the main controller of the system.

Main functional blocks:

Fingerprint Sensor
        |
        v
   Arduino Uno
    /   |   \
   /    |    \
 LCD  Buttons  Memory
              |
            Votes

## Fingerprint Authentication

Fingerprint data is enrolled and stored in the fingerprint module.
During the voting process, the fingerprint of the voter is scanned and
compared with the registered fingerprint data.

Only an authenticated voter is allowed to continue to the voting process.

## Voting Process

After successful authentication:

- Candidate options are displayed to the voter.
- The voter selects a candidate using a push button.
- The vote is recorded.
- The LCD displays the confirmation message.
- The system prevents duplicate voting.

## Testing

The prototype was tested for:

- Registered fingerprint verification
- Unregistered fingerprint rejection
- Candidate selection
- Vote recording
- Duplicate-voting prevention
- LCD status display
- System operation

## Applications

- College elections
- University elections
- Institutional voting
- Club and committee elections
- Small-scale voting systems
- Embedded systems demonstrations

## Future Scope

Possible future improvements include:

- IoT-based remote monitoring
- GSM-based result transmission
- Cloud-based vote storage
- Mobile application integration
- Enhanced biometric authentication
- Larger voter database support


