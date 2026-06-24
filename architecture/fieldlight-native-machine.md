# Fieldlight-Native Machine

Status: Architecture note 0.1  
Created: June 2026

A Fieldlight-native machine is not defined first by form factor, chip vendor, industrial design, or brand.

It is defined by the experience and authority model it makes possible.

## Definition

A Fieldlight-native machine is a human-owned computer whose hardware and operating system are designed around memory ownership, local-first identity, consent enforcement, agent authority, and continuity across time.

It is a trust boundary made physical.

## Constitutional Questions

Before hardware selection, the machine must answer:

- Who owns memory?
- Where does identity live?
- What can leave the machine?
- What requires consent?
- How do agents get authority?
- What survives hardware replacement?
- What is public by default?
- What is local by default?

These are operating-system decisions before they are product features.

## Minimum Properties

### Local-First Operation

The machine should remain meaningful without a cloud account. Cloud services may extend the system, but they should not own the core identity, memory substrate, or agent authority model.

### Inspectable Memory

Private memory should be human-readable or at least human-auditable. The person should be able to inspect what is remembered, what used it, and what permissions govern it.

### Scoped Agent Authority

Agents should operate through grants. A grant should specify scope, duration, permitted resources, permitted actions, network rights, memory rights, and revocation conditions.

### Provenance By Default

Files, memories, public artifacts, agent actions, and shared outputs should preserve trace: origin, author, context, revision, permission, and use.

### Consent-Gated Egress

The machine should know when information is leaving a local/private context for sync, sharing, publication, model use, or archival export.

### Continuity And Recovery

The person should be able to replace hardware without surrendering identity or losing memory, authorship trace, permission history, agent records, and archive continuity.

### Repairability And Physical Trust

The hardware path should prefer repairability, documented components, physical privacy controls, secure boot, encrypted storage, and visible sensor posture.

## Product Path

Fieldlight should not begin by building a laptop.

The proposed sequence:

1. Custom Linux distribution or OS layer.
2. Reference hardware specification.
3. Prebuilt machine on existing hardware.
4. Custom hardware only after the OS has taught the requirements.

This follows the practical lesson of coherent Linux hardware companies: start by defining the experience and control plane, then use hardware to embody it.

## Reference Implementation Direction

The first reference node is Astra: a lived Fieldlight node that proves the stack through one person's real machine, work, memory, agents, relationships, publications, and archive.

Astra is not a demo account.

It is the first lived node.

