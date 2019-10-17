# oresat-c3
## General information
This is the C3 (Command, Communication, and Control) card for OreSat. It
acts as the central control point for the entire OreSat project. It
provides a communication link to the ground via dual AX5043 radios,
providing a telecommand and telemetry interface.

Further documentation can be found in the [doc](doc) folder.

## Software
The software for the C3 card is integrated into the
[oresat-firmware](https://github.com/oresat/oresat-firmware) repository.
This is because the OreSat project is a tightly integrated system with
several common libraries and multiple subsystems working concurrently.

## License
OreSat C3 is licensed under the CERN OHL v1.2. A copy of the license is
located in [here](LICENSE.md)
