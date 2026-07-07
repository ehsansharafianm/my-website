---
title: Trajectory Optimization for Spot-Welding Robots
summary: Time- and energy-optimal trajectory planning for 6-DOF spot-welding robots on an automotive body-production line — my M.Sc. thesis, in collaboration with an automobile manufacturing company.
date: 2020-02-01
tags:
  - Robotics
  - Trajectory Optimization
  - Spot Welding
  - Automotive
  - Optimization
links:
  - type: pdf
    name: Journal Article
    url: /publications/spot-welding-trajectory-2023/
image:
  caption: 'Spot-welding robots on an automotive body-production line'
  focal_point: Center
---

For my M.Sc. thesis, I collaborated with an automobile manufacturing company to optimize the motion of the robots that perform spot welding on the vehicle-body production line.

<!--more-->

## The Problem

On a car-body assembly line, many serial robots perform hundreds of spot welds. Their trajectories were programmed manually by operators — reliable, but far from optimal in speed and energy use.


## What I Did

I formulated the robot's motion as an optimization problem and solved it two ways:

- **Minimum-time trajectory** — a single-objective problem minimizing the welding gun's travel time.
- **Time–energy trajectory** — a multi-objective problem minimizing both travel time and energy consumption.

The planning considered the **position and orientation of the welding gun simultaneously**, in both joint and Cartesian spaces, while respecting the robot's joint limits and the required gun orientation at each weld point. I used **genetic algorithm** and **particle swarm optimization** to search for the best trajectories.


## Results

Applied to a real robot on the production line, the optimized trajectories reduced the spot-welding operation's travel time by:

- **up to 24%** for the minimum-time trajectory
- **up to 11%** for the multi-objective (time + energy) trajectory

This work was published in the *International Journal of Robotics and Automation* (2023) — see the [journal article](/publications/spot-welding-trajectory-2023/).

compared with the manually programmed trajectories in use.

![Row of spot-welding robots on the line](robot-line.jpg)

![Body-in-white production floor](production-floor.jpg)

![Spot-welding station on the body-production line](welding-station.jpg)


