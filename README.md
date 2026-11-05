# PermitLink – LGU Business Permits Integration

ITPC 313 – System Integration and Architecture | Team Nexora
Instructor: Neal Errol K. Bulawan

## Overview

Integrates a Permit Application System, a Treasury System, and a
Notification Service so applicants no longer carry proof of payment
between offices.

## Integrations

1. REST: Permit System -> GET /payments/{applicationId} -> Treasury System
2. Broker: Treasury System publishes payment.posted -> Permit System consumes
3. Event: Permit System publishes permit.approved -> Notification Service sends
   notice

## Data

Synthetic data only (business name, owner name, payment amount).
No real personal data is used.

## Team

- Jose Arym Diaz III – Project Lead / Architect
- Princess Haneen Dibarosan – Integration Developer
- Jericho M. Fegason – Data and Security Lead
- Hannah L. Alcantara – QA and Documentation Lead

## Repository Structure

```
/docs                  proposal, diagrams, consultation minutes
/permit-service
/treasury-service
/notification-service
/docker-compose.yml
```

## Run

```
docker compose up
```

## Status

Prefinal Week 1: proposal parts 1-7 drafted, repository created.
