# Event-Driven Architecture Template

This repository outlines an event-driven architecture with producers, consumers, and shared event contracts.

Producers publish domain events, and consumers react to them asynchronously. This pattern supports loose coupling and reactive workflows.

## Folder Structure

producers/
  order-service/     - emits order-related events
  customer-service/  - emits customer-related events

consumers/
  analytics/         - consumes events for analytics
  reporting/         - consumes events for reporting

events/
  schemas/           - event definitions and contracts

shared/
  messaging/         - messaging infrastructure helpers

tests/               - unit, contract, and integration tests

docs/
  architecture.md
  decisions.md
