# mr-l10n

Language packs for mr-moqui. Spanish and Simplified Chinese cover the framework, tools, webroot, example, mr-mantle, and mr-marble. mr-boss is not in this pack. Each language is a two-letter directory under `data/` and the same load type. Spanish is `data/es/` with `type="es"`. Simplified Chinese is `data/zh/` with `type="zh"`.

`moqui load` and an empty-database startup load `seed`, `seed-initial`, and `install`. They do not load these files. Load Spanish with `moqui load types=es`, and Simplified Chinese with `moqui load types=zh`, or add `es` or `zh` to a longer type list. `types=all` includes them. A database that already has data does not pick a language up until that load runs.

## Files

Each language's files are in `data/<lang>/`, named by prefix (`Es` or `Zh`) and area, split into `A`, `B`, … parts when
large:

| Name | Contents |
| --- | --- |
| `Chrome*` | Shared labels and field titles |
| `Messages*` | Service, screen and framework messages |
| `SeedEnum*`, `SeedMeasure`, `Geo` | Framework enumeration and status text, currency and unit descriptions, country names |
| `Tools*`, `Webroot`, `Example` | The tools screens, login and shell, the example app |
| `Mantle*` | mr-mantle enumerations, states and provinces, messages and templates |
| `Marble*` | mr-marble screens, email and print |
| `EsRegional.xml` | `es_ES` overrides (still type `es`); `es_MX` has none of its own |

`Geo.geoName`, enumeration and status descriptions, status transition names, and UOM description and symbol have `enable-localization="true"`, so these rows show on screen. Product feature description and abbreviation do too. `geoNameLocal` is the place's own name, not the viewer's language. Party names, product names, and GL account names are stored text and stay as entered.

## Writing rows

The wording rules and glossaries for each language are in [docs/Voice.md](docs/Voice.md). In short: a row is stored
only when the text differs from the English original (the omitted originals are listed in `data/<lang>/unchanged-*.txt`,
which the loader ignores); placeholders (`${...}`, `{0}`, `{n,choice,...}`) and number patterns are copied unchanged;
and the localized value is at most 255 characters (`LocalizedMessage.original` holds at most 255 too). Longer texts
stay in English; they are listed in [docs/Strings-Left-In-English.md](docs/Strings-Left-In-English.md).
