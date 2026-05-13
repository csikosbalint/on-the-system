# platform

This directory contains infrastructure-as-code and platform configuration.

## Contents

- **Infrastructure definitions** – cloud resources declared with IaC tools (e.g. Terraform, Pulumi, CDK)
- **Kubernetes manifests** – Helm charts, Kustomize overlays, and raw manifests
- **Observability** – logging, metrics, and alerting configuration
- **Networking & security** – ingress rules, TLS certificates, and RBAC policies

## Environments

| Environment | Purpose |
|-------------|---------|
| `dev` | Local or shared development sandbox |
| `staging` | Pre-production validation environment |
| `production` | Live customer-facing environment |

## Conventions

- All infrastructure changes go through code review before being applied.
- Use remote state backends with locking to prevent concurrent modifications.
- Tag all cloud resources with `env`, `team`, and `service` labels.
- Document runbooks for common operational tasks in this directory.
