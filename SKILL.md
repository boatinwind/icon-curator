---
name: icon-curator
description: Select or integrate one best-fitting UI icon when the user explicitly asks to provide, choose, replace, or standardize interface icons. Do not use for general frontend work, logos, app icons, illustrations, presentations, or document graphics.
---

# Icon Curator

Choose one icon, not a gallery. Prefer semantic accuracy and the target project's Existing Icon System over novelty. This is a global personal skill, but automatic use applies only when the user explicitly asks for UI icons.

## Authority

Infer the permitted outcome from the request:

- **Selection only:** recommend, select, inspect, compare, or “看看/挑选/推荐”. Return one Verified Icon and do not edit files.
- **Integration:** add, replace, use, integrate, or “添加/替换/使用/接入”. Select one icon and make only the necessary project changes.
- **Wider change:** standardize, migrate, or unify. Touch only the explicitly named surface.

Automatic invocation never grants write authority. Brand Icons require an explicit brand-icon request and current brand-rule verification.

## Supported Surfaces

V1 supports code-based web, desktop, and mobile interfaces.

For Figma-only work, return the selected asset identity and export specification only. Do not operate Figma or imply file edits.

Logos, app icons, illustrations, presentations, and document graphics are separate tasks.

## Workflow

1. Inspect the target component or design surface, nearby UI, manifests, icon imports, lockfile, and relevant design tokens. Do not ask the user for facts available in the project.
2. Determine the interface role, target size, visual language, required states, target framework, and License State. If the stack is unknown, default to a static, general-purpose, free route rather than a framework-specific motion library.
3. Read [selection-rubric.md](references/selection-rubric.md) and apply its gates before ranking.
4. Preserve the Existing Icon System when it can express the meaning. Otherwise read [source-matrix.md](references/source-matrix.md) and search the smallest useful route, normally one or two sources.
5. Confirm the exact icon identity and usable import, component, registry, or asset path from an installed package or authoritative vendor source. Never guess an export name.
6. Select exactly one icon. If materially different meanings remain plausible, ask one focused semantic question instead of guessing.
7. Before Adoption, read [licensing.md](references/licensing.md). Check the license shipped with the adopted open-source version or the current official proprietary terms. For an open-source static route such as Disarto, an exact official package export or exact official repository asset path resolved from the current manifest is acceptable.
8. For Integration, prefer an existing named import, then an official framework component or registry, then an official SVG, then a sanitized inline SVG.
9. Verify the import, relevant lint/type/build checks, accessibility, attribution, and rendered states when the UI can run. Visual checks should cover the relevant default, hover, disabled, dark, and reduced-motion states that exist.

## Integration Constraints

- Do not add a dependency for one static icon. Add one only when there is no icon system, the existing system lacks the meaning, the user explicitly requests the library or motion capability, or multiple interfaces will reuse it.
- For a static open-source fallback such as Disarto, use only an exact npm/package export or an exact official repository asset path verified from current source metadata.
- Follow the existing lockfile and compatible versions. Do not upgrade unrelated packages, switch major versions, or migrate the surrounding icon system.
- Modify only the named target and necessary imports, props, styles, tests, and local supporting code.
- Remove obsolete local imports and variables. Do not remove shared components, shared assets, or an old icon dependency without an explicit cleanup request and proof that it is unused.
- Never install or configure vendor MCP servers, vendor Skills, accounts, credentials, or paid access as part of an icon request.
- Never scrape, mirror, bulk-download, or automatically export an icon catalog.
- Refresh third-party manifest, package, and license metadata only when preparing Adoption. Do not maintain an auto-synced local catalog mirror.

For raw SVG, reject or remove scripts, event handlers, external resources, unsafe URLs, unsuitable fixed colors or dimensions, invalid `viewBox` values, and colliding IDs used by masks, gradients, or clip paths. Do not reverse-engineer an SVG from page DOM when the publisher does not provide it as an asset.

## Accessibility and Motion

- Hide decorative icons from assistive technology.
- Put the accessible name on an icon-only control, not only inside its SVG.
- Provide readable text for an icon carrying independent information.
- Use static icons by default.
- Use motion only for interaction feedback, operation results, state transitions, direction, loading, or live activity.
- Support reduced-motion preferences. Reserve perpetual animation for loading or genuinely live state.

## Failure and Completion

If the preferred source is unavailable, use the next licensed source that preserves the semantic, visual, and stack constraints. Disclose the fallback.

If integration cannot be repaired within scope, undo only changes made during the current icon task. Preserve all pre-existing work and never reset the working tree.

Report one completion class:

- **Visually Verified Integration:** code checks passed and relevant rendered states were inspected.
- **Code-Complete Integration:** code checks passed, but the running interface could not be inspected.

For Selection, report the single icon, exact source identity, why it fits, and a direct official page or reliable preview when available. For Integration, lead with the completed result, verification, completion class, and any fallback or license obligation. Do not create a routine selection report.
