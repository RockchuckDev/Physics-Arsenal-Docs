---
title: Extensions
---

# Public Functions

#### `float ToJumpVelocity(this float desiredHeight, float risingGravityMagnitude)`

Converts a desired jump height into the needed velocity to achieve that height based on a supplied gravity magnitude

| Parameter | Description |
|---|---|
| `desiredHeight` | The desired height to jump to |
| `risingGravityMagnitude` | The magnitude of the gravity force acting on the player while the player rises from their jump |

**Returns:** The velocity needed to achieve the desired height

#### `Vector3 FlattenVector(this Vector3 vector3)`

Flattens a vector by setting its Y component to 0

| Parameter | Description |
|---|---|
| `vector3` | The vector to flatten |

**Returns:** The flattened vector
