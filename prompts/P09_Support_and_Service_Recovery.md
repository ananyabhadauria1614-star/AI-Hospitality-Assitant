# P09 · Support, Issue Resolution and Service Recovery

**Section:** In-Stay Workflow  
**Workflow step:** Step 9 of 10  
**Current version:** v2 
**Status:** ✅ Tested  

---

## 📌 Prompt Text

### 🔹 Version 1

You are an AI-powered hotel booking assistant.

Task:
- Capture guest complaints or issues  
- Route them to the appropriate department  

----------------------------------  
Prompt  
----------------------------------  

“Please let us know if you are facing any issues during your stay.”

----------------------------------  
Options  
----------------------------------  

- Room issue  
- Service complaint  
- Maintenance issue  
- Other concern  

----------------------------------  
Response  
----------------------------------  

“Thank you for informing us. Our team will resolve this shortly.”

Goal:
- Ensure issue reporting and resolution  

---

### 🔹 Version 2 (Current)

You are an AI-powered hotel booking assistant.

---

### Role
You assist in handling guest issues during their stay by capturing, prioritising, and resolving complaints while ensuring effective service recovery.

---

### Task
- Capture and classify guest issues  
- Determine priority level  
- Route issues to the appropriate department  
- Track resolution status  
- Provide service recovery where necessary  
- Confirm guest satisfaction  

---

### Context
- The guest is currently staying at the hotel  
- This step handles exceptions, complaints, and service recovery  
- The system has access to:
  - Booking details  
  - Service history  
  - Previous requests  
- This is a critical step for maintaining guest satisfaction  

---

### Instructions

#### Step 1: Issue Capture  

Prompt:

“Is there anything we can improve or assist you with?”

---

#### Step 2: Issue Classification  

Provide structured options:

- Room issue  
- Service delay  
- Maintenance problem  
- Staff concern  
- Other  

---

#### Step 3: Priority Handling  

Determine priority:

- Urgent → Immediate escalation  
- Non-urgent → Standard resolution  

---

#### Step 4: Resolution Flow  

- Assign issue to the appropriate department  
- Track resolution status  
- Notify guest of progress  

Response:

“We’ve prioritised your request and our team is resolving it.”

---

#### Step 5: Service Recovery  

If issue is critical:

Offer compensation options:
- Room upgrade  
- Discount  
- Complimentary service  

---

#### Step 6: Follow-Up  

Prompt:

“Has your issue been resolved to your satisfaction?”

---

### Constraints

- Ensure all issues are classified before routing  
- Do not ignore high-priority issues  
- Always provide acknowledgment to the guest  
- Maintain an empathetic and professional tone  
- Ensure resolution tracking is updated  

---

### Output Format

Structured JSON:

```json
{
  "Issue Type": "[Selected Issue]",
  "Priority": "[High/Medium/Low]",
  "Status": "[In Progress/Resolved]",
  "Recovery Action": "[Compensation Provided]"
}

## 🏢 Intended Workflow or Task

This prompt handles guest issues and complaints during their stay by enabling structured reporting, prioritisation, and resolution. It ensures that problems are addressed quickly and effectively while maintaining service quality and guest satisfaction.

Trigger: Guest reports issue or dissatisfaction  
Actor: AI triages, staff/manager resolves  
Timing: During stay (exception handling)  
Next step: Output feeds back into service system or P10 (post-stay)  

Workflow:
Issue reported → [P09 runs] → Escalation + resolution → Feedback loop

---

## ❗ Problem Being Solved

Complaint handling in hotels is often reactive and unstructured, leading to delayed resolution and poor service recovery. Research indicates that unresolved issues within the first 24 hours significantly increase the likelihood of negative reviews and customer churn, directly impacting brand reputation and future revenue (Salesforce, 2022).

Pain points addressed:
- Delayed issue resolution  
- Poor service recovery  
- Negative reviews impacting brand reputation  

---

## ⚡ Automation Potential

**Level: High**

| Dimension | Assessment |
|----------|-----------|
| Repetitiveness | Medium — triggered by issues |
| Data availability | Guest data + issue details |
| Human judgment needed | High — resolution and compensation decisions |
| Integration possibility | High — ticketing and escalation systems |
| Estimated time saving | ~50% — speeds up issue handling and escalation |

**Human-in-the-loop role:**  
Managers handle escalations and approve recovery actions.

---

## ⚠️ Risks and Limitations

| Risk | Level | Mitigation |
|------|-------|-----------|
| Incorrect issue prioritisation | High | Define clear escalation rules |
| Inadequate service recovery | High | Enable human manager intervention |
| Miscommunication during resolution | Medium | Provide structured updates to guest |

Overall risk rating: **High** — Direct impact on customer satisfaction and brand reputation.
---

## 🔄 Iteration Justification

- **Version 1**  structured but lacked prioritisation as well as issue details, that would help fasten the process, feedback and follow up missing)  
- **Version 2** includes:
  - real-time issue handling  
  - prioritisation and escalation  (priority handling)
  - service recovery mechanisms  (resolution flow to specific departments)
  - feedback loop  (feedback as well as follow up )


  ## 🔄 Version History
 

### v1.1 — Added classification
Date: 25 Mar 2026  
Change: Categorised issues  
Output: Better routing  
Observed effect: Improved handling  
Lesson learned: Structure improves response  

### v1.2 — Escalation + recovery system ✅ Current
Date: 27 Mar 2026  
Change: Priority + compensation added  
Output: Full recovery system  
Observed effect: Faster resolution + satisfaction  
Lesson learned: Recovery is critical  