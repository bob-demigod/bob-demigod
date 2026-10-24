# CYD ↔ Pico UART

Two Arduino sketches that prove a Cheap Yellow Display (ESP32) can talk to a Raspberry Pi Pico over UART.

## Problem

Before building a larger display project, the link itself had to be known-good: pins, baud, and a visible pass or fail on both USB serial monitors.

## What I built

- Sender sketch for the ESP32 Dev Module
- Receiver sketch for the Raspberry Pi Pico (Earle Philhower core)
- Wiring notes: ESP32 GPIO22 to Pico GP1, optional reverse on GPIO27 to GP0, common ground
- Link at 9600 8N1, USB monitors at 115200

## Stack

Arduino CLI, ESP32 core, RP2040 core.

## Status

Personal hardware bring-up. Sketches stay in the private repo. This page is the public description.
