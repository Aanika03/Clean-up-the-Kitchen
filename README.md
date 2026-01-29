# Clean-up-the-Kitchen
Objective: Restore the kitchen to a clean, organized, and safe state. Navigate to the kitchen, identify objects and surfaces, dispose of trash, place dishes and utensils in the sink, organize items on counters or shelves, wipe surfaces, clean the floor, verify cleanliness, then stop.
# Fetch Kitchen Clean-up AI Model

## Overview
This repository contains a Fetch mobile manipulator control model and task
definition designed for kitchen clean-up in ManiSkill / MS-HAB simulation
environments.

The model follows the official **AI Fetch Interface Specification** and is
compatible with `pd_joint_delta_pos` control mode.

## Robot
- Fetch Mobile Manipulator

## Task
- Clean-up the kitchen
- Trash removal
- Dish collection
- Object organization
- Surface and floor cleaning

## Observation Mode
- state (flattened or dictionary)

## Input
- Shape: (state_dim,) or (batch_size, state_dim)
- Data type: float32

## Output
- Shape: (13,)
- Range: [-1.0, 1.0]
- Control:
  - 7 arm joints
  - 1 gripper
  - 3 body joints
  - 2 base velocity controls

## Control Mode
- pd_joint_delta_pos (required)

## Framework
- PyTorch

## Status
Submitted for AI Miner onboarding and Fetch robot evaluation.

## Author
GitHub: https://github.com/Aanika03
