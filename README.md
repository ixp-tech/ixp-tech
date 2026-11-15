# IXP · Real-world screen operations

**A digital signage project built around the realities of operating screens in physical spaces.**

A screen in a building has a location, a purpose, a configuration, and eventually content and a connected playback device. IXP aims to make those relationships understandable, manageable and maintainable—without adding infrastructure complexity before it is needed.

**[Explore IXP at ixp.cool](https://ixp.cool/)** · **[Public website source](https://github.com/jordaninjohnson/ixp.cool)** · **[GitHub organization](https://github.com/ixp-tech)**

> **Development status — November 2026:** A local inventory and draft-content prototype exists; the `v0.3` admin milestone is underway. The application code remains private, no open-source license has been published, and there is no downloadable release or commercial product.

## The problem

Digital signage demos show content appearing on a display. Real installations create different questions: Where is that screen? Who maintains it? What changed? Is the configuration still current? Can someone else troubleshoot it when the original installer is unavailable?

IXP's long-term goal is to connect inventory, content, playback, and operational health in one understandable system. **Today, the working prototype addresses only a subset: organized inventory, draft metadata and reporting.**

## What is working locally

| Capability | Current scope |
| --- | --- |
| **Data layer** | PostgreSQL 17, SQL migrations, fictional seed records, ownership constraints and executable contracts |
| **REST service** | FastAPI resource creation, browsing, logical-screen status editing and paginated inventory reporting |
| **Admin workspace** | React/TypeScript creation and browsing of organization → building → location → screen, with status-only screen editing |
| **Content foundation** | Organization-scoped creation and browsing of *draft metadata*—not files or playable media |
| **Exports and verification** | Local CSV/JSON inventory exports plus CI checks covering API, database, client and browser workflows |

The application uses a **single PostgreSQL database and FastAPI backend**. The local admin provides a human-facing interface to those records. Organization scoping is enforced in SQL, but **it does not substitute for caller authentication**.

## What is not available yet

- Authentication, authorization and role-based access.
- Physical player provisioning, playback or confirmed device health.
- Media upload, playlists, scheduling execution or offline caching.
- Production-ready deployment, monitoring, backups, recovery, customer hosting or support.
- A public application repository, open-source license, packaged release or customer pilot.

**Do not use the current prototype with real inventories or publish its API on a network.** Development uses localhost and fictional records only.

## Engineering roadmap

| Milestone | Direction | State |
| --- | --- | --- |
| v0.1 | Relational data foundation | Implemented in development; no tagged public release |
| v0.2 | FastAPI REST foundation | Implemented in development; package `0.2.0.dev0`, not publicly released |
| **v0.3** | Browser administration | **In progress**; inventory, reports and draft metadata exist |
| v0.4 | Authentication and RBAC | Planned |
| v0.5 | Browser-based display player | Planned |
| v0.6 | Scheduling and targeting | Planned |
| v0.7–v0.8 | Deployment, logging, monitoring and recovery | Planned |
| v0.9 | Real-world pilot | Planned |
| v1.0 | Stable community release | Planned |

Milestones are engineering targets, **not release dates or delivery commitments**. The team will prioritize verified workflows, maintainable code, documentation and safe operational boundaries over feature-count marketing.

## Who this is for

We want to learn from facilities operators, AV installers, IT administrators, property teams, developers and designers who work with information in shared physical spaces. Their experience with real-world constraints will inform later player, deployment, and support decisions.

IXP may eventually have an open-source application and optional commercial services. Both are **plans**, not offerings today. Licensing and a contribution process must be established before public application code is released.

## Follow the project

The safest public places to follow IXP today are [ixp.cool](https://ixp.cool/) and the [public site repository](https://github.com/jordaninjohnson/ixp.cool). You can also visit the [IXP GitHub organization](https://github.com/ixp-tech). Avoid references to speculative repositories, player installers or community channels that have not been created.

---

*Last reviewed: November 2026. Current capability claims are based on the private application's merged development code and test evidence, not deployed customer use.*
