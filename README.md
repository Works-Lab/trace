# Trace

Trace is an early prototype concept for an NFC-enabled smart scale that tracks containers, empty weights, and remaining contents.

The first version is focused on meal prep. In the intended flow, a container gets a cheap NFC tag, the scale saves its empty weight, and future weigh-ins update what is left.

## Concept

1. Register a container.
2. Save its empty weight.
3. Write or assign an NFC tag.
4. Fill the container.
5. Weigh it later.
6. Track remaining contents through a local interface.

## Goals

- local-first
- NFC read/write
- no required cloud account
- no dedicated mobile app
- container empty-weight registry
- live remaining weight
- prep-date and serving logic
- home WiFi support
- fallback direct-device access mode if possible

## First Use Case

Meal prep and food storage.

Trace should help answer simple questions:

- What container is this?
- What did it hold?
- What is the empty weight?
- How much is left?
- When was it prepped?
- How many servings remain?

## Status

Early prototype / active development.

The repo will start with documentation and design notes, then expand as hardware, firmware, and interface files are cleaned up for public release.
