# Guest AI System

## Why?
- Core to the game loop: simulates real-life guest behaviors and challenges.
- Drives player engagement, stress, and narrative moments.
- Modular design allows expansion (VIPs, scammers, event guests).
- Documenting "why" ensures clarity, avoids cargo cult coding, and allows future contributors to understand each decision.

## What?
- Guest spawns with randomized traits (patience, demands, wealth, archetype).
- Pathfinding to front desk, assigned room, amenities, and exits.
- Patience meter that decreases with delays or mishandling. Impacts guest behavior and player reputation.
- Interacts with Property Management System (PMS), can trigger dialogue, and generates events (complaints, reviews).
- Modular logic to support future features (VIPs, event guests, criminal archetypes, etc.).

## How?
- **Unreal:** Blueprint/C++ AIController, Behavior Tree, Blackboard for guest data, NavMesh for pathfinding.
- **Web:** TypeScript class for Guest, state machine pattern, A* pathfinding library for navigation. Modular guest archetypes as subclasses or strategy pattern.

## Version History
- **v1.0:** Basic guest spawn, randomized patience, and pathing to front desk and assigned room.
- **v1.1:** Patience meter tied to player actions, triggers feedback (complaints, rushes).
- **v1.2:** Guest archetypes (VIP, scammer, critic) introduced.
- **v1.3:** Integration with PMS and dialogue system.
- **v2.0+:** Event-driven guest behaviors, expansion to luxury/resort guests, dynamic guest relationship tracking.

---
> Update this file with each version and major design decision.