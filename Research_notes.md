1/30/2026
-Working on getting mujoco environment to run, started playing around with models it was hella fun lmfao, it's like a video game

2/4/2026
-I need to add cameras to the normal Panda model (which has none) to replicate the visual sensing aspect of the ACT paper. The paper adds a wrist camera, a top camera and a front camera. All Logitech C922x webcams, which have a FOV of 78 degrees.

-Simpler to add then expected, mujoco is pretty cool. Camera on wrist done!

2/5/2026
-Successfully placed all cameras in mujoco xml file. Corrected orientations and positions.

Next Step collect teleoperation data.
Now since I don't have a real robot, all I can do is command the robot in sim, and collect data from that.
