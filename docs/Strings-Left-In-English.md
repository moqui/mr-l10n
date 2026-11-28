# Strings left in English

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
- Queries run with your dataset permissions and row filters. Search syntax: field:value, AND, OR, NOT, quoted text, term~
- Quota of ${quotaUserId ?? ''} (${quota?.limitFrom ?? ''}, ${quota?.period ?? ''}): ${quota?.usedTokens ?? 0} of ${quota?
- Search traces by service, span name (* matches any text), status, duration in milliseconds and user, or with a query on
- Storage: ${gitRepository.objectCount ?? '?'} objects, ${gitRepository.storedBytes != null ? Math.round(gitRepository.sto
- The Today tab of the tray panel as a normal screen: groups Overdue, Due today and Later today as captions over dense lis
- The board groups by status or by type (Group by, view-board group-fields: a move posts the field and its new value) and
- The calendar shows each example from its start to its end, colored by status, in month, week, day and list modes; in day
- The find and list screen over one record type, here Enumeration with its type through display-entity: the identifier fir
- The fixture for style changes: every field widget of section 4.5 in one form, every button role of 4.6, the label types
- The home of an app: a row of counters, the lists of my work, shortcuts and a chart, each a link into the List screen wit
- The self-signed certificate this server made (${file}) answers only clients that send no name, such as a health check by
- The status-bar element shows the stages of the framework's EntitySync status flow (the status is the syncStatusId parame
- Total: ${totals.totalChars ?? 0} characters, about ${totals.totalTokens ?? 0} tokens (${totals.charsPerToken ?? ''} char
- container-split (§8.2): a splitter from 1024 px whose side can be dragged from 200 px to what leaves 480 px to the main
- Microsoft asks for an app password for mail apps. Turn on two-step verification, then make an app password (Security, 
- On-disk values come from the merged conf (MoquiDefaultConf, the components' MoquiConf, the runtime conf) and moqui_log
- Outside phones register to the edge node's registrar, which asks this node to check each password, so they cannot regi
- Passthrough: the local node ends TLS with its own certificate, and this edge node sees no content; while its link is d
- Scrape targets are Prometheus-text endpoints read into otel_metrics. Synthetic checks are HTTP requests, each recorded
- The sync maps the server's folders by their kind (and INBOX); choose here which folder is your Sent, Drafts, Archive, 
- This node takes no links, so no local nodes pair with it. An edge node runs with node_role set to front_edge (conf/edge/MoquiEdgeConf.xml), and a full server that also takes local nodes' links with node_role set to all-in-one (conf/all-in-one/MoquiAllInOneConf.xml). To pair this node with an edge node, use Edge Node.
- With a token stored, fetch, pull and push on that root use it in place of the server's own credentials: a user's own t
- You need your email address and its password. Gmail and Outlook.com sign in with Google or Microsoft where this server
- Your contacts are the people your address book knows, when this system has one. People inside the organization are the

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

Commons and Projects texts over 255 characters stay in English. The message key is still used; there is no `es` or `zh` row for it:

- Your phone and desktop apps read and change your calendars, tasks, contacts and files here: the calendar, contacts and files apps
- Settings, Calendar (or Contacts), Accounts, Add Account, Other: Add CalDAV Account for calendars and reminders, Add CardDAV Account
- Install DAVx⁵ (from Google Play or F-Droid), add an account with Login with URL and user name: the URL ${davUrl}
- GNOME Online Accounts and KDE accounts take the CalDAV and CardDAV address ${davUrl}. A file manager opens davs:// with the WebDAV address
- Mentions, assignments, approvals and reminders come to the Notifications inbox, which the header counts; record updates and system messages
- A phone or a contacts app logged in with your username ${syncAddresses.username} and an app password (Settings, Sync) finds these books
- Utilization is the hours logged over capacity; billable utilization the billable hours over capacity. Capacity is the working hours less holidays
- Cost is the hours at the workers' rates plus expenses; billable value is the billable hours at the client rates plus billable expenses
- Each row is its subtree's totals, cancelled items left out; days are the hours over the hours a day given. Act/est is actual over estimated
- A CSV file with a header line and a row per entry: date (yyyy-MM-dd), person (email or user name), work item or project key, hours
- Assignees and reporters are matched by user name, email or full name; one not found is left unassigned and named in the preview
- The estimate is kept as a file of the project's Estimate milestone, and its approval is asked of the client's manager (else the client)
- The branch-protection summary on a repository's settings (force push, delete, merge requests, approvals, checks, methods, pushes)

Products, Accounting, Warehouse, Manufacturing, Purchasing, and Customer Service texts over 255 characters stay in English. The message key is still used; there is no `es` or `zh` row for it:

Accounting:

- Link earlier bills to their orders and receipts from the billing links and receipts they already have. A
- Post ${totalText} over ${preview.allocationRows.length} receipts? The stock on hand takes its share in its
- ${bill.referenceNumber ? 'Supplier reference ' + bill.referenceNumber + ' · ' : ''}${ bill.invoiceDateText
- ${current.stateText == 'Default' ? 'No row yet: the default applies, overhead at each work center overhead
- ${testResult ? testResult.matchedCount + ' open lines match; ' + testResult.applyCount + ' would be
- ${rejectedImport.rejectedCount} rows of statement import ${ rejectedImport.statementImportId} were
- A CSV with the headers direction (receivable or payable), partyId, documentNumber, documentDate and dueDate
- The chart and conventions the books start from, and the day they open. An organization that has its own
- Activation posts the opening balances once, on the opening day: the receivable and payable balances against

Warehouse:

- ${[inspection.organizationName + ', ' + inspection.facilityName, inspection.productName +
- Result: ${inspection.resultText || 'not submitted'}${inspection.resultEnumId ? ', ' +
- ${[(returnShipment.supplierReturn ? 'to ' : 'from ') + returnShipment.partyName,
- ${['Shipment ' + line.shipmentId, line.bin != null ? 'bin ' + line.bin : '', line.containerId ? 'into ' +
- ${packedCount} packed in ${packages.length} package${packages.length == 1 ? '' : 's'}${leftCount > 0 ? '; '
- Takes ${contentsText} back off the shipment; the stock stays where it is, for another pack or a put back. A
- ${[container.typeText, container.serialNumber ? 'Serial ' + container.serialNumber : '',
- ${[selectedAsset.identityText, 'at ' + (selectedAsset.placeText || 'no location'),
- From ${sheet.transfer.originName} to ${sheet.transfer.destinationName} · owner ${sheet.transfer.ownerName}
- ${[selectedAsset.identityText, 'at ' + (selectedAsset.sourceText || 'no location'),
- ${[receipt.organizationName + ', ' + receipt.facilityName, 'from ' + receipt.supplierName,

Manufacturing:

- ${materialsFound?.vendorFacilityName ? 'At ' + materialsFound.vendorFacilityName + ', in the custody of ' +
- Plan ${planRun?.planningRunId} revision ${planRun?.revision}, calculated
- ${load.utilizationFormula} Calendar-adjusted hours are the slots over the work hours less holidays, at the
- Columns: routingName, operationName, quantityUomId; optional sequenceNum, setupTime, runTime,
- ${[selectedTemplate.centerText, selectedTemplate.methodRequiredEvidence ? 'Evidence: ' +
- Each work center's OEE: availability (run time over planned production time, planned stops excluded and
- Each work order's cost evidence: material, labor, machine, overhead and outside cost, output relief, WIP
- Each released work order's material lines, planned against net issued, with substitutes and the usage
- Columns: productId, componentProductId, quantity; optional methodCode, bomName, baseQuantity, baseUomId,
- ${[inspection.organizationName + ', ' + inspection.facilityName, inspection.productName +
- Result: ${inspection.resultText || 'not submitted'}${inspection.resultEnumId ? ', ' +
- ${['Work order ' + workEffortId + (checklist.run.workEffortName ? ' ' + checklist.run.workEffortName : ''),

Purchasing:

- ${[quote.organizationName, quote.reference ? 'their reference ' + quote.reference : '', quote.quoteDateText
- ${[rfq.organizationName, rfq.dueText ? 'respond by ' + rfq.dueText : '', rfq.facilityName ? 'deliver to ' +
- ${[rfq.organizationName, rfq.currencyUomId, rfq.respondedText, {start: '1 Review · 2 Place · 3 Close',
- ${lineRows.map((line) => line.orderItemSeqId + ' ' + line.productText + ' ' + line.quantityText +
- ${closePreview.closingRows.length ? closePreview.closingRows.map((row) => row.supplierName + ' (' +
- Link earlier bills to their orders and receipts from the billing links and receipts they already have. A
- ${['To ' + returnHeader.supplierName, 'from ' + returnHeader.organizationName, returnHeader.facilityName ?
- ${run ? ['Calculated ' + run.ageText, 'as of ' + run.planDateText, run.suggestionCount + ' suggestions',

Shared product, order, and inventory screens:

- ${previewed.policy.stateText} policy: overhead ${previewed.policy.overheadBasisText}, co-products by
- ${currentMatch.isLegacy == 'Y' ? 'Linked from existing billing evidence' : 'Applied by ' +
- ${[inspection.inspectorName ? 'Inspector ' + inspection.inspectorName : 'Not assigned', inspection.dueText
- Left to dispose: ${detail.acceptedLeft} accepted (Release) and ${ detail.rejectedLeft} rejected (the other
- ${'Sample of ' + inspection.sampleSize + ' from ' + inspection.quantity + (inspection.templateName ? ',
- ${inspection.assetId ? 'Stock ' + inspection.assetId + ' at ' + (inspection.assetLocationSeqId || 'no
- ${inspection.resultText}: ${inspection.quantityAccepted} accepted, ${ inspection.quantityRejected}
- Sample: ${template.samplePolicyText}${template.samplePolicyEnumId == 'QspFixed' ? ', ' +
- Applies to ${[template.productName || (template.productId ? template.productId : ''), template.categoryName
- ${template.stageText} inspection, sample on ${template.sampleBasisText.toLowerCase()}${
- ${[count.facilityName, count.blind ? 'Blind' : '', count.assigneeName ? 'Assigned to ' + count.assigneeName
- ${['Demand ' + selected.grossQuantity, 'stock and supply ' + selected.availableQuantity,
- The line takes the agreement's price. A release over what the item has left is refused unless it stays
- ${['From ' + rc.supplierName, rc.facilityName ? 'to ' + rc.facilityName : '', 'expected ' +
- Use this only when everything that remains arrived: every due unit is accepted, then the receipt is
- This rewrites the cost of the product's stock and reposts its receipts, issues and count variances. Use it
- Stock as of an earlier day: each asset's cost then, before the revaluations and landed costs dated after
- Credit ${settlement.creditTotalText} · Refund ${
- Credits ${settlement.receiptlessTotalText} for authorized quantity that was not received. It creates no
- ${[so.orderName, so.organizationName, so.placedText ? 'placed ' + so.placedText : 'entered ' +
- ${serviceOrder.confirmation.stored ? 'The confirmation stored ' + serviceOrder.confirmation.storedText + '
- ${serviceOrder.confirmation.stored ? serviceOrder.confirmation.description + ', stored ' +
- ${[order.customerName, order.orderName, order.entryText ? 'entered ' + order.entryText : '',
- ${[(receipt.purchase ? 'From ' : '') + receipt.supplierName, 'to ' + receipt.facilityName, 'expected ' +
- ${['to ' + outbound.toName, 'from ' + outbound.facilityName, 'scheduled ' + outbound.scheduledText,
- ${[(rh.supplierReturn ? 'to ' : 'from ') + rh.partyName, rh.facilityName ? 'at ' + rh.facilityName : '',
- Nothing more of this ${rh.supplierReturn ? 'supplier' : 'customer'} can be returned: ${rh.supplierReturn ?
- ${[(rs.supplierReturn ? 'to ' : 'from ') + rs.partyName, (rs.supplierReturn ? 'from ' : 'at ') +
- ${['from ' + transfer.originName, 'to ' + transfer.destinationName, 'ships ' + transfer.shipText, 'due ' +
- ${transfer.quantity} to send · ${transfer.sent} sent · ${transfer.inTransit} in transit ·
- ${transfer.statusId == 'ShipInput' || transfer.statusId == 'ShipScheduled' ? 'Sending stock needs the issue
- ${transfer.inTransit} sent from ${transfer.originName} and not yet received at ${transfer.destinationName}:
- ${transfer.statusId == 'ShipDelivered' ? 'Received in full.' : transfer.statusId == 'ShipShipped' ?
- ${['Held by ' + (transfer.custodianName || 'the supplier'), 'run ' + transfer.runText,
- The components stay the organization's stock at their cost in the vendor-custody facility. ${transfer.kind
- ${[outputReceipt.received + ' of ' + outputReceipt.planned + ' received on run ' + outputReceipt.runId,
- ${['to ' + rh.supplierName, 'from ' + rh.organizationName, rh.facilityName ? 'at ' + rh.facilityName : '',
- ${rh.canAuthorize || rh.statusId == 'ReturnCreated' || rh.statusId == 'ReturnRequested' ? 'Authorizing the
- ${[rh.customerName, rh.customerReference ? 'their reference ' + rh.customerReference : '', rh.orderText ?
- From ${warehouseInvoice.invoice.fromName} · ${warehouseInvoice.invoice.invoiceDateText}
- ${[pr.organizationName, pr.filedByName ? 'requested by ' + pr.filedByName : '', pr.facilityName ? 'for ' +
- ${['Stock request ' + requestId, 'for ' + stockRequest.facilityName, stockRequest.requesterName ? 'by ' +

Sales, Marketing, Commerce, Maintenance, People, Insights, Admin, and PASS (Account, the customer and supplier portals, Smithy, Forum, and Shop) had no user-visible message over 255 characters in this pass. Code fragments the extractor joined across lines are not catalog keys and are not listed here.
