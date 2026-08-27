# IXP ⚡

### Open-source software for digital displays and real-world operations.

IXP is an early-stage open-source project built around a simple idea:

> **Digital signage shouldn't become a mysterious black box the moment it gets installed.**

We're building a platform for managing displays, devices, content, schedules, and building communication — with as much attention paid to **deployment, reliability, monitoring, and support** as the UI on the screen.

🌐 **[ixp.cool](https://ixp.cool)**

---

## 👋 Welcome

If you're here early, you found us at a fun time.

IXP isn't a giant finished platform pretending to need contributors.

We're building it **from the foundation up, in public**.

There are still architecture decisions to make.

There are still rough edges.

There are still things we haven't thought of.

That's kind of the point.

---

## 🧩 What is IXP?

At its core, IXP is being designed to understand things like:

```text
Organization
   ↓
Building
   ↓
Location
   ↓
Screen
   ↓
Device
```

and connect them with:

```text
Users
Roles
Content
Playlists
Schedules
Events
Health Checks
```

Over time, that foundation becomes a complete system for managing digital communication across real physical spaces.

Not just:

> "put an image on a TV"

but:

> "know what should be playing, where, when, on which device — and whether that device is actually healthy."

---

## 🚧 Current build

### `v0.1` — Data Foundation

We're intentionally beginning with the boring stuff.

And we mean that as a compliment.

Before dashboards, animations, players, cloud services, or custom hardware, we need a relational model that doesn't fall apart later.

Current work:

* PostgreSQL
* schema architecture
* primary and foreign keys
* constraints
* organizations
* buildings
* locations
* screens
* devices
* users and roles
* content
* playlists
* schedules
* device health events
* seed data
* SQL
* tests
* documentation
* reproducible setup

---

## 🗺️ Where we're headed

```text
v0.1  Data Foundation
        ↓
v0.2  REST API
        ↓
v0.3  Admin Interface
        ↓
v0.4  Authentication + RBAC
        ↓
v0.5  Display Player
        ↓
v0.6  Scheduling
        ↓
v0.7  Linux + Docker Deployment
        ↓
v0.8  Logging + Monitoring + Recovery
        ↓
v0.9  Real-World Pilot
        ↓
v1.0  Stable Community Release
```

The roadmap is a direction, not a sacred artifact.

Real users get a vote.

---

## 🧰 The early stack

We're deliberately keeping things understandable.

```text
Database     PostgreSQL
Backend      Python + FastAPI
API          REST + JSON
Frontend     TypeScript + React
Operations   Linux + Docker
Automation   GitHub Actions
Cloud        AWS when it earns its place
Security     IAM · RBAC · OAuth/OIDC · TLS
```

### Things we are not doing just because they sound impressive

* microservices for a one-developer project
* Kubernetes before Docker becomes boring
* twelve repositories for twelve folders
* infrastructure nobody needs yet
* "enterprise architecture" diagrams that explain nothing

Complexity has to **earn its way in**.

---

## 🏢 The real-world part

IXP is interested in the messy boundary between software and actual places.

Eventually that could mean displays in:

* offices
* medical buildings
* professional buildings
* campuses
* schools
* training facilities
* apartment and leasing environments
* community spaces
* small businesses
* multi-tenant buildings

Those environments introduce problems software demos don't always show:

**networks fail.**

**devices go offline.**

**people move offices.**

**content expires.**

**someone forgets a password.**

**something gets unplugged.**

**the person maintaining the system changes jobs.**

We want IXP to be designed for that world.

---

# 🌱 You can help before you're a contributor

You don't need to arrive with a giant pull request.

Seriously.

Some of the most useful early contributions could be:

### 🐛 Find something weird

Tell us when something doesn't make sense.

### 💡 Bring a real problem

If you've managed signage, AV systems, facilities, displays, kiosks, or shared spaces, we'd love to hear what goes wrong in practice.

### 📝 Improve the words

Documentation fixes count.

Clearer instructions count.

Better examples count.

### 🧪 Break things

As releases become usable, try them somewhere we didn't.

### 🎨 Make it easier to use

Designers and UX-minded contributors are extremely welcome.

### 🔐 Ask uncomfortable security questions

Please.

### 💻 Write code

Also yes. 😎

---

## 👥 Who we'd love to meet

IXP could become an interesting meeting place for:

**developers**
**system administrators**
**designers**
**technical writers**
**security people**
**digital signage nerds**
**AV professionals**
**facilities teams**
**hardware hackers**
**students**
**curious beginners**
**operators who know exactly how technology breaks at 7:42 Monday morning**

If any of those sound like you, welcome.

---

## 🧭 How we want to build

### Useful over flashy

A boring feature that saves somebody 20 minutes every week is a good feature.

### Simple until complexity is earned

Architecture is here to solve problems, not decorate resumes.

### Operability is part of the product

Logs, monitoring, backups, upgrades, and recovery are features.

### Documentation is engineering

If only the original developer knows how it works, we're not done.

### Real-world feedback beats imaginary requirements

Deployments eventually outrank assumptions.

### Be good to people

Ask questions.

Disagree constructively.

Explain things.

Remember that everyone was new once.

---

## 🔓 Open source first

IXP is being built around an open-source core.

If the project becomes useful, the broader ecosystem may eventually include:

### IXP Community

The open-source software.

### IXP Managed

Optional hosting, monitoring, updates, backups, and support.

### IXP Hardware

Preconfigured players, kiosks, displays, enclosures, and installation options where they make deployment easier.

### IXP Professional Services

Implementation, integrations, configuration, migration, customization, training, and support.

The principle is simple:

> **The business should make the open-source software easier to adopt — not make the open-source version miserable to use.**

---

## ⚖️ Licensing

The final IXP open-source license is still being evaluated.

We want something that encourages adoption and contribution while leaving room for a sustainable project ecosystem.

Older references to a specific IXP license should be considered provisional until the project formally adopts one.

---

## 📡 Project status

```text
PROJECT       IXP
STATUS        very early
VERSION       pre-v0.1
CURRENT       Data Foundation
STACK         PostgreSQL + Python + TypeScript
MISSION       make signage infrastructure less painful
COMMUNITY     assembling...
```

---

# 👋 Come hang out

You don't need permission to be curious.

Star the organization if you want to follow the build.

Open an issue when we have something wrong.

Tell us about an annoying digital-signage problem.

Come back in a month and see what changed.

🌐 **[ixp.cool](https://ixp.cool)**
💻 **[github.com/ixp-tech](https://github.com/ixp-tech)**

---

### We're building the boring parts, the cool parts, and everything in between.

> **Make displays easier to run. Make systems easier to trust. Build it together.**
