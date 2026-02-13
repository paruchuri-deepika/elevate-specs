# Static App Constitution

## Core Principles

### I. Static Content Only
All application assets (HTML, CSS, JS, images, etc.) are served as static files. No server-side code or dynamic backend is permitted.

### II. Simplicity
The app must be as simple as possible. Avoid unnecessary dependencies, frameworks, or build steps unless required for static delivery.

### III. Portability
The app must run on any standard web server or CDN without modification. No environment-specific configuration is allowed.

### IV. Accessibility & Responsiveness
The app must be usable on both desktop and mobile devices, and follow basic accessibility best practices (semantic HTML, alt text, etc.).

### V. Version Control
All source code and assets must be tracked in version control (e.g., git).

## Additional Constraints

- No runtime dependencies on a backend or database.
- All configuration must be static (e.g., JSON, YAML, or environment variables at build time only).
- Must include a README with setup and deployment instructions.

## Development Workflow

- All changes must be committed via pull requests with code review.
- Automated checks (if any) must pass before merging.
- Deployment must be automated or documented for reproducibility.
<!-- Example: Code review requirements, testing gates, deployment approval process, etc. -->

## Governance
<!-- Example: Constitution supersedes all other practices; Amendments require documentation, approval, migration plan -->

[GOVERNANCE_RULES]
<!-- Example: All PRs/reviews must verify compliance; Complexity must be justified; Use [GUIDANCE_FILE] for runtime development guidance -->

**Version**: [CONSTITUTION_VERSION] | **Ratified**: [RATIFICATION_DATE] | **Last Amended**: [LAST_AMENDED_DATE]
<!-- Example: Version: 2.1.1 | Ratified: 2025-06-13 | Last Amended: 2025-07-16 -->
