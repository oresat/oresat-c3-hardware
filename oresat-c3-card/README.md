# OreSat C3 Card v7.0

- See also README-fabrication.md and README-assembly.md

## Overview

This card is the main on-board computer (OBC) and housekeeping unit (HKU) and Command and Date Handler (CDH) for OreSat
CubeSats. It:

- Connects to the backplane with a main connector and two RF ports
- Has an L band radio receiver based on the AT86RF215.
- Has a UHF radio transceiver based on the AT86RF215
- Has a radiation tolerant watchdog timer (with a cheap commercial replacement if you're not going to orbit)
- Controls the OreSat Power Domain (OPD), which turns on and off and controls other cards
- Talks to both CAN OreSat CAN busses

For more information: TODO: Link to Google Doc.

