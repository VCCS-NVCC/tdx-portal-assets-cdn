# NVCC TeamDynamix Portal Assets CDN

Public CDN artifact repository for compiled NVCC TeamDynamix portal JavaScript and CSS assets.

## Important: Generated Files Only

The files in this repository are generated and published automatically from the private source repository:

```text
VCCS-NVCC/tdx-portal-assets
```

Do not manually edit compiled JavaScript, CSS, manifest files, branches, or release tags in this repository.

Source-code changes, documentation updates, and workflow changes belong in the private source repository.

## Purpose

This repository provides browser-ready assets for NVCC TeamDynamix portal pages.

Published files may include:

```text
tdx-loader.min.js
tdx-core.min.css
manifest.json
features/
overrides/
```

TeamDynamix portal pages load an exact allowlisted loader-script URL. The loader then selectively loads the required JavaScript and CSS assets.

## Repository Model

```text
Private source repository
-> reviewed source changes
-> automated build
-> generated browser-ready assets
-> this public CDN artifact repository
-> immutable tagged jsDelivr URL
-> TeamDynamix footer loader
```

## Branches and Tags

The publishing workflows will maintain:

```text
sandbox
-> current shared Sandbox integration artifacts

main
-> current production artifacts

version tags
-> immutable production release points
```

Sandbox publishing may also create build-specific tags for testing.

Do not force-update, delete, or recreate production version tags manually.

## Security Boundary

This repository intentionally contains generated deployment artifacts only.

Do not commit:

```text
source files
build tooling
GitHub Actions workflows
credentials
tokens
local environment files
internal operational documentation
```

## Licensing

No open-source license has been applied to this repository.

Public availability does not imply permission to copy, modify, redistribute, or reuse these assets. Contact NVCC before reuse.
