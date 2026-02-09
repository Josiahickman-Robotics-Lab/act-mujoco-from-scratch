Credits A la : https://github.com/StuckAtPrototype/DefineDoneFramework

ACT Pick-and-Place (V1)

One-Sentence-Goal:
A MuJoCo simulation where a Franka Panda robot autonomously picks and places a cube using the ACT policy

Start Date: February 8, 2026
End Date: February 29, 2026 (21 Days)


Done Criteria:

-Environment Setup:	The Franka Panda model loads in MuJoCo with a table and a 5cm red cube. 

-Teleop & Data: I can manually move the gripper to the cube using a script and save 50 successful pick-and-place trials into a single .hdf5 file.

-Model Architecture:	The ACT code (CVAE + Transformer) successfully ingests the .hdf5 data and completes a 500-epoch training run without errors.

-Loss Convergence: The training logs show the L1 reconstruction loss consistently dropping and stabilizing below a threshold of 0.05.

-Autonomous Success: When the "Evaluation" script is run, the robot successfully completes the pick-and-place task in 7 out of 10 consecutive trials.



Version 2 Ideas:
Do not work on these until Version 1 is marked "Done."

-Integrating ResNet-18 for visual-only inputs (using pixels instead of raw x,y,z).

-Temporal Ensembling (exponential moving average of action chunks).