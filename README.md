# 🏪 CHA CONVENIENCE STORE — Point of Sale (POS)

A full-featured, zero-setup **Convenience Store Point of Sale (POS)** web application built with **React 18** and **Tailwind CSS**, designed for Philippine convenience stores and supermarkets with **Philippine Peso (₱ / PHP)** currency, DTI Suggested Retail Prices (SRP), and BIR VAT compliance in the **English language**.

📍 **Address**: Bankers Subd. Antipolo City, Rizal  
📞 **Tel**: (02) 8921-4455 / 0917-882-9090  

---

## 🚀 Instant Zero-Setup Launch
Open [`index.html`](./index.html) directly in any modern web browser (Google Chrome, Microsoft Edge, Safari, Mozilla Firefox) — **no build step, no Node.js, and no server configuration required**.

---

## ✨ What's New & Core Capabilities

### 1. ➕ Auto-Generated Barcode Items with Editable Prices (`F3`)
- **Auto EAN-13 Generator**: Generates authentic 13-digit Philippine barcodes (prefix `480` + 9 unique digits + checksum) with one click of **⚡ Generate New**.
- **Editable Pricing**: Easily customize Selling Price (₱ SRP) and Cost Price for live margin tracking.
- **Weighed (/kg) & Tax Settings**: Toggle whether the item is sold by weight (activating the digital scale) and whether it is VAT-Exempt (fresh agricultural/marine goods) or VATable (12%).
- Once created, new items appear immediately in the product catalog and can be scanned, searched, or weighed.

### 2. 👥 Cashier Management, Log-in & Log-Out
- **Cashier List Management**:
  - Add new cashiers and staff with customized roles (*Senior Cashier*, *Cashier*, *Shift Supervisor*, *Store Manager*) and unique 4-digit PINs.
  - Remove cashiers with safety validation (cannot delete the active cashier).
  - Switch active cashier on the fly.
- **Log-in & Log-Out System**:
  - Click **🔒 Log Out** in the top navigation bar to lock the POS register.
  - Interactive PIN lock screen with numeric touchscreen keypad to select cashier and unlock the register.
  - Active cashier's name and ID are stamped on all completed transactions, thermal receipts, and shift sales reports.

### 3. 📱 Mobile Screen Fitting & PWA App
- **Adaptive Mobile Layout (`100dvh`)**:
  - Dynamically resizes to match mobile viewports without vertical overflow, address bar clipping, or awkward scrolling.
  - Dedicated **Mobile Bottom Navigation Bar** (`Catalog`, `Cart (with live badge)`, `Add Item`, `Printers`, `More Options`).
  - Seamless touch targets, responsive touch keypad, and collapsible side panels for single-handed mobile cashier operation.
- **Mobile App Install QR Code**:
  - Tap **📱 Mobile** or **QR Code** in the navigation bar to bring up an interactive high-resolution QR code.
  - Scan with any smartphone or tablet camera (Android or iOS) to open the POS immediately on the local network or web.
  - **Android**: Tap Chrome menu `⋮` &gt; tap **"Install app"** or **"Add to Home screen"**.
  - **iPhone / iPad**: Tap Safari Share button `⬆` &gt; tap **"Add to Home Screen"**.
  - Supports 100% offline capability via Service Worker (`sw.js`).

### 4. 🖨️ Available Printers List & Thermal POS Hardware
- **Available Printers Button**:
  - Direct access via the header **🖨️ Printers** button (with live green pulse status) and the mobile bottom navigation bar.
- **Hardware Integration Options**:
  - **Bluetooth ESC/POS Thermal Printers**: One-tap scan and pair via Web Bluetooth API for portable mobile printers (Sunmi, Goojprt, PeriPage, MPT-II, etc.).
  - **USB POS Printers**: Plug-and-play detection via WebUSB API (Epson TM-T88/T20, Xprinter, Rongta, POS-58/80).
  - **System Default / AirPrint / Network**: Connects directly to local network printers, Windows spoolers, and iOS AirPrint.
- **Paper Size Format Switch**:
  - Instant toggle between **80mm Standard POS** (supermarket counter width) and **58mm Compact POS** (mobile belt clip width).
- **Auto-Print & Test Print**:
  - Toggle auto-receipt printing upon checkout completion.
  - One-click **Test Receipt Print** directly inside the printer setup modal.

---

## 🇵🇭 Philippine Market & Regulatory Features

1. **Philippine Peso (₱) Currency & Cash Tender**:
   - Quick tender buttons for authentic Philippine Peso banknotes: **₱1,000, ₱500, ₱200, ₱100, ₱50, ₱20**, and **Exact Amount**.
   - Automatic **Change Due** calculation with cash denomination breakdown guide for cashiers (e.g., `1x ₱200, 1x ₱50, 1x ₱20, 1x ₱5`).

2. **Digital E-Wallets & Card Payments**:
   - **GCash QR** simulation with reference number input.
   - **Maya QR** simulation.
   - **Debit / Credit Card POS Terminal** authorization tracking.

3. **BIR Tax Compliance & Dual Tax Rates**:
   - **VATable Goods (12% VAT)**: Processed food, canned goods, household items, beverages, and personal care.
   - **VAT-Exempt Goods**: Fresh, unprocessed agricultural and marine food products (Rice, Fresh Vegetables, Fruits, Eggs, Raw Meat, Fresh Fish) pursuant to Section 109 of the National Internal Revenue Code (NIRC).
   - Clear breakdown of **VATable Sales (Net of 12%)**, **VAT Amount (12%)**, and **VAT-Exempt Sales**.

4. **Republic Act 9994 & RA 10754 Senior Citizen & PWD 5% Grocery Discount**:
   - Built-in 5% discount on Basic Necessities and Prime Commodities (BNPC) for Senior Citizens and Persons with Disability (PWD).
   - OSCA / PWD ID verification tracking printed directly onto the invoice receipt.

5. **Local Bag Fees & Eco Regulations**:
   - One-tap toggle for Sando Bag / Eco Bag fee (+₱2.00) in compliance with city plastic ordinances.

---

## ⚖️ Weighed Produce & Barcode / PLU Scanning

- **Interactive Digital Scale Simulator**:
  - Automatically activates for items sold per kilogram (`/kg`) such as Rice, Fresh Produce (Onions, Tomatoes, Calamansi, Bananas), and Fresh Meat & Seafood (Chicken, Pork Liempo, Bangus).
  - Supports tare weights, quick additions (`+100g`, `+250g`, `+500g`, `+1.0kg`), and manual kilogram typing with live price updates.
- **Hardware Barcode Scanner Support**:
  - Ready for USB/Bluetooth handheld barcode scanners (EAN-13 keyboard wedge emulation).
- **PLU Quick Code Entry**:
  - Quick lookup for produce without barcodes (e.g. `4011` for Lakatan Bananas, `2001` for Red Onions, `3001` for Fresh Whole Chicken).

---

## 🖨️ BIR Compliant 80mm / 58mm Thermal Receipt Printing

- Formatted for standard 80mm thermal receipt printers (Epson, Xprinter, Sunmi, etc.).
- Complete Official Sales Invoice layout with Store Address (*Bankers Subd. Antipolo City, Rizal*), TIN, Machine Serial, MIN, Cashier name, itemized sales with tax identifiers `(V)` and `(E)`, VAT analysis, payment tendered, change due, and return barcode.
- Click **Print Receipt** or press `Ctrl + P` for standard `@media print` styling.

---

## ⌨️ Keyboard Shortcuts Reference

| Shortcut | Function |
| :--- | :--- |
| **`F2`** | Focus Barcode / Search Box |
| **`F3`** | Open Add Barcode Item Modal |
| **`F4`** | View Parked / Held Carts |
| **`F8`** | Open Inventory & Price Manager |
| **`F9`** | Open Daily Shift & Z-Report |
| **`F12`** | Proceed to Checkout |
| **`Esc`** | Close any open modal |
