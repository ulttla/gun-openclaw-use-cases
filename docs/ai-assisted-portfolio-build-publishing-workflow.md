# AI-Assisted Portfolio Build and Publishing Workflow

## Purpose

This case study connects portfolio content, static-site source, Git history, hosting, and live verification into one supervised delivery workflow.

## Workflow

1. Compare the live site, local source, and public supporting repositories before editing.
2. Separate stable facts from beta, unreleased, or unverified runtime behavior.
3. Update source and deploy artifacts together.
4. Run source-to-build parity, link, public-marker, and private-path checks.
5. Commit and push the reviewed public changes.
6. Verify the live domain directly; treat a hosting dashboard status as advisory evidence.
7. Use a controlled fallback only when the preferred deploy path is stale, then repeat live checks.

## Ownership and safety

AI assists with research, editing, review, and smoke tests. The human operator owns public claims, credentials, publishing approval, deployment decisions, and rollback.

This public note omits hosting account details, private paths, credentials, raw browser state, and control-panel implementation details.

## Evidence

A successful closeout records:

- reviewed files and Git commit;
- source/build parity;
- public link and marker checks;
- live-domain smoke and normalized hash comparison;
- any fallback used and the final rollback point.

## Related notes

- [AI Engineering Control Plane](ai-assisted-engineering-control-plane.md)
- [Long Work Window Playbook](long-work-window-playbook.md)
- [Public Release Evidence Pattern](public-release-evidence.md)
- [Communicating AI-Assisted Work](communicating-ai-assisted-work.md)
