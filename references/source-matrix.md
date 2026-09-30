# Source Matrix

Inspect the project's existing library first. These routes apply only when it does not control the choice.

| Need | Preferred source | Access and boundary |
| --- | --- | --- |
| General static UI | Hugeicons Free | Prefer installed packages or the official Skill/MCP; free stroke-rounded is the default route |
| General static UI fallback | Disarto Icons | MIT packages plus a machine-readable manifest; prefer exact exports from `disarto-icons`, `disarto-icons-react`, or `disarto-icons-static`, or an exact official GitHub/raw SVG addressed through the manifest; exclude `Brands` by default and never scrape, mirror, or bulk-download the catalog |
| Refined or small product UI | Nucleo UI | Prefer official AI integration or packages; paid families require verified access |
| Fill, bulk, or duotone variants | Iconsax | Official MCP supports free access and optional Pro access |
| React hover motion | lucide-animated | Open-source React components; preserve Lucide visual language |
| React motion alternative | Its Hover | React/Motion components via source or shadcn registry |
| Svelte motion | moving icons | Svelte-native components and registry |
| Stroke-icon state transition | morphicons | Animation layer for two existing icons, not a primary icon catalog |
| Isometric UI visual | Isocons, then Nucleo Isometric | Browser-assisted for Isocons; Adoption requires CC BY 4.0 attribution |
| 3D or strongly decorative UI | Iconly Pro | Use only when explicitly requested and licensed; browser-assisted by default |

When the target stack is unknown, prefer Hugeicons Free, Disarto Icons, or Nucleo UI before framework-specific motion sources.

## Authoritative entry points

- Nucleo: https://nucleoapp.com/ai-integration
- Hugeicons Skill: https://hugeicons.com/docs/integrations/skill
- Hugeicons MCP: https://hugeicons.com/docs/integrations/mcp
- Iconsax MCP: https://docs.iconsax.io/mcp/ai-integration
- Disarto Icons: https://github.com/Disarto/disarto-icons
- Disarto manifest: https://github.com/Disarto/disarto-icons/blob/main/packages/static/icons.json
- Its Hover: https://www.itshover.com/icons
- lucide-animated: https://lucide-animated.com/
- moving icons: https://www.movingicons.dev/
- morphicons: https://www.morphicons.com/
- Iconly Pro: https://web.iconly.pro/
- Isocons: https://www.isocons.app/

Refresh package, manifest, and license metadata only when preparing Adoption. Do not auto-sync or locally mirror a third-party icon catalog.

Use configured official integrations when present. Do not configure them inside an icon request. For browser-assisted sources, permit targeted search, preview, comparison, and direct-page location; do not bulk collect, mirror, assume login, automatically export, or reverse-extract commercial assets.
