---
title: ShootOnInteract
---

# class ShootOnInteract

## Exported Variables

| Name | Type | Description |
|---|---|---|
| `rootObjectNode` | `Node` | The root object node of this grabbable object |
| `bulletSpeed` | `float` | How fast the bullet travels. Only used in calculating how much force is applied to objects that are shot |
| `bulletMass` | `float` | The mass of the bullet. Only used in calculating how much force is applied to objects that are shot |
| `range` | `float` | The range of the gun |
| `bulletImpactParticles` | `PackedScene` | The GpuParticles3D node that is spawned when an object (static or dynamic) is shot |
| `showCrosshair` | `bool` | Whether or not to show a crosshair on the screen for this gun |
| `crosshairScene` | `PackedScene` | The scene of the crosshair that is shown on the screen for this gun (provided showCrosshair is true) |

## Public Functions

### `void SetScreenSightVisibility(bool isVisible)`

Subscribed to the IsGrabbedTracker "IsGrabbedTrackerUpdated" signal. If the provided bool is true (and showCrosshair is true), the crosshair for this gun is shown on screen, if false, the crosshair is hidden

### `void SubscribeOrUnsubscribeToPlayerRequestInteractOnIsGrabbedTrackerUpdate(bool grabState)`

When the IsGrabbedTrackerUpdated signal fires, if the provided bool is true, subscribe OnPlayerRequestInteract to the custom [[Event Bus Deluxe/EventTypes.cs#struct PlayerRequestedToInteractWithGrabbedObjectEvent | PlayerRequestedToInteractWithGrabbedObjectEvent]] event bus, and unsubscribe if it is false.

### `void OnPlayerRequestInteract(PlayerRequestedToInteractWithGrabbedObjectEvent eventData)`

Apply force to the object that gets shot, and tell [[Managers/ParticleManager.cs#class ParticleManager | ParticleManager]] to spawn the provided impact particles
