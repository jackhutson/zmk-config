# ADR 0001: Prospector Dongle as Split Central for Charybdis Nano

Date: 2026-02-04
Status: Accepted

## Context
- We want a low-power split setup where a Prospector dongle is the central device.
- The Charybdis Nano halves should behave as peripherals that pair to the dongle.
- The Prospector screen should show layer information for easier at-a-glance feedback.
- The assembled Prospector does not include the proximity/ambient light sensor.

## Decision
- Add the Prospector ZMK module and build a new dongle shield configuration.
- Configure the Prospector dongle as the split central and both keyboard halves as peripherals.
- Provide layer `display-name` values so the Prospector roller can show layer names.
- Disable the ambient light sensor and set a fixed brightness value.

## Consequences
- The dongle becomes the only central device and must be flashed/powered for the keyboard to function.
- The keyboard halves will no longer act as centrals unless overridden at build time.
- Layer names are now visible on the Prospector screen when the dongle is active.
- Brightness is fixed unless reconfigured in the dongle config.

## Alternatives Considered
- Keep the left half as central and use the dongle only for display.
  - Rejected because it does not reduce battery usage on the halves and still requires a central keyboard half.
- Add a proximity sensor to auto-adjust brightness.
  - Rejected because the current hardware lacks the sensor.

## References
- Prospector ZMK module documentation (screen, roller, and ambient light settings).
- ZMK dongle configuration guidance (split central vs peripherals).
