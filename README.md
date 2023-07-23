# Helm Multiple Charts

This repository contains a Helm chart that can be used to deploy multiple charts at once.

## Usage

```bash
helm dependency update ingress-controller-aws
helm dependency update ingress-controller-gcp
helm dependency update
helm template -n all ingress-controller . -f values.yaml
```
