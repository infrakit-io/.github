# infrakit-io

Go libraries and CLI tools for infrastructure automation.

## Repositories

| Repository | Description |
|------------|-------------|
| [cli-wizard-core](https://github.com/infrakit-io/cli-wizard-core) | Shared interactive CLI primitives (selectors, prompts, interrupts) |
| [vmware-content-library-core](https://github.com/infrakit-io/vmware-content-library-core) | VMware Content Library client library |
| [vmware-vm-bootstrap](https://github.com/infrakit-io/vmware-vm-bootstrap) | VM provisioning with Ubuntu autoinstall on vSphere |
| [talos-vmware-cluster-bootstrap](https://github.com/infrakit-io/talos-vmware-cluster-bootstrap) | Talos Linux cluster deployment on VMware |
| [talos-docker-bootstrap](https://github.com/infrakit-io/talos-docker-bootstrap) | Talos Linux dev clusters in Docker |
| [kubernetes-orchestrator](https://github.com/infrakit-io/kubernetes-orchestrator) | Kubernetes cluster lifecycle orchestrator |
| [repo-standards-kit](https://github.com/infrakit-io/repo-standards-kit) | Reusable CI/CD workflows, pre-commit hooks, and repo templates |

## Dependency graph

```
cli-wizard-core              (standalone)
vmware-content-library-core  (standalone)
    |
    v
vmware-vm-bootstrap          -> cli-wizard-core, vmware-content-library-core
    |
    +---> talos-docker-bootstrap
    +---> talos-vmware-cluster-bootstrap
    +---> kubernetes-orchestrator

repo-standards-kit           (standalone — governance)
```
