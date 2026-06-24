# Development Roadmap

Status: Architecture roadmap 0.1  
Created: June 2026

This roadmap keeps the hardware ambition grounded in the correct order of operations.

Fieldlight should not begin by manufacturing a laptop.

It should begin by defining what makes a machine Fieldlight-native.

## Phase 1: Operating Doctrine

Define the principles and boundaries:

- local by default
- consent as architecture
- identity continuity
- memory ownership
- agent authority by grant
- provenance by default
- public as intentional state
- archive as continuity over time

Primary artifacts:

- sovereign personal computing doctrine
- Fieldlight-native machine definition
- agent authority and consent model
- stack overview

## Phase 2: OS Architecture

Define the technical architecture for a Fieldlight OS layer.

Work areas:

- Linux base and update model
- encrypted local storage
- identity and key management
- local memory substrate
- agent permission broker
- audit log
- context firewall
- model/runtime integration
- UI surfaces for grants, memory, sharing, and publication

Primary artifact:

- Fieldlight OS architecture specification

## Phase 3: Prototype On Existing Hardware

Build the first working system on commodity hardware.

Candidate path:

- custom Linux distribution or image
- immutable or semi-immutable base
- local-first data layer
- agent runtime with scoped grants
- Sanctum memory substrate
- Mesh communication primitives
- Town Square publishing path
- Archive export and recovery workflow

Primary artifact:

- Astra reference node

## Phase 4: Reference Hardware Specification

Define hardware requirements after the OS architecture has made them visible.

Specification areas:

- CPU/GPU/NPU expectations
- memory and storage requirements
- secure boot and hardware root of trust
- physical privacy controls
- camera and microphone posture
- networking requirements
- repairability
- battery and thermal requirements
- peripheral support
- offline capability

Primary artifact:

- Fieldlight reference hardware spec

## Phase 5: Prebuilt Fieldlight Machine

Ship a coherent machine on existing hardware.

This phase should focus on:

- reliable installation
- driver support
- update safety
- onboarding
- backup and recovery
- visible consent surfaces
- agent authority UX
- memory migration
- repair and replacement story

Primary artifact:

- first prebuilt Fieldlight machine

## Phase 6: Custom Hardware

Consider custom hardware only after the OS, reference node, and prebuilt machine reveal requirements that existing hardware cannot satisfy.

Custom hardware should serve the doctrine, not replace it.

