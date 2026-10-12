# m.me-kiosk-sellerpage
# 🛒 ShareMap MessengerStore's Kiosk System

**ShareMap MessengerStore** is a scalable, web-based e-commerce order and dispatch platform designed specifically for Facebook Page merchants (MSMEs, restaurants, groceries, and wet market sellers). It leverages direct Messenger integration and ultra-accurate GPS location capture using **ShareMap Digital Address** to streamline local ordering and delivery fulfillment without high third-party app commissions.

---

## 🚀 Key Features & Value Proposition

* **Dual Ordering Modes:**
  * **Full Kiosk Mode:** High-visual, category-based interactive menu tailored for fast food, milk tea shops, and restaurants.
  * **Semi-Kiosk Mode:** Dynamic, flexible dispatch system designed for fast-changing inventories like wet markets (*palengke*) and mini-marts.
* **Smart GPS & Delivery Dispatch:** Auto-detects high-accuracy GPS coordinates using native browser location API and generates standard Google Maps/Plus Codes navigation links for seamless delivery rider handoff.
* **Direct Messenger Integration:** Eliminates expensive third-party commission fees by converting social media followers directly into buyers via Messenger chat links.
* **Zero App Download:** Works instantly on mobile browsers inside Facebook/Messenger auto-replies or QR codes.

---

## 🗺️ System Architecture & Dashboard Links

Below is the complete ecosystem breakdown of the ShareMap MessengerStore Kiosk Platform:

### 🛍️ Customer-Facing Interfaces
* **Primary Visual Kiosk Menu (`kioskmode.html`):**  
  The main visual entry point for buyers to browse rich photo categories, select items, and add to cart (Fast Food / Restaurant Style).  
  🔗 [Open Kiosk Mode](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/kioskmode.html?page=YourFbPageUsername)

* **Order Checkout & Location Gateway (`multigateway.html`):**  
  Captures order summaries, table numbers for dine-in, or delivery address preferences prior to submitting to Messenger.  
  🔗 [Open Checkout Gateway](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/multigateway.html?page=sharemapdammystore)

* **GPS & Delivery Order Dispatch (`index.html`):**  
  Captures high-accuracy device GPS coordinates and formats standardized ShareMap location pins for delivery riders.  
  🔗 [Open Dispatch Gateway](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/index.html)

---

### 🔑 Merchant & Admin Management Portals
* **Kiosk Store Manager Dashboard (`createmenugateway.html`):**  
  Merchant portal for updating menu items, managing inventory availability (In Stock / Out of Stock), pricing, and Google Drive image links.  
  🔗 [Open Store Manager](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/createmenugateway.html?)

* **Account Security & Password Gateway (`accountgateway.html`):**  
  Dedicated portal for newly onboarded store owners to set up or update their secure store passwords.  
  🔗 [Open Account Security Portal](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/accountgateway.html?page=YourFbPageUsername)

* **Master Admin Developer Dashboard (`admin.html`):**  
  Secure master portal for system administrators to generate merchant licenses, manage client subscriptions, and trigger activation templates.  
  🔗 [Open Admin Portal](https://sharemap-digital-address.github.io/m.me-kiosk-sellerpage/admin.html?)

---

## 🛠️ Tech Stack & Infrastructure

* **Frontend:** HTML5, CSS3 (CSS Variables, Responsive Flexbox/Grid), JavaScript (ES6+)
* **Backend & Database:** Supabase (PostgreSQL with Row Level Security and Upsert functionality)
* **Location API:** Native Browser Geolocation API & Web Share API
* **Hosting:** GitHub Pages
