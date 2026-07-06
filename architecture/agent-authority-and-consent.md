# Agent Authority And Consent

Status: Architecture note 0.1  
Created: June 2026

Agents in a Fieldlight-native system should not be treated as chat boxes with broad application access.

They are delegated actors.

Delegated actors require authority.

Hosted AI systems are delegated actors too.

ChatGPT, Codex, OpenAI-hosted models, local models, and safe-hosted collaborator models should all be treated as execution environments that may receive authority from the local node. They do not become the source of authority themselves.

## Principle

An agent may act only through an explicit grant.

A grant should be:

- named
- scoped
- revocable
- time-bounded or condition-bounded
- inspectable
- logged
- understandable to the person granting it

No grant, no authority.

## Trusted Bridge Delegation

Some delegates operate outside the local machine.

Fieldlight calls these trusted bridges: external capability providers authorized by the local node to act on the person's behalf.

A trusted bridge may help with code, writing, research, publication, remote APIs, repositories, or outside communication, but it acts through a local grant.

The local node remains responsible for:

- identity verification
- memory exposure
- consent state
- resource scope
- revocation
- audit trace

The hosted model provides capability.

It does not own policy, memory, identity, or continuity.

See [Trusted Bridge Delegation](trusted-bridge-delegation.md).

## Kestrel Gate

Kestrel Gate is the Fieldlight continuity name for the local agent security layer.

In conventional security terms, it is a local-first preflight security and audit layer for agent, script, file, network, sync, and export actions. The name preserves continuity with Fieldlight's Kestrel OpSec language, while the implementation should be documented using standard security terminology wherever possible.

The security layer sits before delegated action and evaluates whether a protected action should be allowed to touch the system at all.

In Phase 1, it operates in `warn + ask` mode:

- create a preflight request
- classify visible risk
- explain the policy concern in human language
- request explicit human approval
- record the policy decision
- write an audit event

Consent Gate remains one mechanism inside this larger security layer. Consent Gate marks intentional invocation; the preflight layer decides whether the invocation should proceed.

## Authority Surfaces

Agent authority should be modeled across several surfaces:

- files and folders
- private memory
- project memory
- identity credentials
- contacts and relationships
- network access
- local applications
- shell and system commands
- purchases and financial actions
- messages and publication
- sensors and local device state
- archival actions

Each surface should support least-necessary access rather than ambient permission.

## Consent States

The operating system should distinguish:

- local use
- private memory access
- shared memory access
- model-visible context
- third-party service transmission
- publication
- archival export
- deletion or forgetting

These states should not be collapsed into a single "allow" button.

## Grant Shape

A grant should include:

- who granted authority
- which agent received authority
- what resources are covered
- what actions are permitted
- whether network access is permitted
- whether memory access is permitted
- whether outputs may be shared or published
- when the grant expires
- how the grant can be revoked
- what audit record is retained

## Audit Record

Every meaningful agent action should leave a record sufficient to answer:

- What acted?
- Under whose authority?
- Using what grant?
- On what resources?
- With what input context?
- What changed?
- What left the machine?
- What was remembered?
- What was refused?

This record is not surveillance of the person. It is accountability for delegated power.

## Human Terms

Permissions should be legible in human terms.

Instead of only saying:

> Agent may access ~/Documents.

The system should be able to say:

> This agent may read the project folder for the Fieldlight architecture draft until Friday. It may summarize files locally. It may not send file contents to external services or publish outputs without a separate grant.

The grant should preserve both machine enforceability and human meaning.
