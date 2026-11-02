# Transport Checkout

A responsive shipping checkout prototype built using the supplied `TRANSPORT Rate Calculator V1.0.xlsx` rate cards.

## Included
- Shipment checkout UI, destination PIN/state, invoice value, COD/prepaid, weight and multiple package dimensions.
- Volumetric weight follows the workbook dashboard formula: `L × W × H × boxes × 6 / 27000` (cm).
- State-level zone comparisons for DTDC Express, Delhivery, Safexpress and Spoton.
- Customer/address details, service selection and copyable booking request.

## Accuracy and limitations
- The workbook is configured for a Delhi NCR dispatch origin; this prototype uses that origin.
- This first public prototype uses **state-level zone mapping**, not the full PIN-level databases. PIN is captured for the booking request but does not currently validate carrier serviceability or calculate PIN-specific ODA charges.
- Rates are estimates from workbook rate cards, not live carrier API quotes. Other carriers in the workbook remain disabled pending formula reconciliation.
- The workbook's Delhivery calculator has broken external references; this version uses the standalone rate card and zone mapping.
- The form prepares a local, copyable booking request. It does not persist orders, book a carrier, generate labels, or accept payment.
- Confirm serviceability, remote-area charges, taxes, transit time and final freight before dispatch.

## GitHub Pages
Enable repository Settings → Pages → Deploy from a branch → `main` / root.

The original workbook and internal contact/credential sheets are intentionally not published.