# ADDENDUM — Arlo: New **Current Coverage** field
*Effective immediately (Q4 2025). This addendum supersedes prior Arlo form instructions wherever applicable and must be applied in **all** submissions.*

---

## 1) What changed
Arlo introduced a new required form field named **Current Coverage** placed **between** **Effective Date** and **Census** on the *New Quote* page. It presents the following **exact** selectable options:

- **Level-funded plan**
- **Self-insured plan**
- **Fully-insured plan**
- **Through PEO**
- **No Coverage**

> Position in form (updated order):
> 1. Group Name → 2. Programs to Quote → 3. HQ State → 4. Effective Date → **5. Current Coverage** → 6. Census → 7. Additional Files → 8. “I confirm…” checkbox → 9. Submit.

---

## 2) How this affects our standard instructions
- All Arlo submission checklists and copy/paste blocks **must include** the new **Current Coverage** field in the exact position shown above.
- When drafting instructions for the user, always show the field as a separate block, just like the others (title outside, content inside code block), per our fixed format.

---

## 3) Mapping to HubSpot (stay consistent across systems)
Use the mapping below to keep Arlo **Current Coverage** aligned with HubSpot **Employer Current Insurance Type**.

| Arlo – Current Coverage | HubSpot – Employer Current Insurance Type |
|---|---|
| **Level-funded plan** | **Level Funded** |
| **Self-insured plan** | **Traditional Medical Stop Loss** *(self-funded)* |
| **Fully-insured plan** | **Fully Insured** |
| **Through PEO** | **Other** *(and clarify in Ticket description: “Through PEO”)* |
| **No Coverage** | **None** |

**Notes:**
- If the RFP/email explicitly states current carrier is level-funded or self-funded, mirror it in both places.
- For **PEO**, Arlo has a dedicated option; HubSpot does not. Select **Other** in HubSpot and document **“Through PEO”** in *Ticket description*.

---

## 4) Quick selection rules (copy-ready)
- **Virgin group** (no medical in force): choose **No Coverage**.
- **Currently Fully Insured** (e.g., Anthem, UHC, BCBS, Aetna): choose **Fully-insured plan**.
- **Currently Level Funded** (any carrier TPA): choose **Level-funded plan**.
- **Currently Self-funded/ASI/Traditional Stop Loss**: choose **Self-insured plan**.
- **Covered via PEO** (TriNet, Insperity, ADP TotalSource, etc.): choose **Through PEO**.

---

## 5) Example blocks to include in every Arlo instruction set
**Current Coverage:**
```
Fully-insured plan
```
*(Replace with the five exact strings as applicable.)*

---

## 6) Compliance with our Fixed Instructions
- The **INSTRUÇÕES FIXAS** document is updated by reference: every Arlo section must now list **Current Coverage** after **Effective Date** and before **Census**.
- The **LevelHealth_Full_Guide.md** workflow references this addendum for Q4 2025; if the Arlo UI changes again, this addendum must be revised.

---

## 7) Edge cases & troubleshooting
- If the broker’s description conflicts with renewal/SBC, prefer **renewal/SBC** and note the discrepancy in the HubSpot **Ticket description**.
- If unknown, infer from documents. Only as a last resort, temporarily select **Fully-insured plan** or **None** based on strongest evidence, and document the assumption in the note.
- This field does **not** change MGU routing rules (Q4 table still governs). It only clarifies the current funding arrangement to Arlo.

---

## 8) Audit checklist (add to your pre-submit review)
- [ ] **Current Coverage** populated with the exact string from the five options.
- [ ] HubSpot **Employer Current Insurance Type** set to the mapped value.
- [ ] Ticket description includes clarifier when **Through PEO** is chosen.
- [ ] Arlo field appears in the correct position in our copy/paste instruction set.

---

*Owner:* Assistente de Cotação LevelHealth Simpara  
*Status:* Active  
*Version:* Q4 2025 — v1.0  
*Next review:* On next Arlo UI change or Jan 2026 transition.

