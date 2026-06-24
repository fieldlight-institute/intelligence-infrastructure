# Sovereign Personal Computing Stack

Status: Architecture note 0.1  
Created: June 2026

Fieldlight treats personal computing as infrastructure that should be owned by the person.

The work is not to build another application, SaaS product, or mesh tool. The work is to define a coherent stack in which hardware, operating system, identity, memory, agents, communication, publication, and archive share one governing philosophy.

Short form:

> Mac-level coherence. Linux-level ownership. Human-level consent.

## Core Claim

The personal computer is becoming the site where AI systems touch memory, authorship, identity, attention, work, relationships, and public life.

That makes the machine a governance surface.

A Fieldlight-native system should not treat the person as an account inside a platform. It should treat the person as the owner of the machine, the memory substrate, the identity layer, and the authority grants by which agents act.

## Stack Layers

### Hardware

The physical trust boundary.

Hardware defines what can be sensed, stored, accelerated, repaired, replaced, secured, and disconnected.

Questions:

- What sensors exist?
- What secure hardware exists?
- What can be physically disabled?
- What can be repaired?
- What remains usable without cloud services?
- What compute is available locally?

### Operating System

The enforcement layer.

The OS decides what can run, see, remember, change, share, publish, sync, and leave the machine.

Questions:

- What is local by default?
- What is network-visible by default?
- What requires explicit consent?
- How are agent capabilities granted and revoked?
- How are memory, identity, and provenance exposed to applications?

### Identity

The continuity layer.

Identity is not merely login. It is the durable link between person, devices, keys, memory, authority, authorship, recovery, and archive.

Questions:

- Where do keys live?
- How is a device trusted?
- How does identity survive device replacement?
- How is recovery possible without surrendering custody?
- How are human, device, and agent identities distinguished?

### Sanctum

The memory and authorship substrate.

Sanctum is not only an app. In the Fieldlight stack, Sanctum becomes part of the operating substrate: the place where private memory, source trace, authorship, consent states, personal continuity, and agent context are governed.

Questions:

- What belongs to private memory?
- What memory can an agent access?
- What memory is shared?
- What memory is model-visible?
- What memory can be forgotten, sealed, exported, or archived?

### Agents

The delegated action layer.

Agents act through scoped authority. They should not inherit ambient power from apps, accounts, or sessions.

Questions:

- What grant authorizes this action?
- What can the agent read?
- What can the agent write?
- What can the agent send?
- What can the agent buy, execute, publish, delete, or remember?
- What record remains after action?

### Mesh

The communication and collaboration layer.

Mesh governs shared presence, private channels, collaboration, sync, and movement between personal nodes.

Questions:

- Who can see what?
- What is shared with whom?
- What moves peer-to-peer?
- What requires a relay?
- What remains private even during collaboration?

### Town Square

The public expression layer.

Town Square is the intentionally public surface. It distinguishes publication from leakage and public authorship from platform capture.

Questions:

- What has been intentionally published?
- What trace and licensing follow it?
- What relationship exists between a public artifact and its private source?
- What can be cited, mirrored, remixed, or withdrawn?

### Archive

The continuity over time layer.

Archive governs durable records, migration, inheritance, institutional memory, and long-term preservation.

Questions:

- What survives hardware replacement?
- What survives account loss?
- What survives institutional failure?
- What should be portable?
- What should be sealed?
- What should be inherited?

## Design Principle

Every layer should preserve the difference between:

- local
- private
- shared
- synced
- agent-visible
- model-visible
- published
- archived

If the system cannot name the difference, it cannot govern the difference.

