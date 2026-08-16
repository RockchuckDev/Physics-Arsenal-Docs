---
title: EventTypes
---

# struct PlayerRequestedToInteractWithGrabbedObjectEvent

Fires when the player presses the interact button for a given hand. Only the objects that are actively being held and have a child node that defines interaction behavior are subscribed to this event

## Public Variables

| Name | Type | Description |
|---|---|---|
| `requestedHandDataToInteractWithGrabbedObject` | `GrabData` | The GrabData of the hand that is requesting to interact with the grabbed object |

# struct PlayerSuccessfullyInteractedWithGrabbedObjectEvent

Fires when the player successfully interacts with a grabbed object.

## Public Variables

| Name | Type | Description |
|---|---|---|
| `handDataWhichWasHoldingObjectThatWasInteractedWith` | `GrabData` | The GrabData for the hand that was holding the object that was interacted with. |

# struct SpawnBulletImpactParticlesEvent

## Public Variables

| Name | Type | Description |
|---|---|---|
| `impactPoint` | `Vector3` | Position in world space to spawn the particles at |
| `impactNormal` | `Vector3` | Essentially the "ricochet" direction of the impact point. |
| `bulletImpactParticlesScene` | `PackedScene` | The particles to spawn in |

# struct PlayerChangedGrabModeEvent

Fires when the player changes their grab mode.

## Public Variables

| Name | Type | Description |
|---|---|---|
| `isToggleGrabModeOn` | `bool` | Boolean to represent if the active grab mode is "toggle" (true) or is "hold" (false) |
