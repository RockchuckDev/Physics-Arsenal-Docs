---
title: PlayerController
---

# Exported Variables

| Name | Type | Description |
|---|---|---|
| `groundedAccel` | `float` | The rate at which the player accelerates (speeds up) when they are on the ground |
| `groundedDeceleration` | `float` | The rate at which the player decelerates (slows down) when they are on the ground |
| `maxSpeed` | `float` | The maximum speed the player can travel at on the XZ plane |
| `jumpHeight` | `float` | The height of the peak of the player's jump, in world space units |
| `camera` | `Camera3D` | The player's first person camera |
| `cameraSensitivity` | `float` | The sensitivity of the player's camera, controlling how fast the camera rotates when the mouse moves |
| `sensitivityDivisor` | `float` |  |
| `baseGravityMagnitude` | `float` | The acceleration due to gravity, in world space units per second squared (bigger = fall faster) |
| `gravityScaleWhenFalling` | `float` | The scale factor of gravity when the player falls, best to be set above one, as it makes the player's jump feel less floaty |
| `cutFactorWhenJumpReleasedEarly` | `float` | The amount of the player's velocity (0 - 1) that is removed when the jump button is released early |
