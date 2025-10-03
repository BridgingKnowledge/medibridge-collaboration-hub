# Feedback Log – 15 Jan 2025

## 🧑‍⚕️ Clinician Request
> “It takes too many clicks to save a case. I would like a single button that saves everything at once.”

---

## 🔍 Analysis
- Current workflow: requires 3 steps (Save → Confirm → Upload).  
- Clinician frustration: slows down consultation, distracts from patient.  
- Risk: clinicians may skip saving or delay documentation.  

---

## 📖 User Story (for Developers)
**As a clinician**,  I want to save a case with one click,  so that I can focus on the patient instead of the system.  

- **Context:** Requested by multiple clinicians during training.  
- **Expected Outcome:** Faster workflow, less frustration.  
- **Priority:** ✅ Must Have (workflow efficiency).  

---

## 🛠️ Developer Notes
- Technical constraint: validation of data must occur before upload.  
- Risk: skipping validation could compromise data integrity.  
- Possible solution: run validation in the background after the “Save” click.  

---

## 📢 Feedback to Clinicians
- ❌ A single button that bypasses validation is **not feasible**.  
- ✅ Alternative: We will implement a **“Save & Validate” button**.  
  - Clinician clicks once.  
  - System saves immediately.  
  - Validation runs in the background.  
  - If issues are found, clinician is notified later.  

**Simplified explanation:**  
> “We can’t remove the validation step, because it ensures patient data is correct. But we can make it invisible to you, so it feels like one click.”  

---

## 📊 Status
- 🛠️ In Progress (planned for next release).  
- Next step: Developer prototype → Specialist test → Clinician pilot.  
