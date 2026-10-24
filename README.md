# 🚀 Helm Zero to Hero

A hands-on learning repository for **Helm and Kubernetes**, covering basic concepts, commands, chart structure, templates, and practical deployments.

## 📚 What is Helm?

Helm is a package manager for Kubernetes applications. It helps us install, configure, upgrade, roll back, and uninstall applications using reusable Helm Charts.

## 🎯 Learning Objectives

- Understand Helm and why it is used
- Learn Helm repositories, charts, and releases
- Understand `Chart.yaml` and `values.yaml`
- Create Kubernetes resources using Helm templates
- Install and upgrade applications with Helm
- Practice deploying applications such as NGINX and Argo CD

## 📂 Repository Structure

```text
helm-zero-to-hero/
├── README.md
├── notes/
│   └── helm-quick-notes.md
└── projects/
    └── payments/
        ├── Chart.yaml
        ├── values.yaml
        └── templates/
            └── deployment.yaml
```

## 🧠 Important Helm Concepts

| Concept | Meaning |
|---|---|
| Repository | Stores and distributes Helm Charts |
| Chart | Package containing Kubernetes templates and configuration |
| Release | An installed instance of a Chart |
| `Chart.yaml` | Contains chart metadata |
| `values.yaml` | Stores configurable values |
| `templates/` | Contains Kubernetes resource templates |

## ⚙️ Basic Helm Commands

```bash
# Check Helm version
helm version

# Add a Helm repository
helm repo add argo https://argoproj.github.io/argo-helm

# Refresh repository information
helm repo update

# Search for charts
helm search repo argo-cd

# Preview generated Kubernetes YAML
helm template payments ./payments

# Install a chart
helm install payments ./payments

# List releases
helm list

# Upgrade a release
helm upgrade payments ./payments

# Uninstall a release
helm uninstall payments
```

## 🛠️ Hands-on Project: Payments Application

This project demonstrates how to:

1. Create a Helm chart.
2. Define configuration in `values.yaml`.
3. Use `{{ .Values... }}` in Kubernetes templates.
4. Render Kubernetes YAML using `helm template`.
5. Deploy and inspect the application.

## 📈 Learning Progress

- [x] Helm fundamentals
- [x] Repository, Chart, and Release
- [x] Basic Helm templates and values
- [ ] Services and application networking
- [ ] Chart upgrades and rollbacks
- [ ] Argo CD installation using Helm
- [ ] Prometheus and Grafana deployment using Helm

## 🎯 Goal

Build practical Helm skills for Kubernetes deployments and DevOps workflows.

**Learning by doing — one chart at a time.**
