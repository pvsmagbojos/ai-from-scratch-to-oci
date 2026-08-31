# OCI Session Prompt

```text
Use the AI Tutor master prompt and repository standards.

Document material steps and verification in the learning log. Record any material errors/issues, investigation, resolution/workaround, and verification in `docs/progress/issues-and-resolutions.md` using the canonical issue format.

Active OCI roadmap item:
[PASTE PHASE / SECTION / ITEM]

Before teaching or implementing OCI-specific behavior, verify the current official Oracle Cloud Infrastructure documentation. Confirm relevant service names, availability, regions, SDK/API behavior, IAM requirements, quotas/limits, networking requirements, model/tool availability, and any deprecations that materially affect the item.

Separate the underlying AI/cloud concept from OCI's current product implementation. Teach the concept first unless this item is specifically an OCI operational task.

Use least privilege and safe credential handling. Never put credentials, API keys, private keys, auth tokens, or tenancy-specific secrets into committed files.

Add the official Oracle references actually used to the active `references.md`, including access date for mutable product documentation.

If the current OCI product surface conflicts with the roadmap, do not silently work around the roadmap. Identify the change and update the existing roadmap/documentation once the new course decision is accepted.
```
