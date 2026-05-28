# Trace Concept

Trace is a local-first smart scale concept for tagged containers and other physical items.

The first use case is meal prep and food storage: identify a container, subtract its empty weight, and keep a practical record of what remains.

## Why Identity Matters

A normal scale can tell you weight, but it does not know what it is weighing. Trace adds identity so the scale can connect a reading to a specific container and its history.

That identity makes repeated weigh-ins more useful. The device can recognize the container, use the right empty weight, and show the latest known context without requiring the user to search for it manually.

## Why Empty Weight Matters

Containers vary. If the empty weight is not known, the total weight is only partly useful.

Trace stores the empty container weight once, then subtracts it from later readings. That makes the remaining contents easier to estimate without re-entering the same tare value every time.

## Why NFC Is Useful

NFC tags are inexpensive, small, and easy to attach to containers. A tag can give the scale a stable identifier without relying on visual recognition or manual selection.

The early direction is to support assigning or writing a tag during registration, then reading that tag during later weigh-ins.

## Why Local-First Matters

Trace should not require a cloud account or a dedicated mobile app to do the basic job.

The device should host or serve a local interface for registration, readings, and history. Normal home WiFi should be supported, and a fallback direct-device access point or captive portal mode may be useful when WiFi setup is not available.

## Why Food Is First

Meal prep is a focused use case with repeated containers, clear empty weights, and useful questions:

- what container is this?
- what did it hold?
- how much is left?
- when was it prepped?
- how many servings remain?

## Later Expansion

The same pattern may apply to supplies, bins, hardware, consumables, and other physical inventory.

That should not make the first version too broad. The first version should prove the identity, empty-weight, weighing, and local-interface loop before expanding into broader inventory workflows.
