# Agent Authority And Consent

Status: Architecture note 0.1  
Created: June 2026

Agents in a Fieldlight-native system should not be treated as chat boxes with broad application access.

They are delegated actors.

Delegated actors require authority.

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

