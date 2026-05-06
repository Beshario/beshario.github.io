---
layout: post
title: Gear Teeth Vision Inspection
subtitle: PLC-Integrated Machine Vision for CNC Quality Control
thumbnail-img: /assets/img/GearTeeth/standAloneStationInCell.jpg
tags: [machine-vision, automation, PLC, Kuka, commissioning, inspection, Siemens]
comments: true
categories: experience
---

**Customer:** Linamar
**Role:** Vision Engineer
**Via:** Ascension Automation Solutions
**Location:** Guelph, Ontario
**Timeline:** Aug 2025

---

#### The Challenge

A CNC machining line producing gears was experiencing intermittent quality escapes:

- CNC occasionally skips teeth during machining
- Operators entering wrong dimensions
- Air supply instability causing inconsistent part positioning
- Manual checks missing edge cases

Stand-alone vision inspection station integrated into the production cell:

<div align="center">
<img src="/assets/img/GearTeeth/standAloneStationInCell.jpg" width="100%"/>
</div>

---

#### System Design

Designed a PLC-integrated vision inspection system to detect missing or incorrect gear teeth within cycle-time constraints and real factory conditions.

Camera, lens, lighting, and trigger strategy were tuned specifically for the cell geometry. PLC-synchronized capture timing was critical to reliable inspection.

Robot placing part before inspection:

<div align="center">
<img src="/assets/img/GearTeeth/robotPlaceb4inspection.jpg" width="100%"/>
</div>

---

#### Bench Testing

Built an offline bench test to simulate real-world failure modes before touching production equipment:

- Missing and incorrect tooth detection
- Wrong dimension input scenarios
- Camera and lighting proof of principle

<div align="center">
<img src="/assets/img/GearTeeth/benchTestValidation.jpg" width="100%"/>
</div>

---

#### Integration and Commissioning

Key integration work:
- Camera trigger timing optimization
- Vision to PLC handshake coordination
- Kuka robot teach points for part handling
- System validation and fault logging

Full inspection station overview:

<div align="center">
<img src="/assets/img/GearTeeth/robotPlaceInspectionO.jpg" width="100%"/>
</div>

---

#### Results

- Stable detection of missing and incorrect teeth
- Quality escapes caught before reaching downstream operations
- Early bench validation enabled smooth production commissioning
- Operators confident in automated inspection replacing manual checks

---

#### Demo Video

<iframe class="d-block mx-auto" width="560" height="315" src="https://www.youtube.com/embed/OldRA3Rxs5o" title="Gear Teeth Vision Inspection Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---

#### Tools and Technologies

- IFM Machine Vision Systems
- Siemens TIA Portal (PLC)
- Kuka Robot Programming
