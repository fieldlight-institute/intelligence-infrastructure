# Sovereign Personal Computing Stack

Status: Architecture note 0.2  
Created: June 2026  
Updated: June 2026

Fieldlight is designing a sovereign computing architecture from silicon to society.

The goal is not to build a Linux distribution, a laptop company, or an AI assistant. The goal is to define and build a successor architecture to personal computing: a human-owned system where authority originates with the person and is delegated outward.

The laptop is the first embodiment, not the category.

This includes hosted AI systems. Fieldlight does not require every useful intelligence capability to run locally. It requires that legitimacy remain local. Cloud systems may act as trusted bridges when they receive scoped, revocable authority from the local node.

It also includes relay infrastructure. Fieldlight does not require every workload to route through a distant hyperscale center. Local machines, vehicle nodes, home nodes, regional micro centers, and trusted bridges can form a Pony Express-style relay network where governed state moves through bounded handoffs.

## Core Architecture

The Fieldlight stack includes:

1. Silicon
2. Hardware
3. Firmware
4. Operating system
5. Identity
6. Sanctum
7. Agents
8. Mesh
9. Relay infrastructure
10. Authorship
11. Governance
12. Public space
13. Archive
14. Society

The stack is unified by one authority model.

The machine should understand:

- who it belongs to
- what it knows
- how it knows it
- what it is permitted to do
- who delegated that permission
- what left the machine
- what was remembered
- what was published
- how to explain itself

## Layer Responsibilities

### Silicon

Silicon defines the physical limits of local intelligence: model execution, memory bandwidth, secure computation, isolation, energy use, and embodied trust.

Architecture questions:

- What must run locally?
- What must be accelerated locally?
- What identity or key material requires hardware support?
- What forms of isolation must be physically enforced?
- What local inference envelope is required for ordinary use?

### Hardware

Hardware makes trust physical.

Architecture questions:

- What can be sensed?
- What can be physically disabled?
- What can be repaired?
- What compute, memory, and storage are needed for the whole loop?
- What battery, thermals, keyboard, display, camera, microphone, and speaker quality make this usable for normal people?
- What must remain functional without cloud services?

### Firmware

Firmware is the first authority boundary after power-on.

Architecture questions:

- What is allowed to boot?
- How is boot integrity verified?
- How are recovery and replacement handled?
- How does the system distinguish trusted, degraded, and compromised states?

### Operating System

The Fieldlight OS is the enforcement and explanation layer.

Architecture questions:

- What can run?
- What can see?
- What can remember?
- What can change?
- What can leave?
- What requires consent?
- What authority grant permits an action?
- What audit record remains?

### Identity

Identity defines belonging and continuity.

Architecture questions:

- Who does this machine belong to?
- How are person, device, agent, collaborator, service, and institution identities distinguished?
- How does identity survive hardware replacement?
- How does recovery work without surrendering custody?

### Sanctum

Sanctum is continuity, identity, memory, and agency.

Architecture questions:

- What belongs to the person's private continuity?
- What memory may agents use?
- What is source, memory, inference, preference, artifact, or archive?
- How are consent state and provenance preserved?
- How does a person inspect, seal, export, forget, or inherit memory?

### Agents

Agents are delegated actors.

Architecture questions:

- What grant authorizes the action?
- What can the agent read, write, remember, send, buy, publish, execute, or delete?
- When does the grant expire?
- What explanation does the agent owe?
- Is this agent local, remote, hosted, peer-operated, or institutional?
- What proof binds the delegate to the grant?

### Trusted Bridges

Trusted bridges are external capability providers acting under local authority.

Architecture questions:

- Which hosted systems may act on behalf of the person?
- What memory or context may be exposed to them?
- What tools may they use?
- What must remain local?
- What proof verifies the delegate identity?
- How is the grant revoked?
- What audit trace returns to Sanctum?

### Mesh

Mesh is inter-node communication and delegation.

Architecture questions:

- Which nodes trust each other?
- What is shared peer-to-peer?
- What requires relay infrastructure?
- What can be delegated across nodes?
- How are presence, collaboration, refusal, revocation, and trace handled?

### Relay Infrastructure

Relay infrastructure is the topology of bounded handoffs.

Architecture questions:

- Which nodes act as relays?
- What local work does each relay perform?
- What governed state travels with each handoff?
- What may be computed locally, forwarded, refused, or queued?
- How does the route survive relay failure or replacement?
- How do mobile nodes, home nodes, regional micro centers, and trusted bridges cooperate without centralizing authority?

### Authorship

Authorship preserves origin and rights.

Architecture questions:

- Who made this?
- From what source?
- With what contribution history?
- Under what permission?
- What is public, cited, mirrored, remixed, licensed, or withdrawn?

### Governance

Governance makes power legible.

Architecture questions:

- Who can grant authority?
- Who can revoke authority?
- What happens when grants conflict?
- How are disputes, refusals, errors, and harms recorded?
- How does the machine participate in institutional and civic governance without surrendering human authority?

### Public Space

Public space is intentional visibility.

Architecture questions:

- What has been intentionally published?
- What remains private behind the public artifact?
- How is public authorship preserved?
- How does the system resist platform capture?

### Archive

Archive is continuity over time.

Architecture questions:

- What survives device replacement?
- What survives account loss?
- What survives institutional failure?
- What should be inherited?
- What should be sealed?
- What should remain readable decades later?

### Society

Society is not an afterthought.

Architecture questions:

- What social order does this trust stack produce?
- Who gains power?
- Who loses extraction rights?
- What institutions become possible when machines are accountable to humans first?

## Design Rule

If the machine cannot distinguish a state, it cannot govern that state.

The system must distinguish:

- local
- private
- shared
- synced
- delegated
- agent-visible
- model-visible
- institution-visible
- published
- archived
- inherited
- revoked
