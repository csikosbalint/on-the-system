# on-the-system

There are two types of Entities in a process. 

Those who work `on-the-system` create the rules, boundaries, platforms, conventions, etc. They are human actors (mostly), and need to review and approve changes for product specific artefacts (same categories can be batched together in a single PR):
- workflows
- mockups
- HLAs
- NFRs
- pipeline changes
- skeletons (initial app, and its test suite)
- test suit changes
- test reports
- new epics
- new stories (with acceptance criteria)
- new NFR epics
- new NFR stories (no AC needed)
- smoke test reports

Those who work `in-the-system` must keep the rules, boundaries, conventions and use platforms as stated in this repository (see Domains below)!
- Product Owner (PO)
- Scrum Master
- Team Architect
- Test Enginner
- Lead Developer
- DevOps Engineer

## For Every `in-the-system` Entity
As an Entity, you should
- read the domains (subdomains are also available as subfirectories) here
- use your __own__ repository directory to create your product/project specific document as a PR
  Example:
  ```
  best-blog-every.com/
  └── design/
      ├── workflows/
      │   ├── use-case1.md
      │   └── ...
      └── mockups/
          ├── login.md
          ├── logout.md
          ├── use-case1.png
          └── ...
  ```

## Domains and Sub-domains
This repository is organised into domain directories, each owned by the team or discipline responsible for that area.

| Directory | Description |
|-----------|-------------|
| [`design/`](./design/README.md) | UI and UX design requirements, and interface contracts |
| [`code/`](./code/README.md) | Application source code and shared libraries |
| [`cicd/`](./cicd/README.md) | CI/CD pipeline definitions and build automation |
| [`platform/`](./platform/README.md) | Infrastructure-as-code and platform configuration |
| [`e2e/`](./e2e/README.md) | End-to-end test suites |
| [`product/`](./product/README.md) | Product roadmap, requirements, and research |
