# PayOpsKit

PayOpsKit is an open-source payment operations toolkit for validating, visualising, tracing, replaying, and governing modern payment messages.

Initial support focuses on ISO 20022 payment flows, starting with:

- pacs.008
- pacs.002

PayOpsKit is not a payment processor or payment hub.

It is the operational layer around modern payment systems.

---

# Vision

Modern payment systems still lack cloud-native operational tooling for:

- validation
- replay
- tracing
- observability
- schema governance
- operational investigations

PayOpsKit aims to provide a developer-first and operations-friendly platform for payment engineering.

---

# Current Phase

Phase 1 focuses on:

- ISO 20022 message upload
- message type detection
- XSD validation
- business rule validation
- XML tree visualisation
- synthetic message generation
- local Docker-based deployment

---

# Architecture

```text
React UI
    ↓
Spring Boot WebFlux API
    ↓
ISO 20022 Parser
    ↓
Validation Engine
    ↓
Postgres
```

Future phases will introduce:

- Redpanda/Kafka
- payment replay
- OpenTelemetry tracing
- OpenSearch
- schema registry
- operational dashboards
- multi-standard support

---

# Quick Start

## Clone

```bash
git clone https://github.com/openpayops/payopskit.git
cd payopskit
```

## Start locally

```bash
docker compose up
```

## Open UI

```text
http://localhost:3000
```

---

# Repository Structure

```text
apps/
modules/
deploy/
examples/
docs/
```

---

# Technology Stack

- Java 21
- Spring Boot WebFlux
- React + TypeScript
- Maven multi-module
- Postgres
- Docker Compose

Future:
- Redpanda/Kafka
- OpenSearch
- OpenTelemetry
- Cassandra

---

# Roadmap

## Phase 1
- ISO 20022 validator
- XML tree viewer
- synthetic message generator

## Phase 2
- payment journey model
- replay engine
- event streaming

## Phase 3
- operational search
- observability
- tracing

## Phase 4
- schema registry
- compatibility validation
- multi-standard support

---

# Contributing

Contributions, feedback, architecture discussions, and ideas are welcome.

See:
```text
/docs
```

for architecture and roadmap details.

---

# License

[Apache License 2.0 ](./LICENSE)
