## 📂 03 — In-Stay Workflow  
**Business function:** Service Delivery & Guest Experience  
**Trigger:** Guest checks in / stay begins  
**Prompts in this section:** P08, P09  

---

## Section Purpose  

These prompts manage real-time guest interactions during the stay, including service requests and issue resolution. Traditional hotel service relies heavily on manual coordination, leading to delays. This workflow enables real-time request handling, reducing response time from ~5–15 minutes to near-instant acknowledgement and faster execution.

---

## Chain Diagram  

Guest checks in  
        │  
        ▼  
   P08 · During Stay Assistance  
   (Service requests + concierge)  
        │  
        ▼  
If issue occurs  
        │  
        ▼  
   P09 · Support & Service Recovery  
   (Escalation + resolution)  

---

## Human-in-the-Loop Points  

| Step | Human action required |
|------|----------------------|
| P08 output | Departments execute service requests |
| P09 output | Managers handle escalations and compensation |

---