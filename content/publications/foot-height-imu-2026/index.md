---
title: "Real-Time Foot Height Estimation and Activity Classification Using a Foot-Mounted IMU Implemented on a Smartphone"
authors:
  - me
  - Babak Hejrati
date: "2026-05-16T00:00:00Z"
publishDate: "2026-05-16T00:00:00Z"
publication_types: ["article-journal"]
publication:
  name: "Sensors"
  volume: 26
  issue: 10
  pages: "3166"
peer_reviewed: true
open_access: true
abstract: "We developed a real-time, single-IMU smartphone system that reconstructs continuous foot-height trajectories and simultaneously classifies five locomotion activities entirely on-device. A Zero Height Change (ZHC) constraint corrects the cumulative vertical drift that limits conventional zero-velocity methods, while a heel-strike velocity feature drives adaptive activity classification. Validated on twenty adults, the system reached 96.08% classification accuracy with less than one gait-cycle latency and kept cumulative height errors below 1.1 cm across ramp and stair negotiation — providing a practical basis for real-time gait intervention and fall prevention."
tags:
  - Wearable Sensing
  - Foot Clearance
  - Drift Correction
  - Zero Height Change
  - Object Crossing
  - Locomotion Activities
  - Smartphone Applications
featured: true
image:
  caption: "Real-time foot height estimation from a foot-mounted IMU"
  focal_point: "Center"
  preview_only: false
projects: []
slides: ""
links:
  - type: pdf
    url: "/uploads/foot-height-imu-2026.pdf"
  - name: DOI
    url: "https://www.mdpi.com/3889232"
---

## Why it matters

Tripping is a leading cause of falls, and it is closely tied to how high we lift our feet while walking. Measuring **foot clearance** continuously, out in daily life, could flag fall risk early — but doing it well with a wearable sensor is hard:

- A single inertial measurement unit (IMU) drifts, so integrated foot height accumulates error over time.
- The usual fix (zero-velocity updates) does not fully remove **vertical** drift.
- More accurate methods work only **offline** and do not tell you what activity the person is doing.

## What I built

A **real-time, single-IMU system that runs entirely on a smartphone** — no cloud, no multi-sensor setup. It reconstructs the foot's height trajectory stride by stride *and* classifies five locomotion activities (level walking, ramp ascent/descent, stair ascent/descent) at the same time.

![The IMU is mounted on top of the foot; the toe position is recovered from the sensor pose by a rigid-body transformation](imu-toe-schematic.jpg)

Key contributions:

- **On-device Android app** for stride-by-stride foot-clearance measurement and live activity classification.
- **Zero Height Change (ZHC) constraint** — a biomechanically grounded correction that cancels cumulative vertical drift at each stride boundary.
- **Heel-strike velocity error** used as a compact, physically meaningful feature to adaptively pick the right reconstruction model per activity.
- **Toe-height estimation** from the IMU pose through a rigid-body transformation, with accuracy comparable to the foot itself.

![The custom Android app: (a) system and sensor controls, (b) activity labeling, (c) live activity detection with gait parameters, (d) deployment on stairs](app-interface.jpg)

## Validating the height measurement

The reconstructed foot trajectories separate cleanly by activity, and the continuous height signal tracks real-world ramps and stairs across a full walking circuit.

![Reconstructed foot trajectories for the five activities; dashed boxes mark stair entry/exit transition strides](foot-trajectories.jpg)

![Continuous foot-height trajectory across a full circuit of level ground, ramps, and stairs, with zero-velocity points marked](foot-height-activities.jpg)

To confirm the system measures real clearance, participants stepped over boxes of known heights and the estimated peak stride height was checked against each obstacle.

![Obstacle-clearance validation: participants step over boxes of increasing height, and the peak vertical displacement is compared against each box](obstacle-clearance.jpg)

## Results

- **96.08%** overall activity-classification accuracy, with **less than one gait cycle** of latency.
- Level walking stayed at the ground reference (**0.0 cm**, 95% CI −1.8 to 1.8 cm).
- Cumulative height error stayed **below 1.1 cm** across ramp and stair negotiation (mean absolute error **0.42%**).
- Toe height was recovered with accuracy comparable to foot height.

Together, this gives a practical foundation for **real-time gait feedback and fall-prevention** tools that could one day run on the phone already in someone's pocket.