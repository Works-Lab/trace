# Proposed Architecture

This is a proposed architecture, not a finalized BOM.

Trace will likely need these system pieces:

- microcontroller
- load cell
- load-cell amplifier
- NFC reader/writer
- local web UI
- home WiFi mode
- fallback access point or captive portal mode
- local storage
- optional future sync/export

## Device Layer

The device layer reads weight, handles calibration, reads or writes NFC tags, stores local records, and serves the interface.

The exact controller, amplifier, reader, enclosure layout, and storage approach are still TBD. Do not lock documentation to a specific part until the repo contains supporting hardware notes.

## Local Interface

The local web UI should support container registration, tag assignment, live readings, current contents, prep dates, servings, and history.

The first usable interface can be simple. It should make the core loop clear before adding broader inventory features.

## Network Modes

Home WiFi is the normal target mode.

A fallback direct-device access point or captive portal mode may help with setup, offline use, and recovery. This mode is part of the initial direction, not a confirmed implementation yet.

## Storage and Export

Trace should store core data locally. Future sync or export could be useful, but the baseline should work without a required account or external service.
