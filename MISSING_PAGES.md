# Missing Pages

Audit of `docs/menu.json` against files in `docs/`. Each entry below is referenced in the menu but has no corresponding `.adoc` file.

Once changes to `master` are published to https://developer.enonic.com/docs/code/stable, missing pages here surface as broken navigation links.

Per `AGENTS.md`: every page in `menu.json` must have substantive content. Either create the page or remove the entry from the menu.

## Missing `.adoc` files

| Menu title | Menu `document` | Expected path |
|---|---|---|
| Deploying CMS schemas | `schemas` | `docs/schemas.adoc` |
| Examples | `examples` | `docs/examples.adoc` |
| Asset serving | `static-assets` | `docs/static-assets.adoc` |
| Admin tools | `admin-tools` | `docs/admin-tools.adoc` |
| Admin extensions | `admin-extensions` | `docs/admin-extensions.adoc` |
| ID providers | `id-providers` | `docs/id-providers.adoc` |
| Metrics | `metrics` | `docs/metrics.adoc` |

## Naming mismatch

- `docs/idprovider.adoc` exists, but the menu references `id-providers`. Either rename the file to `id-providers.adoc` or update the menu entry.

## Orphan files (exist but not in `menu.json`)

- `docs/sites/component-api.adoc`
- `docs/sites/site-engine.adoc`
- `docs/webapps/webapp-engine.adoc`

These should either be added to the menu or removed if obsolete.
