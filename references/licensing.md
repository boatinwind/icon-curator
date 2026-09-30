# Licensing

License notes route the search; they are not permanent proof. Verify current official terms before Adoption.

## License State

- `unknown`: no entitlement declared; adopt only currently verified free assets.
- `free_only`: adopt only assets whose free terms permit this product and distribution model.
- `paid_allowed_but_unverified`: paid candidates may be discussed but not adopted.
- `vendor_licensed`: paid assets from the named vendor may be adopted through already configured official access.

Never infer a subscription from login state, installed software, cached files, or discoverable environment variables. Never create, reveal, copy, store, rotate, or modify a key.

## Adoption check

Before adding an asset:

1. Identify whether the deliverable is an end product, template, theme, plugin, open-source project, component library, or product that lets end users choose icons.
2. Verify commercial-use, redistribution, seat, client-delivery, quantity, and attribution terms that apply to that deliverable.
3. Prefer the license included with the exact installed open-source package version. For proprietary sources, open the current official license page.
4. If the terms are unavailable or ambiguous, do not adopt the asset; use an allowed fallback.
5. If the requested asset is prohibited, select one semantically equivalent permitted alternative and explain the substitution.
6. Refresh source metadata only at Adoption time. Do not rely on an auto-synced local mirror when the official package or repository is easy to verify.

## Attribution

When required, update the project's existing `NOTICE`, `THIRD_PARTY_NOTICES`, or attribution file. If none exists, create `docs/icon-attributions.md`. Record attribution only after Adoption, not after browsing or Selection.

## Source cautions

These observations were checked on 2026-09-04 and must be refreshed before Adoption:

- Nucleo uses proprietary limits for project quantity, distributable products, client sharing, seats, and licensed packages. Official terms: https://nucleoapp.com/license/
- Hugeicons provides free and Pro assets; Pro packages/API access use vendor licensing and seat/token rules. Official terms: https://hugeicons.com/license-agreement
- Iconsax is proprietary and restricts loose-file redistribution; distributable digital products have additional attribution conditions. Official terms: https://docs.iconsax.io/license-and-terms/usage-manifesto
- Iconly Pro prohibits direct resale or redistribution and applies special limits to templates, themes, logos, and client delivery. Official terms: https://iconly.pro/pages/licensing-guide
- Isocons identifies its icons as CC BY 4.0; Adoption requires appropriate credit, a license link, and indication of changes. Official license: https://creativecommons.org/licenses/by/4.0/
- Disarto Icons publishes MIT terms for its artwork and packages; preserve the MIT notice in copies or substantial portions. Its official packages include `disarto-icons`, `disarto-icons-react`, and `disarto-icons-static`, and its `packages/static/icons.json` manifest can be used to resolve exact official GitHub file paths. Its `Brands` category contains third-party marks outside that grant, so those icons require separate trademark review. Verify the exact adopted package or repository version before Adoption. Official terms: https://github.com/Disarto/disarto-icons/blob/main/LICENSE and https://github.com/Disarto/disarto-icons/blob/main/TRADEMARKS.md
- Its Hover, lucide-animated, moving icons, and morphicons publish open-source licenses. Verify the license file in the exact adopted repository or package version.
