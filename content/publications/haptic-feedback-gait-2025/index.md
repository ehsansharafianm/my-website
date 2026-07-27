---
title: "The Effects of Real-Time Haptic Feedback on Gait and Cognitive Load in Older Adults"
authors:
  - me
  - Colby Ellis
  - Ben Sidaway
  - Marie Hayes
  - Babak Hejrati
date: "2025-06-11T00:00:00Z"
publishDate: "2025-06-11T00:00:00Z"
publication_types: ["article-journal"]
publication:
  name: "IEEE Transactions on Neural Systems and Rehabilitation Engineering"
  volume: 33
  pages: "2335-2344"
peer_reviewed: true
abstract: "Slower walking speed is one of the clearest warning signs of declining mobility in older adults, and it often comes from neuromotor changes rather than weak muscles or poor fitness. We built a wearable, smartphone-based system that delivers gentle vibration to the thighs during walking to nudge each step toward greater peak thigh extension (PTE), which in turn lengthens the stride and raises walking speed. In thirty community-dwelling older adults (79.9 years on average), a single session with the haptic system increased stride length by 14% and gait speed by 18%, matching the gains from verbal coaching. A probe reaction-time task showed the added mental effort was small (27 to 74 ms), so the feedback improved gait without overloading attention, making it a practical option for gait training in older adults."
tags:
  - Haptic Feedback Systems
  - Gait Analysis
  - Fall Prevention in Older Adults
featured: true
image:
  focal_point: ""
  preview_only: false
projects: []
slides: ""
links:
  - type: pdf
    url: "/uploads/haptic-feedback-gait-2025.pdf"
  - name: DOI
    url: "https://doi.org/10.1109/TNSRE.2025.3578865"
---

## Why it matters

Walking speed is one of the strongest predictors of health and independence in later life, and when it drops the cause is often **neuromotor**, the timing and coordination of movement, rather than weakness or poor fitness. A key culprit is reduced **peak thigh extension (PTE)**, how far the thigh swings back at the end of each step. If we could cue people to extend the thigh a little more, in real time and out in the world, we could lengthen their stride and speed them up, without a treadmill, a therapist, or a lab.

## What I built

A **wearable, smartphone-based haptic feedback system**. Two IMUs track the thigh and foot angles, the phone computes PTE stride by stride, and small **vibrotactile cells on the thighs** deliver a gentle cue when a step needs adjusting.

![The closed-loop system: IMUs stream thigh and foot angles to the phone over Bluetooth, which commands vibrotactile feedback on the thighs; right, a participant wearing the modules, IMUs, and vibrotactile cells](haptic-system.jpg)

How the feedback works:

- Each stride's **PTE is compared to a personalized target**.
- Two feedback strategies were tested: a cue when the step was **incorrect** (PTE below target, F_IR) and a cue when the step was **correct** (target met, F_CR).
- A third group received only **verbal instructions** (I_V), as a benchmark for the haptic system.

![Left, the thigh and foot angle over a gait cycle with heel strike and PTE marked; middle and right, the incorrect-response and correct-response feedback strategies relative to the target thigh extension](pte-feedback-logic.jpg)

## Measuring the mental cost

Any gait cue is only useful if people can follow it without concentrating so hard that they stop paying attention to their surroundings. To measure that **cognitive load**, participants did a probe reaction-time task while walking, responding to audio beeps, with reaction time measured precisely from the sent and received audio.

![The probe reaction-time setup: audio beeps are sent and the participant's spoken response is captured, and the delay between them is measured as reaction time](reaction-time-measurement.jpg)

## Results

- **+14% stride length** and **+18% gait speed** from a single session with the haptic system.
- Gains were **comparable to verbal coaching**, but reached through a different mechanism (direct thigh feedback rather than instruction).
- Added cognitive load was **small**: reaction time rose only **27 ms (F_IR)** to **74 ms (F_CR)**.
- Thirty community-dwelling older adults, averaging about **80 years old**.

![Gait and cognitive-load outcomes across baseline, fast, and treatment trials for the three feedback groups: PTE, stride length, speed, cadence, and reaction time](results-bars.jpg)

Together this shows that real-time thigh haptics can meaningfully improve older-adult gait in a single session while keeping attentional demand low, a promising, low-cost path toward wearable gait training and fall prevention.