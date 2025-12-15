# T12 Falco Helm Chart

This Helm chart installs:
- Falco (runtime security)
- Falcosidekick (event forwarding)
- T12 Heartbeat CronJob (liveness signal)

## Prerequisites
- Kubernetes 1.24+
- Helm 3.x

## Installation

```bash
git clone https://github.com/t12cloud/t12-falco-helm.git
cd t12-falco-helm

helm dependency update
helm install falco . -n falco --create-namespace

