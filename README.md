# Current & Voltage Reader Slice

Current and voltage reader slice for AC and DC supplies.

## Ratings

**r1: buses up to 60 V DC only.** The isolated side (GNDISO, tied to DC_BUS-
through NT2) floats at the bus voltage. Above 60 V, every primary-side item (GND,
+5V, the Nano, I2C) needs 5.3 mm creepage and clearance to the isolated side, the
ADuM5010's rating (datasheet Table 10). r1 does not have it: the ACS724 current
sensor is rated for 4.2 mm creepage, and its primary-side parts (R1, C5, C6, C7)
sit 1.639 mm from the isolated side's C11. The fix for higher buses is tracked
in [#2](https://github.com/feastorg/Slice_VCDC/issues/2).

## Introduction

[Short introduction on the project.]

## Usage

[Explain how to use the project. Include examples and screenshots if applicable.]

## Documentation

Please refer to the [docs](/docs) for more info.

---

<div align="center">
  <p>
    <img src="https://img.shields.io/badge/Developed_by-UWO--FAST--et--al-orange" alt="Developed by UWO-FAST et al.">
    <img src="https://img.shields.io/badge/Powered_by-Open_Source-blue" alt="Powered by Open Source">
  </p>
</div>
