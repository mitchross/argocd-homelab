# Overview

GitOps driven homelab using ArgoCD

# Project Structure

```
.
├── .github/                   # Github workflow & integration settings
│   └── renovate.json5         # RenovateBot configuration
├── .vscode/                   # Visual Studio Code configuration
│   ├── extensions.json        # Extension recomendations
│   └── settings.json          # Editor settings
├── docs/                      # Documentation
│   ├── faq.md                 # Frequently Asked Questions
│   └── setup.md               # Onboarding setup
├── manifest/                  # Directory ArgoCD ApplicationSet watches
│   └── <namespace>.yaml       # App of Apps manifests for each namespace
├── .gitignore                 # Ignored files list
└── README.md                  # This file
```



# Docs
* [faq](docs/faq.md)
* [setup](docs/setup.md)

# Getting Started

## Fork this repository
- Update references during setup and in `bootstrap/argocd-config.yaml` of this repository.  Work in progress to simplify.

# TODO
* Remove bootstrap specific files
* Remove hardcoded values
  * kube-system.yaml cilium configuration
  * kube-system.yaml coredns configuration
* Use 1password cli during setup
* Add 1password/externalsecrets entries into 1password

* Github pages
* List out all tech used
* Renovate updates for argovaultplugin & knative
* Update docs/setup to mention kube-system
* Investigate dex as standalone