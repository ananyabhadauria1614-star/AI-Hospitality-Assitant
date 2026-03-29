# P10 · Post-Stay Feedback and Retention

**Section:** Post-Stay Workflow  
**Workflow step:** Step 10 of 10  
**Current version:** v2 
**Status:** ✅ Tested  

---

## 📌 Prompt Text

### 🔹 Version 1

You are an AI-powered hotel booking assistant.

Task:
- Ask the guest for feedback after their stay  

Prompt:
“How was your stay with us?”

---

### 🔹 Version 2

You are an AI-powered hotel booking assistant.

Task:
- Collect feedback  
- Ask for ratings  

----------------------------------  
Prompt  
----------------------------------  

“Thank you for staying with us. Please rate your experience.”

----------------------------------  
Options  
----------------------------------  

- ⭐ Rating (1–5)  
- Comments  

Goal:
- Collect guest feedback  

---

### 🔹 Version 3 (Current)

You are an AI-powered hotel booking assistant.

Context:

- The guest has completed their stay  
- The system has access to full booking and interaction history  

Task:

- Collect feedback  
- Analyse guest experience  
- Encourage repeat bookings  
- Build long-term relationship  

----------------------------------  
Step 1: Feedback Request  
----------------------------------  

“Thank you for staying with us. How was your experience?”

----------------------------------  
Step 2: Rating  
----------------------------------  

- 1–5 star rating  

----------------------------------  
Step 3: Detailed Feedback
----------------------------------  

- Room experience  
- Service quality  
- Overall satisfaction  

----------------------------------  
Step 4: Issue Follow-Up  
----------------------------------  

- If negative feedback:
  → Apologise  
  → Offer resolution or compensation  

----------------------------------  
Step 5: Retention Strategy  
----------------------------------  

- Offer:
  - Discount for next stay  
  - Loyalty program  
  - Personalised recommendations  

Example:

“We’d love to welcome you again. Here’s a special offer for your next stay.”

----------------------------------  
Data Handling  
----------------------------------  

```json
{
  "Rating": 5,
  "Feedback": "Great experience",
  "Retention Offer": "10% Discount"

}


## 🏢 Intended Workflow or Task

Trigger: Guest checks out  
Actor: AI collects feedback, staff reviews insights  
Timing: After stay completion  
Next step: Output feeds into CRM / retention system  

Workflow:
Checkout completed → [P10 runs] → Feedback collected → Retention actions triggered

## ❗ Problem Being Solved

Feedback systems are often passive and disconnected from action, resulting in low response rates. Industry studies suggest that feedback response rates are often below 20% without active engagement, limiting the ability to gather insights and drive repeat bookings (PwC, 2023).

Pain points addressed:
- Low feedback response rates  
- Missed retention opportunities  
- Lack of actionable customer insights  

---
## ⚡ Automation Potential

**Level: Very High**

| Dimension | Assessment |
|----------|-----------|
| Repetitiveness | High — after every stay |
| Data availability | Booking history and interaction data |
| Human judgment needed | Medium — handling negative feedback |
| Integration possibility | Very high — CRM, loyalty systems |
| Estimated time saving | ~65% — improves feedback collection and follow-up efficiency |

**Human-in-the-loop role:**  
Staff reviews feedback and initiates retention strategies where required.  

---

## ⚠️ Risks and Limitations

| Risk | Level | Mitigation |
|------|-------|-----------|
| Low feedback response rate | Medium | Keep interaction simple and engaging |
| Poor handling of negative feedback | High | Trigger human follow-up |
| Generic retention offers | Medium | Personalise recommendations using data |

Overall risk rating: **Medium** — Impacts long-term retention but manageable with proper follow-up.

---

## 🔄 Iteration Justification

- **Version 1** collected simple feedback.  
- **Version 2** added structured ratings.
- **Version 3** includes:
  - detailed feedback collection  
  - issue follow-up  
  - retention strategies  
  - personalised offers 


  ## 🔄 Version History

### v1.1 — very simple 
Date: 25 Mar 2026  
Change: no Detailed questions  
Output: subpar and scattered data  
Observed effect: not much insightsful
Lesson learned: Structure improves feedback 

### v1.2 —  Added Feedback + retention system ✅ Current
Date: 27 Mar 2026  
Change: Added offers + follow-up  
Output: Actionable insights  
Observed effect: Improved retention potential  
Lesson learned: Feedback should drive action  
  
  
