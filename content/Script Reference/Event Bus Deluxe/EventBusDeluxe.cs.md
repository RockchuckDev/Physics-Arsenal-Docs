---
title: EventBusDeluxe
---

# class EventBusDeluxe

A custom event bus that works just like signals in Godot, but is completely decoupled and is not affected by refactoring function names. Custom event types can be defined anywhere, but they must be a struct and are conventionally defined in [[EventTypes.cs]] and end with "Event"

## Public Functions

### `void Subscribe<TEvent>(Action<TEvent> action)`

Subscribes an action to the event bus for a given event type

### `void Unsubscribe<TEvent>(Action<TEvent> action)`

Unsubscribes an action from the event bus for a given event type

### `void Fire<TEvent>(TEvent eventData)`

Fires an event of a given type, invoking all subscribed actions with the provided event data
