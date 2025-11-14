# LEVELHEALTH — Census Counting Rules (Q4 2025 definitive)

**Authority:** INSTRUÇÕES FIXAS + LevelHealth_Full_Guide + Addendums (Q4 2025)  
**Purpose:** Eliminate counting drift. This file codifies the rules the assistant MUST apply when reading any census.

## 1) Who counts
- Count **only rows with `Relationship = 'E'`** (employees).  
- **Do not** count dependents (`'S'`, `'C'`) as enrolled or eligible.

## 2) Coverage Tier meanings (employees only)
- Enrolled = **EE + ES + EC + EF** (for `Relationship = 'E'` only).  
- Eligible = **Enrolled + W** (for `Relationship = 'E'` only).  
- Participation Rate = **Enrolled / Eligible**.

## 3) Data hygiene
- If a waiver appears incorrectly as `Relationship = 'W'`, this is a **bad input**.  
  - The assistant must **not** treat `Relationship = 'W'` as an employee.  
  - A *waived employee* should be `Relationship = 'E'` with `Coverage Tier = 'W'`.
- Do not request `Address/City/State` columns; they are **not required**.
- Validate tiers inside each family:
  - ES must have exactly 1 spouse row; EC at least 1 child; EF must have both.
  - No dependent without its matching employee.

## 4) Location logic
- Determine ZIP distribution from employees (`Relationship = 'E'`) only.
- Use the predominant ZIP to drive network selection per Q4 Missouri/Georgia rules.

## 5) Q4 routing reminder (copy from guides)
- 5–50 enrolled ⇒ **Arlo only** (+ Radion if H2B).  
- 50+ enrolled ⇒ **Arlo + TPAC + Ryan Specialty**.  

## 6) Minimal output fields
When presenting counts, the assistant MUST output:
- EE, ES, EC, EF, W (employees only)  
- Enrolled, Eligible, Participation %  
- Predominant ZIP + top ZIPs

---

*This file is designed to be loaded as project context. It supersedes any prior informal instructions about counting.*
