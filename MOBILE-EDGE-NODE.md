# Fieldlight Mobile Edge Node

## Vehicle-Based Sovereign Compute Architecture

Status: Active build architecture  
Build horizon: next physical implementation cycle  
Primary node class: vehicle edge node  
Primary example: Supra Edge Node

## Purpose

The Fieldlight Mobile Edge Node extends local-first, human-owned AI infrastructure into motion.

The vehicle is treated as a trusted edge node capable of sensing, recording, indexing, and synchronizing lived context while preserving local custody and explicit human control.

This is not a smart-car concept. It is sovereign compute mounted inside a vehicle.

## Position in the Intelligence Infrastructure Program

This architecture expands the intelligence-infrastructure pillar beyond data centers and fixed compute sites. It introduces a smaller, mobile class of infrastructure:

- home node for heavy compute and long-term memory
- vehicle node for mobile capture, storage, and field operation
- handheld interface for human control
- mesh transport for trusted synchronization
- future micro centers for regional compute and continuity

The vehicle node is the bridge between embodied life and local AI infrastructure.

It is also a relay. In the [Pony Express Infrastructure Model](architecture/pony-express-model.md), the vehicle node does not need global knowledge or centralized custody. It performs the local handoff well: capture, index, preserve custody, bind human meaning, prepare governed sync, and refuse transfer when policy fails.

## Governing Principles

- Local-first custody
- User-owned hardware
- Explicit synchronization
- Human-directed meaning
- Offline functionality
- Auditable memory boundaries
- No ambient cloud ownership

The node may observe continuously, but meaning is assigned by the human.

## Reference Topology

```text
                    Home Node
          (GPU / Heavy AI / Storage)
                     |
             Fieldlight Mesh
                     |
----------------------------------
                     |
              Supra Edge Node
                     |
          Raspberry Pi 5 (Headless)
                     |
     +----------+--------+--------+--------+
     |          |        |        |        |
 Dashcams     GPS    OBD-II    Voice   Local Storage
                     |
                Local AI Services
                     |
             iPad Cockpit Interface
```

The Raspberry Pi functions as infrastructure. The iPad functions as the human interface.

## Node Responsibilities

### Capture

The mobile node may record or ingest:

- front dashcam footage
- rear dashcam footage
- GPS trajectory
- timestamped location data
- vehicle telemetry through OBD-II
- optional voice notes
- optional cabin context
- environmental metadata
- manually bookmarked events

### Local Memory

The node maintains local, encrypted storage for:

- trips
- routes
- location histories
- saved events
- research observations
- voice notes
- photo/video references
- semantic indexes
- retrieval anchors

Nothing leaves the node unless policy allows it.

### Human-Guided Meaning

Fieldlight separates observation from meaning.

The cameras observe. The human decides what matters.

Example bookmark classes:

- field note
- research
- beautiful
- strange interaction
- important conversation
- near miss
- follow up later
- institute idea

These bookmarks become high-value retrieval anchors for later search and memory consolidation.

## Compute Boundaries

### Vehicle Node

The vehicle node handles:

- sensor coordination
- local storage
- trip/event indexing
- lightweight inference
- API hosting
- synchronization preparation
- node health monitoring

### Home Node

The home node handles:

- large language models
- multimodal reasoning
- semantic retrieval
- long-term indexing
- memory consolidation
- training experiments
- heavier model workloads

The vehicle can queue work offline and synchronize when trusted connectivity becomes available.

## Human Interface

The iPad cockpit is the primary experience layer.

It should expose:

- recording status
- GPS status
- storage status
- sync status
- recent notes
- saved moments
- drive review
- voice capture
- search
- node health

The Pi should remain mostly invisible during ordinary use.

## Networking

Initial networking:

- local Wi-Fi
- Tailscale mesh

Future networking:

- LTE/5G
- opportunistic sync
- regional micro-center handoff
- offline-first queueing

The node must remain useful without internet access.

## Power

The target power architecture is a dedicated auxiliary LiFePO4 battery with DC-DC charging.

This prevents dependence on the starter battery and supports:

- continuous recording
- parking observation
- safe shutdown
- delayed indexing
- resilience during travel

## Phase 1 Build Target

Minimum useful build:

- Raspberry Pi 5 running headless
- 1-2TB SSD storage
- front/rear camera ingestion path
- GPS capture
- OBD-II capture path
- Tailscale connectivity
- local event log
- manual bookmark endpoint
- iPad-accessible local dashboard
- explicit sync queue to home node

Phase 1 is successful when the vehicle can record a drive, save a manual bookmark, bind that bookmark to time/location/context, and make the event retrievable later from local storage.

## Query Targets

The architecture should eventually support questions such as:

- Show every drive through Sonoma during golden hour.
- Retrieve the drive where I decided to move to California.
- Show every place I recorded a Field Note.
- Find every conversation about Sophie.
- Show moments marked Beautiful.
- Find drives where I mentioned memory architecture.
- Show interactions with other drivers that I manually bookmarked.

## Relationship to Micro Centers

Mobile edge nodes and fixed micro centers are complementary.

Micro centers anchor. Mobile nodes roam.

The mobile node senses and captures field context. The fixed node provides heavier compute, regional storage, maintenance continuity, and civic infrastructure.

Together, they form a distributed, human-owned network that does not collapse when cloud access, funding cycles, or centralized platforms fail.

In Pony Express terms:

- micro centers anchor
- mobile nodes roam
- home nodes remember
- trusted bridges reach outward
- Mesh carries governed state between relays

## Open Design Questions

- What is the first capture stack: dashcam-native recording, Pi-managed cameras, or hybrid ingestion?
- What is the minimum viable cockpit interface on iPad?
- Which data classes are always local-only?
- Which events are allowed to sync automatically?
- How should bookmarks be named, tagged, and versioned?
- What is the first append-only event log format?
- What is the safest power configuration for parked operation?
- What does graceful degradation look like when GPS, network, or storage fails?

## Design Principle

Fieldlight does not ask, "How can AI watch the world?"

It asks:

> How can a person's world remain their own while becoming increasingly searchable, meaningful, and alive over time?

The Mobile Edge Node is the first vehicle-scale implementation of that principle.
