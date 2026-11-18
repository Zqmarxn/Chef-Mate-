# Project Final Report: Chef-Mate

**Course:** Introduction to Software Engineering (15031001)
**Team:** Hallo world (Team 22)
**Repository:** https://github.com/Zqmarxn/Chef-Mate-
**SDLC approach:** Agile (Scrum-style iterations across Milestones M1 to M3)

---

## 1. Team Members

| Student ID | Full Name |
|---|---|
| `6931503070` | Woranat Duangmano |
| `6931503067` | Rattasard Khamlid |
| `6931503056` | Patsu Namphungmongkhonsakun |
| `6931503039` | Thanakrit Kosintorn |

---

## 2. Problem Definition and User Validation (M1 Foundation)

- **Problem:** People who buy fresh food in small, frequent amounts often cannot work out what to cook with what they already have. Items at the back of the fridge are forgotten and thrown away, and the person buys more. Recipe apps start from a dish and assume you will go shopping; none starts from the contents of your fridge and its expiry dates.
- **User validation:** The problem and the target users were defined and checked with users in Milestone 1 (see `M1 Team Charter-chef_mate.pdf`), and the resulting requirements were written up in the M2 SRS (`Team22_M2_SRS.pdf`).
- **Solution overview:** Chef-Mate is a web app that turns food already in the fridge into recipes before it expires. Users record the ingredients in their fridge with the days left before expiry, get an alert for items close to expiring, and can jump straight to recipes that rescue them. The prototype also has a shopping list, step-by-step cooking with a timer, cooking history, daily quests, and a Thai/English language switch.

---

## 3. Golden Thread Traceability Matrix (M1 → M2 → M3)

Each functional requirement (FR-1 to FR-5) and use case (UC-1 to UC-5) links from a user pain point to a clickable feature in the M3 prototype:

| FR & Use Case | User Pain Point | Prototype Implementation (current M3) | AI Rollout Plan (future scope) |
|---|---|---|---|
| **FR-1 / UC-1**<br>Add food to the fridge with days left before expiry | Items at the back of the fridge are forgotten | Fridge tab: add-item form with an expiry (days) field. Items are stored in the browser with `localStorage` | Scan receipts or photos to add items automatically |
| **FR-2 / UC-2**<br>See items close to expiry | Users do not notice food is about to expire | An expiry alert banner lists expiring ingredients as chips, and the fridge has an "expiring" filter with a live count | Smart reminders based on each food type's typical shelf life |
| **FR-3 / UC-3**<br>Get recipes from what is in the fridge | Recipe apps start from a dish, not from the fridge | Recipes tab with a "rescue expiring items" filter and a one-tap button that picks a menu from expiring ingredients | AI-generated recipes from the fridge contents |
| **FR-4 / UC-4**<br>Shopping list for missing ingredients | Users buy duplicates or forget what is missing | Shopping tab: add missing ingredients from a recipe and check items off | Auto-built lists from planned meals |
| **FR-5 / UC-5**<br>Bilingual interface (Thai / English) | Language barriers for Thai and international users | A language switch updates labels and messages across the app using pre-translated text | More languages, AI-translated recipes |

---

## 4. Non-Functional Requirements (NFR) Summary

- **NFR-1 (Performance):** The prototype is a single standalone HTML file (about 0.4 MB) designed to load and render within 3.0 seconds; check with the Chrome DevTools Network tab.
- **NFR-2 (Localization):** Every screen shown to the user, including the login and fridge screens, is available in both Thai and English through the language switch.
- **NFR-3 (Usability):** A new user should be able to add an ingredient and find a recipe that uses it within 45 seconds without a manual; evaluate with a timed test of new participants.
- **NFR-4 (Compatibility):** The interface is responsive (mobile viewport) and runs in a modern web browser with no installation.
- **NFR-5 (Security & Privacy):** The client-side prototype keeps only app data and settings in the browser's `localStorage`. It makes no calls to external APIs, and the Google sign-in screen is a simulated account picker.

---

## 5. Explicitly Out of Scope

The following are intentionally excluded from the M3 prototype:

1. Real Google OAuth sign-in and cloud account storage (the sign-in screen is simulated)
2. Real-time AI recipe generation or image recognition through an external API
3. Online grocery ordering, payment gateways and e-commerce transactions
4. Social features such as messaging or sharing between users

---

## 6. How to Use the Prototype

1. Clone the repository:
   ```bash
   git clone https://github.com/Zqmarxn/Chef-Mate-.git
   ```
2. Open the `prototype` folder.
3. Open `chef_mate_redesign-3.html` in a web browser (no installation or server required). It needs an internet connection only for the web fonts.
4. Suggested test flow: sign in with the simulated Google account picker → add an ingredient with 1 to 2 days left → see the expiry alert → tap the rescue button to view matching recipes → start cooking and use the timer → add a missing ingredient to the shopping list → switch the language between Thai and English.

---

## 7. AI Use

See [ai-use-statement.md](ai-use-statement.md).
