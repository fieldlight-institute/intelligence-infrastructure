# Trusted Bridge Delegation

Status: Architecture note 0.1  
Created: July 2026

Fieldlight treats hosted AI systems as delegated bridges, not as the source of identity, memory, policy, or authority.

The local node remains the source of truth.

Cloud systems may provide capability.

They do not become the constitutional center.

## Core Claim

The important question is not only where intelligence runs.

The important question is where legitimacy lives.

In Fieldlight:

- local node equals legitimacy
- hosted model equals capability
- governance equals permission
- cryptographic identity equals proof
- delegation equals temporary authority

The person does not ask:

> Which AI owns this task?

The person asks:

> Who do I authorize to act on my behalf for this task?

That distinction is the trust model.

## Authority Shape

The Fieldlight authority path is:

```text
Human
  |
Sanctum / local authority
  |
Signed delegation grant
  |
Delegate environment
  |
Result, refusal, or audit trace
```

Delegate environments may include:

- a local model
- a local agent
- ChatGPT
- Codex
- OpenAI-hosted models
- a safe-hosted model operated by a trusted collaborator
- a future model or service

The execution environment may change.

The constitution does not move.

## Trusted Bridge

A trusted bridge is an external capability provider authorized to act through a local grant.

It may:

- receive task context
- use tools scoped by policy
- operate on selected artifacts
- communicate with outside systems
- return work products
- produce an audit trace

It may not:

- claim ownership of memory
- expand its own authority
- retain private context beyond the grant
- rewrite consent state
- become the source of identity
- treat platform access as user permission

In this model, ChatGPT, Codex, and other hosted systems are ambassadors.

They may represent the person outward.

They do not rule inward.

## Delegating Authority, Not Only Tasks

Most software delegates tasks.

Fieldlight delegates authority.

A task delegation says:

> Do this.

An authority delegation says:

> You may act on my behalf within this boundary, for this purpose, under this identity, until this condition ends.

That grant should be:

- signed
- scoped
- time-bounded or condition-bounded
- revocable
- inspectable
- logged
- understandable to the person
- enforceable by local policy

No valid grant means no authority.

## Grant Contents

A trusted bridge grant should define:

- granting human identity
- granting node identity
- delegate identity
- delegated task or role
- permitted resources
- prohibited resources
- permitted tools
- network permissions
- memory permissions
- publication permissions
- retention limits
- expiration condition
- revocation path
- audit requirements

The grant should be readable by both machines and humans.

## Memory Rule

Memory remains under local authority.

A hosted delegate may receive memory fragments only when a grant permits them.

Memory exposure should be treated as a scoped capability, not an ambient feature.

The local node should be able to answer:

- which memory was made visible
- why it was made visible
- to which delegate
- under what grant
- for how long
- what came back from the interaction

## Codex As Representative

Codex is especially useful as a trusted bridge because it can act across public and technical surfaces:

- repositories
- code
- documents
- publication surfaces
- issue and pull request workflows
- local files
- remote APIs

In Fieldlight terms, Codex should not be treated as a developer with ambient access.

Codex should be treated as a delegated representative acting under a signed local grant.

That means each meaningful action should be traceable to:

- user intent
- local authorization
- tool scope
- changed artifacts
- external systems contacted
- publication or push events

## Relationship To Existing Layers

This note does not replace Sanctum, Consent Gate, Kestrel Gate, or Mesh.

It clarifies their relationship.

### Sanctum

Sanctum is the local authority and continuity layer.

It holds identity, memory, consent state, authorship state, and the record of what may be delegated.

### Consent Gate

Consent Gate marks intentional invocation.

It helps prove that an action began from a human-authored, local act rather than from ambient system behavior.

### Kestrel Gate

Kestrel Gate evaluates whether a proposed action should proceed.

It is the preflight and audit layer for scripts, agents, tool use, network actions, file mutation, sync, export, and publication.

### Mesh

Mesh carries delegated action across nodes.

It should transport not only messages, but the authority state attached to those messages.

## Conflict Check

This architecture does not conflict with local-first AI.

It makes local-first AI more precise.

Local-first does not mean every capability must run locally.

It means authority, identity, memory, consent, and revocation remain local even when capability is delegated outward.

This architecture also does not conflict with use of hosted models.

It changes their role.

Hosted models become powerful bridges to outside capability, not custodians of the self.

## Design Rule

Authority remains local.

Capability may be delegated outward.

Every delegate must be able to answer:

> Who authorized me, under what proof, for what scope, and what must I return to the local record?

