# Design principles for AI agents

These principles guide future interface work, not a request to redesign existing products. Explicit user instructions take precedence; retain applicable repository and more specific local guidance.

## Start with purpose and context
Inspect the existing interface, design assets, components and workflows before proposing changes. Identify the users, their task, environment, device and information needs. Use the established visual language and interaction conventions unless the task explicitly requires a change. Each product should have an identity suited to its purpose; shared components do not require identical application shells.

## Avoid default AI/SaaS patterns
Do not automatically use card grids, oversized rounded panels, pastel gradients, generic dashboard layouts, decorative badges or excessive whitespace. None is forbidden: choose elements for a clear functional reason. Choose typography, color, spacing and hierarchy from the product context, not from a fashionable template. Keep copy specific and useful; avoid filler, invented metrics and decorative elements that compete with the task.

## Work and accessibility first
Choose information density and layouts for actual tasks: maps and data tables need usable workspace, field tools need clear touch targets and outdoor readability, and educational screens need legible content and feedback. Preserve domain conventions, units, precision and established workflows. Support keyboard operation, visible focus, semantic labels, sufficient contrast, responsive layouts and relevant states including errors, loading and empty results. Do not rely on color alone. Respect reduced-motion preferences.

## Change and verification
Limit changes to the requested scope. Preserve behavior, data, calculations, exports and accessibility; do not initiate a broad redesign. In spreadsheets preserve workbook formatting, controls, formulas and macros unless explicitly instructed otherwise. For interface changes inspect representative states and viewport sizes, check keyboard and touch interactions as appropriate, and report what was actually verified and any limitations. For shared components consider all consuming products before changing their appearance or behavior.
