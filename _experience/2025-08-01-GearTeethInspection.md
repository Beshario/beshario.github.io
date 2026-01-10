---
layout: post
title: Gear Teeth Vision Inspection
subtitle: PLC-Integrated Machine Vision for CNC Quality Control
thumbnail-img: /assets/img/GearTeeth/standAloneStationInCell.jpg
tags: [robotics, automation, vision, PLC]
comments: true
categories: experience
---

**Customer:** Linamar
**Role:** Vision / Automation Engineer
**Via:** Ascension Automation Solutions
**Location:** Guelph, Ontario
**Timeline:** Aug 2025

---

#### The Challenge

A CNC machining line producing gears was experiencing intermittent quality escapes:

- CNC occasionally skips teeth during machining
- Operators can enter wrong dimensions
- Air supply instability leading to inconsistent part positioning
- Manual checks weren't catching edge cases

Stand-alone vision inspection station integrated into the production cell:

<div align="center">
<img src="/assets/img/GearTeeth/standAloneStationInCell.jpg" width="100%"/>
</div>

---

#### System Design

Designed a robust, PLC-integrated vision inspection system that detects missing or incorrect gear teeth, fits cycle-time constraints, and survives real factory conditions.

Camera, lens, lighting, and trigger strategy tuned specifically for teeth geometry. PLC-synchronized capture was critical — timing mattered a lot here.

Robot placing part before inspection:

<div align="center">
<img src="/assets/img/GearTeeth/robotPlaceb4inspection.jpg" width="100%"/>
</div>

---

#### Bench Testing

Built an offline bench test to simulate real-world failure modes:

- Bad air supply conditions
- Wrong dimension inputs
- Timing drift scenarios

Validated inspection logic before touching production equipment:

<div align="center">
<img src="/assets/img/GearTeeth/benchTestValidation.jpg" width="100%"/>
</div>

---

#### Controls & Software

Developed a **Python MVC application** to:

- Teach Fanuc robot points
- Run inspection cycles
- Log system state and faults

PLC debugging during commissioning focused on camera trigger timing and handshakes between Vision, PLC, and Robot systems.

Full inspection station overview:

<div align="center">
<img src="/assets/img/GearTeeth/robotPlaceInspectionO.jpg" width="100%"/>
</div>

---

#### Results

- Stable detection of missing and incorrect teeth
- Issues caught before parts reached downstream operations
- Smooth commissioning thanks to early bench validation
- Operators gained confidence in automated inspection

---

#### Demo Video

<iframe class="d-block mx-auto" width="560" height="315" src="https://www.youtube.com/embed/OldRA3Rxs5o" title="Gear Teeth Vision Inspection Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---

#### Tools and Technologies Employed

- Python (MVC Architecture)
- Fanuc Robot Programming
- PLC Integration
- Machine Vision Systems
- Bench Test Validation

