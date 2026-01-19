# Kubernetes GitOps Repository

## Purpose
This repository is the single source of truth for Kubernetes desired state.
All application and platform changes are declared here and reconciled into the cluster
using GitOps principles.

## Principles
- Git is the source of truth
- No direct kubectl apply for applications
- Desired state is continuously reconciled
- Cluster credentials never leave the cluster

## Structure
- apps/      : Application definitions (what runs)
- clusters/  : Environment bindings (where it runs)
- platform/  : Platform services (Argo CD, etc.)

## Deployment Model
Pull-based GitOps using Argo CD.
