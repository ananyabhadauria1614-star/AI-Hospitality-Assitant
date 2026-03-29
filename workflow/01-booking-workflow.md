## 📂 01 — Booking Workflow  
**Business function:** Booking & Reservation Management  
**Trigger:** User initiates booking on hotel website  
**Prompts in this section:** P01, P02, P03, P04, P05, P06  

---

## Section Purpose  

These prompts automate the complete booking process, from initial intent capture to final confirmation and payment. Traditional booking systems require users to navigate multiple disconnected steps, increasing drop-offs and errors. This workflow reduces booking completion time from ~10–15 minutes to under 3–5 minutes, while improving accuracy, personalisation, and conversion rates.

---

## Chain Diagram  

User clicks “Book a Stay”  
        │  
        ▼  
   P01 · Intent & Dates  
   (Session start — context creation)  
        │  
        ▼  
   P02 · Guest Details  
   (Contact capture & validation)  
        │  
        ▼  
   P03 · Guests & Room Configuration  
   (System recommendation)  
        │  
        ▼  
   P04 · Arrival, Contact & Payment  
   (Operational decisions)  
        │  
        ▼  
   P05 · Personalisation & Add-ons  
   (Upsell & preferences)  
        │  
        ▼  
   P06 · Booking Summary & Confirmation  
   (Payment + booking completion)  

---

## Human-in-the-Loop Points  

| Step | Human action required |
|------|----------------------|
| P02 output | Staff reviews invalid or flagged contact details |
| P03 output | Staff overrides room allocation if needed |
| P04 output | Staff monitors payment or special arrival requests |
| P05 output | Staff validates add-on feasibility |
| P06 output | Staff intervenes in payment failure or booking conflict |