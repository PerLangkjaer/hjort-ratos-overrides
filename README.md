# Hjort RatOS Overrides

This repository contains machine-specific override configuration files used by **Hjort Creations** for RatOS/Klipper 3D printers. Each file only holds the parameters that deviate from the standard RatOS configuration for that machine. By centralizing these overrides, we can reuse, track and share our modifications while keeping the upstream config intact.

## Usage

To use an override, include it at the end of your machine’s `printer.cfg` in RatOS/Klipper. For example:

    [include rapunzel_printer.cfg]

The `_printer.cfg` files bundle the machine-specific configuration together with common input-shaper and chamber heater settings. If you only need the machine-specific parameters (without input-shaper and heater overrides), you can include the `.cfg` file directly instead, e.g.:

    [include rapunzel.cfg]

Alternatively, open the file and copy the relevant blocks into your own configuration. We intentionally avoid replacing the standard RatOS config here; these files only append or override specific sections.

## Contents

- **rapunzel.cfg** – Machine-specific overrides for the Rapunzel build with 1000 mm Z-height and additional sensors.
- **rapunzel_printer.cfg** – Example _printer_ file that includes `rapunzel.cfg` and defines input shaper and chamber heater PID settings.
- **hjort.cfg** – Machine-specific overrides for a standard V-Core 4 build with a chamber heater for faster heat soak.
- **vcore4_printer.cfg** – Example _printer_ file that includes `hjort.cfg` and defines the same input shaper and chamber heater PID settings.
- **yggdrasill.cfg** – Machine-specific overrides for the Yggdrasill build (chamber heater macros, sensors, etc.).
- **yggdrasill.md** – Wiring guide for the Octopus Max EZ board used by the Rapunzel/Yggdrasill build.

As you add new machines, create a new `.cfg` file for the machine or build and include only the non-standard parameters. Optionally create a `_printer.cfg` file to bundle the machine overrides with common input-shaper and chamber heater settings.
