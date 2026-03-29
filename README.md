# AI-Hospitality-Assistant
# 🧠 Prompt Library — AI Hospitality Booking Assistant

> Assessment 1 | BUS4005 - Artificial Intelligence for Business
> Student: Ananya Bhadauria  
> Business Field: Hospitality (Hotel Booking & Guest Experience Systems)  
> Model tested on: GPT-4
> Last updated: March 2026  

---

## 🌍 Industry Context & Innovation

Today, leading hotel chains such as Marriott use AI to enhance guest experience through chatbots, virtual concierges, and personalised recommendations. However, these innovations are primarily focused on improving services around the booking process, while the core booking experience itself remains largely form-based and unchanged.

This creates a clear gap.

Current systems still require users to navigate multiple screens, interpret options, and manually configure their booking. This process can be time-consuming, inefficient, and prone to errors.

This solution addresses the gap by redesigning the booking experience itself. Instead of starting with static forms, the system introduces an **intent-driven, conversational approach** that understands why the user is travelling and guides them step-by-step. It actively supports decision-making, recommends optimal configurations, prevents invalid selections, and connects inputs directly to operational outcomes such as room allocation and check-in preparation.

This transforms booking from a passive data-entry process into an intelligent, guided experience.

### 💡 Business Impact

For hotels:
- Reduced booking errors  
- Improved operational efficiency  
- Increased revenue through smarter upselling  

For guests:
- Faster booking experience  
- Reduced cognitive effort  
- More personalised and relevant interactions  

---

## Why This Is Better Than Traditional Apps

This model is more effective than traditional hotel apps because it moves beyond static, menu-driven interaction and provides a guided, conversational experience.

Traditional apps:
- Require navigation across multiple screens  
- Depend on manual input and user interpretation  
- Treat each step independently  

This system:
- Guides users step-by-step  
- Is context-aware (remembers previous inputs)  
- Adapts dynamically to user intent  
- Connects user input to real-time decisions (e.g., room allocation, check-in preparation, booking status)  

As a result, the experience is:
- More intuitive  
- More efficient  
- More personalised  

---

## 📌 What This Library Does

This prompt library automates the **end-to-end hotel guest journey**, transforming traditional booking systems into an **AI-powered conversational workflow**.

Instead of static forms, the system:
- captures user intent  
- guides booking decisions  
- validates inputs  
- personalises the experience  
- supports guests before, during, and after their stay  

The library contains **10 prompts**, structured across the full guest lifecycle.

---

## 📂 Folder Structure

AI-Hospitality-Assistant/

├── README.md  
├── workflow/  
│   └── booking-workflow.md  
│  
├── prompts/  
│   ├── P01-intent-dates.md  
│   ├── P02-guest-details.md  
│   ├── P03-room-configuration.md  
│   ├── P04-arrival-contact-payment.md  
│   ├── P05-personalisation-addons.md  
│   ├── P06-booking-confirmation.md  
│   ├── P07-pre-arrival-engagement.md  
│   ├── P08-during-stay-assistance.md  
│   ├── P09-service-recovery.md  
│   └── P10-post-stay-feedback.md  

---

## 📊 Library Summary Table

| ID | Prompt Name | Workflow Stage | Automation Level | Risk Level | Status |
|----|-------------|---------------|-----------------|------------|--------|
| P01 | Intent & Dates | Booking | High | Medium | ✅ |
| P02 | Guest Details | Booking | Very High | Medium | ✅ |
| P03 | Room Configuration | Booking | Very High | Medium | ✅ |
| P04 | Arrival, Contact & Payment | Booking | High | Medium | ✅ |
| P05 | Personalisation & Add-ons | Booking | High | Medium | ✅ |
| P06 | Booking Confirmation | Booking | Very High | Medium | ✅ |
| P07 | Pre-Arrival Engagement | Pre-Arrival | High | Low | ✅ |
| P08 | During Stay Assistance | In-Stay | Very High | Medium | ✅ |
| P09 | Service Recovery | In-Stay | High | High | ✅ |
| P10 | Post-Stay Feedback | Post-Stay | Very High | Medium | ✅ |

---

## 🔗 Prompt Chaining Map

### Booking Workflow
P01 → P02 → P03 → P04 → P05 → P06  

### Pre-Arrival Workflow
P06 → P07  

### In-Stay Workflow
P07 → P08 → P09  

### Post-Stay Workflow
P09 → P10  

---

## ⚙️ Prompting Strategies Used

| Strategy | Usage |
|----------|------|
| Role framing | “You are an AI-powered hotel booking assistant” |
| Step-by-step control | One question at a time interaction |
| Validation constraints | Email, phone, occupancy rules |
| Structured outputs (JSON) | Booking and service data |
| Context injection | Personalisation across lifecycle |
| Decision logic | Room allocation, payment handling |
| Error handling | Invalid inputs and guided correction |

---

## 🔄 Iteration Evidence

Each prompt includes **three or two versions (v1 → v3)** demonstrating:

- transition from manual input → structured interaction  
- introduction of validation rules  
- evolution into decision-support systems  
- improved clarity, accuracy, and usability  

---

## 📊 Business Value

### Operational Impact
- Reduces front desk workload by automating repetitive tasks  
- Improves coordination across departments  
- Enables proactive service preparation  

### Financial Impact
- Increases revenue through targeted upselling  
- Reduces booking abandonment  
- Improves room utilisation  

### Customer Experience
- Personalised booking journey  
- Faster service response  
- Seamless end-to-end experience  

### Strategic Impact
- Transforms booking into a full guest lifecycle system  
- Enables data-driven decision making  
- Strengthens long-term customer relationships  

---

