# HubSpot API Integration

**Direct HubSpot CRM integration (contacts, deals, companies) for clients who have outgrown Zapier or Make.**

> **This is a proprietary project. Source code is private. This page showcases the system's architecture and results.**

**Case study page:** [https://jryahia.github.io/showcase-hubspot-api-integration/](https://jryahia.github.io/showcase-hubspot-api-integration/)

![HubSpot API Integration](assets/00-api-dashboard.png)

## Problem it solves

No-code connectors hit limits on volume, logic and error handling. This service talks to the HubSpot CRM API v3 directly and gives the client app full CRUD with its own dashboard.

## Architecture

![Architecture](assets/architecture.svg)

1. The client app calls the integration's REST endpoints.
2. Requests go to HubSpot CRM API v3, or to a mock in demo mode.
3. Results are tracked for sync health.
4. The dashboard shows contacts, the deal pipeline and activity.

## Key features

- Contacts, deals and companies CRUD
- Kanban deal pipeline view
- Mock mode with realistic HubSpot-shaped data
- Validated configuration with safe fallbacks
- Sync statistics

## Tech stack

![Python](https://img.shields.io/badge/Python-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![FastAPI](https://img.shields.io/badge/FastAPI-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![HubSpot API](https://img.shields.io/badge/HubSpot%20API-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Jinja2](https://img.shields.io/badge/Jinja2-161b22?style=for-the-badge&labelColor=161b22&color=161b22)

## What it does in practice

- Replaces a chain of no-code zaps with one maintainable service.

## Screenshots

**Contacts, pipeline and sync health**

![Contacts, pipeline and sync health](assets/00-api-dashboard.png)

**Contacts, activity and companies**

![Contacts, activity and companies](assets/10-pipeline.png)

---

Built by [Yahya Jarray](https://github.com/jryahia). Interested in a similar system? [Get in touch](mailto:yahiajarray43@gmail.com).

This repository contains no source code. It is a case study for a proprietary project. © Yahya Jarray.
