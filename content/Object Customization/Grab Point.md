![[Grab Point demonstration.gif]]

Typically, when the player grabs an object, the object is grabbed at a point on the object where the player was looking. However, for some objects, such as those with handles, you want the player to always grab the object in the same spot. This is achievable using Grab Points. 
# Usage
Simply add any 3D node to your object's root RigidBody node, and name it "Grab Point" (case sensitive). 
<br>
![[grab-point-node-in-tree.png]]
<br>
Now, whenever the player grabs your object, their hand will teleport to the position of the Grab Point node, and grab the object from there.
<br>
Note: The Grab Point node does not need to be physically touching the RigidBody node in any way for this to work. The player will still be able to pick up and move the object around.
![[grab-point-not-touching-the-rest-of-the-object.gif]]

%%last-updated-start%%
---
*Last updated: 08-02-2026 14:21*
%%last-updated-end%%
