# Contributing

Contributions are welcome. Please open an issue first to discuss proposed changes.

## Development

All Go repositories use Go 1.26+ and follow conventional commits (`feat:`, `fix:`, `refactor:`, `docs:`, `test:`, `chore:`).

### Local multi-repo development

Use `go.work` at the workspace root for cross-repo development:

```bash
go work init
go work use ./cli-wizard-core ./vmware-vm-bootstrap ./...
```

### Before submitting

```bash
go build ./...
go test ./...
go vet ./...
```

## Reporting issues

Open an issue in the relevant repository. If unsure which repo, open it in [kubernetes-orchestrator](https://github.com/infrakit-io/kubernetes-orchestrator/issues).
