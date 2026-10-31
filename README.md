# 🛒 MAHARLIKA — Philippine Grocery Store & Supermarket Point of Sale (POS)

A full-featured, zero-setup **Philippine Grocery Store & Supermarket Point of Sale (POS)** web application built with **React 18** and **Tailwind CSS**, designed specifically for Philippine businesses, sari-sari stores, and supermarkets with **Philippine Peso (₱ / PHP)** currency, DTI 2026 Suggested Retail Prices (SRP), and BIR VAT compliance.

---

## 🚀 Instant Zero-Setup Launch
Open [`index.html`](./index.html) directly in any modern web browser (Google Chrome, Microsoft Edge, Safari, Mozilla Firefox) — **no build step, no Node.js, and no server configuration required**.

---

## 🇵🇭 Philippine Market & Regulatory Features

1. **Philippine Peso (₱) Currency & Cash Denominations**:
   - Quick tender buttons for authentic Philippine Peso banknotes: **₱1,000, ₱500, ₱200, ₱100, ₱50, ₱20**, and **Exact Amount**.
   - Automatic **Sukli (Change Due)** calculation with cash denomination breakdown guide for cashiers (e.g., `1x ₱200, 1x ₱50, 1x ₱20, 1x ₱5`).

2. **Philippine Digital E-Wallets & Card Payments**:
   - **GCash QR** simulation with reference number input.
   - **Maya QR** simulation.
   - **Debit / Credit Card Terminal** authorization code tracker.

3. **BIR Tax Compliance & Dual Tax Rates**:
   - **VATable Goods (12% VAT)**: Processed food, canned goods, household items, beverages, and personal care.
   - **VAT-Exempt Goods**: Fresh, unprocessed agricultural and marine food products (Rice, Fresh Vegetables, Fruits, Eggs, Raw Meat, Fresh Fish) pursuant to Section 109 of the National Internal Revenue Code (NIRC).
   - Clean breakdown of **VATable Sales (Net of 12%)**, **VAT Amount (12%)**, and **VAT-Exempt Sales**.

4. **Republic Act 9994 & RA 10754 Senior Citizen & PWD 5% Grocery Discount**:
   - Built-in 5% discount on Basic Necessities and Prime Commodities (BNPC) for Senior Citizens and Persons with Disability (PWD).
   - OSCA / PWD ID verification tracking printed directly onto the invoice receipt.

5. **Local Bag Fees & Eco Regulations**:
   - One-tap toggle for Sando Bag / Eco Bag fee (+₱2.00) in compliance with local city plastic ordinances.

---

## ⚖️ Weighed Produce & Barcode / PLU Scanning

- **Interactive Digital Scale Simulator**:
  - Automatically activates for items sold per kilogram (`/kg`) such as Rice, Produce (Onions, Tomatoes, Calamansi, Bananas), and Fresh Meat & Seafood (Chicken, Pork Liempo, Bangus).
  - Supports tare weights, quick additions (`+100g`, `+250g`, `+500g`, `+1.0kg`), and manual kilogram typing with live price updates.
- **Hardware Barcode Scanner Support**:
  - Ready for USB/Bluetooth handheld barcode scanners (EAN-13 keyboard wedge emulation).
- **PLU Quick Code Entry**:
  - Quick lookup for produce without barcodes (e.g. `4011` for Lakatan Bananas, `2001` for Red Onions, `3001` for Fresh Whole Chicken).

---

## 🖨️ BIR Compliant 80mm / 58mm Thermal Receipt Printing

- Formatted for standard 80mm thermal receipt printers (Epson, Xprinter, Sunmi, etc.).
- Complete Official Sales Invoice layout with Store TIN, Machine Serial, MIN, Cashier name, itemized sales with tax identifiers `(V)` and `(E)`, VAT analysis, payment tendered, change due, and return barcode.
- Click **Print Receipt** or press `Ctrl + P` for standard `@media print` styling.

---

## 📦 Inventory Management & Shift Z-Reports

- **Inventory Modal (`F8`)**:
  - Live stock deductions upon checkout.
  - Low-stock visual warning badges (`<= 10`).
  - In-app price editor and one-click `+Restock` actions.
- **Shift Z-Report (`F9`)**:
  - Real-time cashier end-of-shift reconciliation.
  - Cash in drawer breakdown vs. GCash, Maya, and Card collections.
  - BIR VAT totals and Senior/PWD discounts audit.
- **Park / Hold Orders (`F4`)**:
  - Hold multiple customer carts with custom labels when a shopper forgets their wallet or grabs additional items.

---

## ⌨️ Keyboard Shortcuts Reference

| Shortcut | Function |
| :--- | :--- |
| **`F2`** | Focus Barcode / Search Box |
| **`F4`** | View Parked / Held Carts |
| **`F8`** | Open Inventory & Price Manager |
| **`F9`** | Open Daily Shift & Z-Report |
| **`F12`** | Proceed to Checkout / Bayad |
| **`Esc`** | Close any open modal |

---

## 📱 PWA & Offline Support
- Built-in `manifest.json` and `sw.js` (Service Worker) allows full offline functionality and home screen installation on Windows, Android, iOS, and macOS tablets and POS terminals.
