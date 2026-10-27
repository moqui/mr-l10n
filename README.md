# mr-l10n

Language packs for mr-moqui. Spanish covers the framework, tools, webroot, example, mr-mantle, and mr-marble. mr-boss is not in this pack. Each language is a two-letter directory under `data/` and the same load type. Spanish is `data/es/` with `type="es"`.

`moqui load` and an empty-database startup load `seed`, `seed-initial`, and `install`. They do not load these files. Load Spanish with `moqui load types=es`, or add `es` to a longer type list. `types=all` includes it. A database that already has data does not pick a language up until that load runs.

## Voice

Locale `es` is neutral international Spanish: Latin American words that Spain also understands.

| English | es |
| --- | --- |
| computer | computadora |
| file | archivo |
| mobile phone | celular |
| email | correo electrónico |
| password | contraseña |
| settings | configuración |
| save | guardar |
| default | predeterminado |

Actions use the infinitive (Guardar, Cancelar). The `es` files do not use ordenador, fichero, móvil, vosotros, or voseo.

`EsRegional.xml` is a short overlay, not a second catalog:

- `es_ES`: fichero, móvil, and ajustes where the English is Settings. No label in this pass is Computer, so there is no ordenador row.
- `es_MX`: the same headwords as `es` (archivo, celular, configuración), stated on purpose so the regional file shows the choice.

These nine originals stay in `framework/data/CommonL10nData.xml` and are not repeated here: Add, Create, Delete, Description, Find, Name, Status, Type, Update.

Placeholders `${...}` and `{0}` `{1}` `{2}` `{3}` are copied unchanged. A `##` suffix stays on the key. Strings longer than 255 characters cannot be keys.

## Files

These live in `data/es/`. `EsRegional.xml` is still type `es`. Its rows use locale `es_ES` and `es_MX`.

| File | Contents |
| --- | --- |
| EsChromeAD.xml, EsChromeEL.xml, EsChromeMR.xml, EsChromeSZ.xml | Shared labels and field titles |
| EsMessagesA.xml, EsMessagesB.xml, EsMessagesC.xml | Service, screen, and framework messages |
| EsSeedEnumA.xml, EsSeedEnumB.xml | Enumeration and status text |
| EsSeedMeasure.xml | Currency and unit descriptions |
| EsGeo.xml | Country names (`Geo.geoName`) |
| EsToolsApp.xml, EsToolsSystem.xml, EsToolsLlm.xml | Tools screens |
| EsWebroot.xml | Login and shell |
| EsExample.xml | Example app |
| EsRegional.xml | `es_ES` and `es_MX` only |
| EsMantleEnumAccountA.xml, EsMantleEnumAccountB.xml, EsMantleEnumAccountC.xml | Accounting, ledger, payroll, and item-type text |
| EsMantleEnumWork.xml | Work, project, and request text |
| EsMantleEnumPartyA.xml, EsMantleEnumPartyB.xml | Party, human resources, and marketing text |
| EsMantleEnumProductA.xml, EsMantleEnumProductB.xml | Product, asset, store, and facility text |
| EsMantleEnumOrder.xml | Order, shipment, request, and ACH return text |
| EsMantleGeoA.xml, EsMantleGeoB.xml | State and province names |
| EsMantleMsgAccount.xml | Invoice, payment, and ledger messages |
| EsMantleMsgWorkA.xml, EsMantleMsgWorkB.xml | Work, inventory, and shipment messages |
| EsMantleTemplates.xml | Name and order message templates (the key stays English; the Spanish value is the template) |
| EsMarbleAccountA.xml, EsMarbleAccountB.xml | Accounting screens |
| EsMarblePartyA.xml, EsMarblePartyB.xml | Party, customer, supplier, and My Account screens |
| EsMarbleOrder.xml | Order and return screens |
| EsMarbleShipA.xml, EsMarbleShipB.xml | Shipment, facility, and warehouse screens |
| EsMarbleProductA.xml, EsMarbleProductB.xml | Catalog, asset, store, and manufacturing screens |
| EsMarbleWorkA.xml, EsMarbleWorkB.xml | Project, task, request, wiki, and the Marble menus |
| EsMarbleEmail.xml | Invoice, order, and shipment email |
| EsMarblePrintAccount.xml | Invoice, check, payment, and statement print |
| EsMarblePrintShip.xml | Shipment pick, pack, and bill of lading print |
| EsMarblePrintOther.xml | Order, production, timesheet, and payroll print |

`Geo.geoName`, enumeration and status descriptions, status transition names, and UOM description and symbol have `enable-localization="true"`, so these rows show on screen. Product feature description and abbreviation do too. `geoNameLocal` is the place's own name, not the viewer's language. Party names, product names, and GL account names are stored text and stay as entered.

## Strings left in English

`LocalizedMessage.original` holds at most 255 characters. These longer texts are not in the catalog:

- A detail for a party seen through the app's role, here a user account: a header card with the avatar, identity, classifi
- A document the user writes: the page list at the side, the rendered page with its title and version in a title row, and
- A master list beside a detail pane: countries on the side with a header find, the selected country in the main pane with
- A work breakdown as a tree (view-tree): the top-level items, each opened to its children as the tree asks the screen's f
- An app's settings index as a row of cards, one per group with a line of description and the links into its pages, then o
- Checked database ${envMap.entity_ds_database} at ${adminMap.entity_ds_host}: connect ${dbConnectSuccess ? 'successful' :
- Create and edit without leaving the list: New is a 600 px container-dialog with a single-column form-single whose submit
- Fallbacks for style-guide section 8: number cards are q-card with text-overline and text-h5 until number-card exists; th
- Fallbacks for §8: number-card size="sm" is the row of numbers inside the header q-card (render-mode); chatter
- Fallbacks for §8: the state chip is a tonal anchor-button link (Enumeration has no status, so the state is derived per r
- Flat (tertiary): icon-only links with link-type=hidden-form-link. The first uses a Material Symbols outlined name (icon=
- Multi-step creation: subscreens-panel type="wizard" is a stepper with one step per subscreen (the menu titles,
- No §8 fallbacks. The form attributes for a background submit are background-submit, background-hide-id and background-re
- One form-list of example records with views="board,list,calendar": the switch at the right above the list keep
- One operational job at a time: the current pick line with large read-only location and product, a focused scan field (En
- One record with its parts and actions: a title row with the identifier, the status flow, one primary action and a menu o
- Parameters in the URL (the form submits to this screen), number cards, two charts and a result table with exports and a
- Quota of ${quotaUserId ?? ''} (${quota?.limitFrom ?? ''}, ${quota?.period ?? ''}): ${quota?.usedTokens ?? 0} of ${quota?
- Storage: ${gitRepository.objectCount ?? '?'} objects, ${gitRepository.storedBytes != null ? Math.round(gitRepository.sto
- The Today tab of the tray panel as a normal screen: groups Overdue, Due today and Later today as captions over dense lis
- The board groups by status or by type (Group by, view-board group-fields: a move posts the field and its new value) and
- The calendar shows each example from its start to its end, colored by status, in month, week, day and list modes; in day
- The find and list screen over one record type, here Enumeration with its type through display-entity: the identifier fir
- The fixture for style changes: every field widget of section 4.5 in one form, every button role of 4.6, the label types
- The home of an app: a row of counters, the lists of my work, shortcuts and a chart, each a link into the List screen wit
- The status-bar element shows the stages of the framework's EntitySync status flow (the status is the syncStatusId parame
- Total: ${totals.totalChars ?? 0} characters, about ${totals.totalTokens ?? 0} tokens (${totals.charsPerToken ?? ''} char
- container-split (§8.2): a splitter from 1024 px whose side can be dragged from 200 px to what leaves 480 px to the main

Mantle and marble texts over 255 characters stay in English. The message key is still used; there is no `es` row for it:

- Found similar order ${nearOrder.orderId} (OrderApproveNearOrder)
- The postal-address info template (PostalAddressInfoTemplate)
- Recurring orders in the Approved status will be automatically cloned according to the schedule
- Invoices by Customer Classification, with the day/week/month selector in the title
- No past due invoices found for customer ${toPartyId} and org ${fromPartyId} with due before...
- Newer or same revision order ${orderId} found for customer
- Tried to return total more than is returnable for non-product item
- Quantity specified differs from current on hand
- Moved quantity from Asset ... to Asset ...
- Found GlAccount Org TimePeriod ...
- Set quantity on details for an invoice item, when the message names every facility
