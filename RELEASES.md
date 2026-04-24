# Releases

This repository is a public showcase for `YoYoung Shorts 优扬短剧`.

Release assets, when published here, are not open-source source-code distributions. They are limited closed-source trial/runtime packages intended to let users try the public-facing local shell while the private backend and commercial implementation remain closed.

## v0.1.1-docker-thin-public-clean

Package: `docker-local-package-thin-bundle.zip`

SHA256:

```text
9DB915D3B2105C1B5CB3C3DABB442517059F8CE7FD455EF1082B9C7C614E6A31
```

### What This Package Contains

- Docker/DACKER thin local runtime shell.
- Static frontend runtime assets required for the local package experience.
- Local reverse-proxy/runtime configuration needed to connect the shell to the official service flow.
- Public package metadata and startup instructions.

### What This Package Does Not Contain

- Private backend source code.
- Cloud deployment code.
- Model-provider routing implementation.
- Proxy/fallback strategy implementation.
- API keys, cloud secrets, SSH keys, database files, or private environment files.
- Admin/license backend implementation.
- Commercial orchestration or billing implementation.

### Verification Summary

Before publication, this package was checked for:

- No backend source package directories included.
- No `.env`, database, private key, SSH key, or API-key files included.
- No hardcoded public backend IP URLs in the packaged frontend output.
- Docker startup smoke check passed locally.
- Backend health route proxy check passed locally.
- Admin page static access check passed locally.

This verification does not convert the package into an open-source distribution. The package remains governed by `LICENSE-NOTICE.md` and any release-specific notes.
