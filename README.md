# Fuel Inventory Management System & Variance Checker ⛽

A high-performance, lightweight single-page application (SPA) built for retail fuel station operations in the Philippines. This system handles real-time wet stock reconciliation, Philippine Suggested Retail Price (Ph-SRP) financial auditing, and automated Underground Storage Tank (UST) priority order forecasting.

## 🚀 Live Demo
Access the live dashboard here:
https://jomerbiason.github.io/fuel-inventory-management-system-and-variance-checker/

---

## 🗺️ Local Market Context: "Tuesday Adjustments"
In the Philippine downstream oil industry, fuel pricing follows a structured routine:

1. Monday Afternoon: Oil firms announce nationwide price hikes or rollbacks.
2. Tuesday Morning (6:00 AM): These pricing updates officially go live.

This application is built directly into that operational workflow. Station managers configure the price matrix during the pre-dawn hours on Tuesday. Once saved, the transaction system instantly tracks variances and asset sheets against the true running pump rates for that shift cycle.

## 🛠️ Key System Features
* Wet Stock Audit Engine: Cross-examines computer sales against manual physical dipstick readings.
* 0.5% Industry Standard Safeguard: Automatically flags inventory discrepancies as CRITICAL if they exceed the industry-standard 0.5% volumetric threshold.
* Historical Price Lock: Historic transactions retain their exact pricing metrics to protect financial auditing records from retrospective drift.
* UST Forecasting: Real-time progress bars provide visual alerts. If tanks drop to or below 30% capacity, the system triggers a Priority Order Alert.
* GitHub Pages Ready: Fully optimized for static hosting via GitHub Pages.

---

## 📐 Mathematical Blueprint

### Daily Book Inventory Balance
The expected book stock is calculated as:
I_expected = (I_opening + V_delivery) - V_sales

### Variance Monetary Evaluation
The financial impact is determined by:
E_monetary = (I_physical - I_expected) * P_SRP

(Where P_SRP is the immutable board rate at the time of the transaction)

---

## 🚀 How to Run Locally
Because this application is a pure client-side SPA, you can run it directly in your browser without any backend dependencies:

1. Clone the repository:
git clone https://github.com/jomerbiason/fuel-inventory-management-system-and-varicance-checker.git

2. Open the project:
Simply open index.html in your favorite web browser (Chrome, Edge, or Firefox).

3. Deploying to GitHub Pages:
If you make changes, simply push your code to the main branch. GitHub Actions will automatically redeploy your updates to your live link.

---

## 📋 Data Persistence
This system uses browser localStorage. Your data is private and saved locally on your machine. You can export your audit logs at any time using the "Export Audit Sheet (.CSV)" button within the application.

## ⚖️ License
Distributed under the MIT License.
