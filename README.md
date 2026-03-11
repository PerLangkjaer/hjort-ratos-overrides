# Hjort RatOS Overrides

This repository contains machine specific override configuration files used by Hjort Creations for RatOS (Klipper‑based) 3D printers. Each file holds only the parameters that deviate from the standard RatOS configuration for that machine. By centralizing these overrides, we can reuse, track and share our modifications while keeping the upstream config intact.

## Usage

To use an override file, include it at the end of your machine’s `printer.cfg` in RatOS. For example:

    [include rapunzel.cfg]

Alternatively, open the file and copy the relevant blocks into your own configuration.

We intentionally avoid replacing the standard RatOS config here; these files only append or override specific sections.

## Contents

- **rapunzel.cfg** – Overrides for the Rapunzel build with 1000 mm Z‑height and additional sensors.
- **printer.cfg** – Example file showing how to include `rapunzel.cfg` along with input shaper and chamber heater settings.

As you add new machines, name the file after the machine or build and include only the non‑standard parameters.

## Contributing

If you have a new Hjort Creations build you’d like to add:

1. Create a new `.cfg` file in the root with a descriptive name (e.g. `vcore500‑hjort.cfg`).
2. Include **only** settings that differ from the stock RatOS/V‑Core configuration.
3. Commit the file with a clear message describing the machine and changes.

Pull requests and issues are welcome!
