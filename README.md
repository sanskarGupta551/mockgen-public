# **MockGen — Self-Hosted Mock Backend Generator**

Turn a simple JSON schema into a fully functional mock backend with real CRUD APIs, deterministic fake data, and OpenAPI documentation.

**Self-hosted. Deterministic. Privacy-first. No vendor lock-in.**

---

## **🔥 The Problem**

Developers lose countless hours waiting for backend APIs or hand-writing mock endpoints.
Common issues:

* Mock APIs drift from real APIs
* SaaS mocking tools lock you into their platform
* Example responses lack state or persistence
* Datasets change unpredictably
* Internal teams can’t host mocks inside their own environment

MockGen solves this entire category of pain **with one input**: a JSON schema.

---

## **🚀 The MockGen Solution**

MockGen takes a schema like this:

```json
{
  "entities": [
    {
      "name": "User",
      "path": "users",
      "records": 50,
      "fields": [
        { "name": "id", "type": "uuid", "primary": true },
        { "name": "name", "type": "string", "faker": "name.fullName" },
        { "name": "email", "type": "string", "faker": "internet.email" },
        { "name": "age", "type": "int", "min": 18, "max": 65 },
        { "name": "created_at", "type": "datetime" }
      ]
    }
  ]
}
```

…and generates a **complete mock backend** featuring:

* `/users` GET → paginated list
* `/users/{id}` GET → detail
* POST / PUT / DELETE endpoints
* Deterministic dataset of 50 records
* Persistent storage (JSON or SQLite)
* `/openapi.json` and `/docs` (Swagger/Redoc)

All **self-hosted**, reproducible, and ready in seconds.

---

## **✨ Why MockGen Stands Out**

### **1. Self-Hosted**

Runs locally, in CI, or in your VPC. No external dependency.

### **2. Deterministic Fake Data**

Seeded faker output ensures **stable datasets across runs**.

### **3. Real Stateful CRUD**

Not static examples — actual create, update, delete, list, filter, and detail operations.

### **4. Schema-First Development**

Define your mock backend declaratively. Zero manual endpoint wiring.

### **5. Instant Developer Experience**

One command → a complete mock API with documentation.

### **6. Built for Automation**

Perfect for Git, CI, ephemeral environments, and n8n workflows.

---

## **🎥 Demo Video**

*A 30–60 second demo should be placed here.*
This dramatically improves conversions and asset sale velocity.

---

## **🧠 High-Level Architecture**

MockGen includes:

* **Schema Ingestor** → validates JSON DSL
* **Data Generator** → creates deterministic datasets
* **CRUD Engine** → auto-generates REST endpoints
* **Storage Engine** → JSON or SQLite persistence
* **OpenAPI Generator** → builds route documentation
* **Admin API** → regeneration + docs access
* **CLI** → project generation & serving
* **Docker Runtime** → identical behavior across environments

> Only the high-level architecture is shared publicly.
> All internal implementation is included **only in the private licensed repository**.

---

## **📚 Public Documentation Included in This Repo**

This repository includes **high-level, non-proprietary documentation**:

* Product overview
* Schema DSL format
* Example schema inputs
* Example outputs
* Demo references
* Licensing and acquisition information

Full technical documentation is provided only to license holders.

---

## **🏷️ What You Get When You Purchase MockGen**

Licensed buyers receive:

* Full private repository
* Complete source code
* Internal architecture documentation
* Schema DSL documentation (full version)
* CLI implementation
* Backend engine (ingestor, generator, CRUD engine, storage engine)
* Dockerfile + docker-compose
* Example schemas + demo package
* Test suite (unit + integration)
* n8n automation workflows
* Handover notes + pitch deck
* Version history + changelog

Everything is packaged as a **clean, professional, acquirable micro-product asset**.

---

## **🚫 What This Public Repo *Does Not* Include**

To protect the commercial IP, this public repo excludes:

* Source code
* Internal architecture diagrams
* CRUD engine implementation
* Data generator logic
* CLI code
* Storage engine
* OpenAPI generator internals
* Deployment scripts
* Dockerfiles
* Test suite
* n8n workflows

These are included only in the private licensed version of MockGen.

---

## **🧩 Use Cases**

* **Frontend Development:** Build UI against a realistic API, before backend exists.
* **QA & Testing:** Generate stable datasets for automation testing.
* **Agencies:** Spin up isolated mock environments per project.
* **DevOps:** Run mock microservices inside CI and staging.
* **Education & Prototyping:** Demonstrate backend flows instantly.

---

## **💼 Licensing & Acquisition Options**

MockGen is a **commercial, closed-source, self-hosted developer product**.

You may choose:

### **1. Commercial License**

Use MockGen internally within your organization.

### **2. Full Asset Acquisition**

Acquire complete ownership of the MockGen codebase and IP.

For licensing, demos, or acquisition inquiries:

```
[Your Name / Email / Website]
```

---

## **📄 License**

All content in **this public repository** is provided under the **MIT License**.

The actual product codebase is licensed separately under the
**MockGen Commercial License (Proprietary)**
and is *not included* here.

---

## **🎯 Call to Action**

If you want mock backends that are:

* predictable
* self-hosted
* deterministic
* schema-driven
* and ready in seconds

→ **Request the MockGen demo & licensing details:**

```
[guptasanskar551@gmail.com]
```

---

