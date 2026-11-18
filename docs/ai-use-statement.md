# AI Use Statement

**Project:** Chef-Mate – a web app that turns food already in the fridge into recipes before it expires
**Course:** Introduction to Software Engineering (15031001)
**Team:** Hallo world (Team 22)
**Repository:** https://github.com/Zqmarxn/Chef-Mate-

---

## 1. Purpose of This Statement

This document transparently discloses how the team **Hallo world** used generative AI tools during the key stages M1, M2 and M3, including the human verification and engineering controls applied to every AI-assisted work product.

---

## 2. AI Tools Used

- **Anthropic Claude:** Used across M1 to M3 to help refine requirements wording, check consistency between the M1 charter, the M2 SRS and the prototype, and help organize and debug the single-file HTML/CSS/JS prototype. In M3 it was also used to draft this AI use statement and the final report, modeled on the structure of another team's published example; the team supplied and checked all project facts.

---

## 3. Chronological AI Usage Log (Month 1 – Month 3)

| Milestone & Date | AI Tool | What We Asked | What AI Produced | Human Verification & Changes Made |
|---|---|---|---|---|
| M1 / M2<br>Month 1–2 | Claude | Help structure and tighten the problem statement, scope and SRS wording (functional requirements, non-functional requirements, use cases) | Draft wording and structure for the SRS sections | Team compared the draft with its own user findings, removed out-of-scope items and kept only requirements it agreed with |
| M2 / M3<br>Month 2–3 | Claude | Check the prototype against the M1 charter and the M2 SRS | A list of mismatches between the prototype and the documents | Team reviewed each proposed change and applied only the ones it approved |
| Implementation & M3 testing<br>Month 3 | Claude | Help organize the HTML/CSS/JS prototype: fridge and expiry tracking, recipe filtering, shopping list, cooking timer, Thai/English switch | Code suggestions and fixes for the single-file prototype | Team opened the prototype in a browser, tested each user flow and fixed issues before submitting |
| M3 documentation<br>Month 3 | Claude | Draft the AI use statement and final report in English, modeled on another team's example | Markdown drafts of both documents | Team replaced all project facts (names, requirements, features) with its own and checked them against M1 and M2 |

---

## 4. Human Verification and Engineering Controls

1. **Clear separation between the prototype and planned AI features:** All documents and UI labels clearly distinguish what the M3 prototype does in the browser from what is out of scope for a future release.
2. **End-to-end testing:** Every AI-suggested code section and SRS status description was verified by opening the HTML prototype directly in a web browser and walking through all user flows (FR-1 to FR-[n]).
3. **Team accountability:** Every member of team **Hallo world** reviewed the repository changes, requirements traceability and code modules related to their own responsibility, in preparation for the individual oral exam.

---

## 5. Sample Prompts Used

- **Requirements and scope check:** *"Check this prototype against our M1 charter and M2 SRS, list any mismatches, and suggest wording so the SRS matches what the prototype really does."*
- **Prototype logic:** *"Help me organize a single-file HTML/CSS/JS prototype for a fridge-to-recipe app: add ingredients with days left before expiry, highlight items close to expiring, filter recipes by expiring items, and add a Thai/English switch."*
- **Documentation:** *"Write an English AI use statement for our project in the same structure as this Thai example."*
