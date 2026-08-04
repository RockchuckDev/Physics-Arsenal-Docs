
# v0.1.2-alpha
- Renamed project from "Physkit" to "Physics Arsenal"
- Added a simple color palette to the Materials folder. 
- PlayerController.cs now manually handles gravity to have a less 'floaty' character controller. 
- jumpForce in PlayerController.cs replaced with jumpHeight. 
- Added a function to Extensions.cs that converts a float into the vertical velocity needed to apply to an object to get that object to rise to the provided value
- Fixed a bug that would cause objects with rotation_override to chase a seemingly random rotation.
- Added MIT License file

# v0.1.1-alpha
- Added missing dependencies in World.tscn. 
- Removed the need for grabbable metadata to be a boolean set to true. Now Physics Arsenal simply looks for any metadata tag named "grabbable"
	- This means the type of the "grabbable" tag no longer matters
- Fixed a bug regarding the way torque was applied to grabbed objects that would cause objects to have an incorrect rotation when held. 
- Updated README to reflect these changes.

# v0.1.0-alpha
- First versioned release of Physics Arsenal
- PlayerInteraction.cs reworked so that grab functionality only needs to be defined once
	- All data regarding the left and right hands are stored inside GrabData classes
- Added "[[rotation_override]]" metadata tag support.
	- This gives the ability to define the rotation objects will have relative to the camera when grabbed
- Added "[[Grab Point]]" support
	- This gives the ability to define a location on an object where the player will always grab when grabbing the object. Such as a handle
- Added ability to switch between hold and toggle grab modes. 
- Added a UI label that displays which grab mode you are in. 
- Added the scene I test everything in to the asset.

# Pre v0.1.0-alpha
- Objects can be picked up and moved around in a physics based way
- Physics based, first-person character controller
- Objects can be grabbed with left and right hands independently
- Updated README to mention that this project was programmed in C#