# Repo for BT in DT

## This repository contains several controllers, which are designed to run on a duckiebot with the daffy configuration.

### 1 PID-Controller
A simple PID controller, uses a weighted sum of distance to center and heading angle as error term. Reference for both are zero (driving at the center of the lane, heading parallel to the lane)

### 2 Cascade-PID-Controller
For the outer loop, use distance to lanecenter to compute reference angle and use this, to compute output from the heading angle and the reference angle. The innerloop uses a linear extrapolation to approximate the current angle, as the inner loop has a higher frequency, then the lane-filter-node, which provides the position values.

### 3 PurePursuit

### 4 PolePlacement
