![[shoot on interact demonstration.gif]]
[[ShootOnInteract.cs]] is a script that attaches to a Raycast3D node. With it, the object (most likely a gun) you are holding can shoot static objects, and dynamic objects (and even move them around).

# Requirements
- [[Is Grabbed Tracker]] node
- A Raycast3D that [[ShootOnInteract.cs]] can attach to
![[requirements.png]]

Shoot On Interact pairs very well with [[look_at_target]], but has extra requirements if you chose to do so:
- The X component of the local position of the RayCast must be 0
	- ![[0 x component.png]]
- Only the Z component of the RayCast target position may be modified, and it must be negative
	- ![[target position with only z modified.png]]
Both of these requirements stem from the math that enables [[look_at_target]] to work.

See [[ShootOnInteract.cs#Exported Variables]] for inspector variable reference
%%last-updated-start%%
---
*Last updated: 08-15-2026 21:45*
%%last-updated-end%%
