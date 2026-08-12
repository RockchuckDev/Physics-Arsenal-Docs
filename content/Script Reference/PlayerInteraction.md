---
title: PlayerInteraction
---

# Exported Variables

| Name | Type | Description |
|---|---|---|
| `grabPivotScene` | `PackedScene` | The scene that is instantiated and grabs the object. Essentially your "hand" |
| `maxInteractDistance` | `float` | The maximum distance away from the camera that the player can interact with objects |
| `dropDistanceBuffer` | `float` | Added to maxInteractDistance to determine how far away a grabbed object needs to be from the player to be grabbed. Adding a small buffer instead of just dropping the object when it's distance from the player exceeds maxInteractDistance gives the player a little wiggle room when grabbing something at the very edge of their interact distance |
| `grabStrength` | `float` | The strength of the force applied to grabbed objects to move them |
| `grabDampening` | `float` | Prevents jitter when moving grabbed objects, but if turned up too high can make it harder to move objects |
| `grabRotationStrength` | `float` | The strength of the force applied to grabbed objects to rotate them |
| `grabRotationDampening` | `float` | Prevents jitter when rotating grabbed objects, but if turned up too high can make it harder to rotate objects |
| `grabDistanceAdjustmentIncrement` | `float` | The amount to increment/decrement the distance the grabbed object is from the player |
| `grabCenterOffset` | `float` | How far off to the left/right grabbed objects are when grabbed by the corresponding hands. Done so that when the player grabs two objects, they don't fight for the same space directly in front of the player |

%%last-updated-start%%
---
*Last updated: 08-11-2026 22:00*
%%last-updated-end%%
