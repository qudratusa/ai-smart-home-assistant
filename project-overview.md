# Project Overview

## Problem

Smart-home systems can improve convenience, but many rely on preset routines, fragmented device ecosystems, and cloud processing. The project investigates how a smart-home assistant could become more adaptive while maintaining user trust and privacy.

## Design Approach

The project followed a design-first methodology with four main activities:

1. **Simulated device interaction** — mapped scenarios involving devices such as a smart doorbell, smart speaker, thermostat, lights, cameras, and robot vacuum.
2. **Pattern-detection planning** — identified behaviors an eventual ML system could learn, such as repeated nighttime thermostat changes, and anomalies it could flag, such as unusual vacuum power usage.
3. **Figma prototyping** — designed interactive screens for the home dashboard, routine management, temperature controls, privacy controls, and other device interactions.
4. **Privacy-by-design** — designed around local data storage/processing, user-configurable collection, and transparent data-activity information.

## Prototype Results

The Figma prototype demonstrates:

- a unified dashboard for connected devices;
- customizable routines and AI-suggested optimizations;
- anomaly alerts;
- a privacy dashboard for collection/storage preferences and usage visibility;
- device-specific controls for cameras, temperature, and vacuum scheduling;
- contextual voice-assistant interactions.

## Important Limitation

This repository represents a **proof-of-concept design**, not a deployed AI smart-home system. The original project did not implement live machine-learning models, real-time smart-device data collection, or commercial smart-home APIs. Accessibility support also remains incomplete.

## Technical Roadmap

### Phase 1 — Functional prototype

- Build a simple application shell around the existing interaction design.
- Model devices and routines with synthetic/local data.
- Persist preferences and privacy settings locally.

### Phase 2 — Personalization and anomaly detection

- Build a small behavior-event schema.
- Start with interpretable baselines for routine prediction.
- Add anomaly-detection experiments and confidence/uncertainty indicators.
- Keep user approval in the loop for consequential automation.

### Phase 3 — Device integrations

- Design an adapter layer for multiple smart-home ecosystems.
- Add authentication/permissions carefully per platform.
- Keep device data isolated according to user-selected permissions.

### Phase 4 — Privacy-preserving edge AI

- Evaluate lightweight inference approaches such as quantized models or TinyML where appropriate.
- Explore on-device/edge inference to reduce cloud dependency.
- Add audit logs, data-expiration controls, and fine-grained permissions.

### Phase 5 — Evaluation

- Conduct usability testing with diverse participants.
- Measure trust, perceived control, usefulness of suggestions, and false-alert burden.
- Run longer-term studies to evaluate changing routines and user expectations over time.

## Ethical and HCAI Considerations

Future development should continue to prioritize informed consent, user agency, clear explanations, privacy controls, safety when commands conflict, and accessibility. Technical accuracy should not come at the expense of understandable interaction or user control.
