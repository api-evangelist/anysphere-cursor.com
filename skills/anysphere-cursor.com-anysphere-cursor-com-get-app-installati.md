---
name: anysphere-cursor-com-get-app-installation
description: Retrieve details of a specific app installation for the authenticated app.
api: openapi/anysphere-cursor.com-openapi.yaml
operations:
- OriginService_ListAppInstallations
- OriginService_GetAppInstallation
generated: '2026-09-25'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/anysphere-cursor.com-openapi.yaml ; every operationId checked against the contract
---

# anysphere-cursor.com-anysphere-cursor-com-get-app-installati

Retrieve details of a specific app installation for the authenticated app.

## Steps

1. 1. `OriginService_ListAppInstallations` – no query parameters; uses Bearer token in `Authorization` header.
2. 2. `OriginService_GetAppInstallation` – path parameter `installationId` obtained from the list response; uses Bearer token in `Authorization` header.

## Rules

- Auth: Include `Authorization: Bearer <token>` header (bearerAuth).
- Idempotency: GET operations are safe and idempotent.
