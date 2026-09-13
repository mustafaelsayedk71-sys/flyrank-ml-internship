# General AI Fluency Track Retrospective

**Author:** Mustafa Elsayed  
**Word Count:** ~600 words  

---

## 1. Initial Expectations vs. Evolution
Entering Week 1 of this track, my primary focus was exploring basic prompt engineering and isolated code generation. Over the eight-week trajectory, my perspective evolved from treating AI as a conversational assistant to utilizing it as an engineering co-pilot and system auditor. 

The transition became evident during the site-hardening phase (Week 7) and capstone model design (Week 8). Instead of relying on happy-path demonstrations, I learned to systematically stress-test systems—evaluating double submissions, empty payload edge cases, and cross-validation data leakage across domain groups.

---

## 2. Key Architecture & Design Decisions
A critical design decision made during the capstone build was implementing `GroupKFold` cross-validation instead of standard random splits. Standard random splits allowed domain-specific patterns to leak between training and validation sets, artificially inflating accuracy metrics. Restricting validation splits by domain hash created an honest benchmark, reducing true prediction error (MAE) by 36.5% against baseline heuristics.

On the frontend, trading over-engineered frameworks for clean, static HTML/CSS with light JavaScript state handling ensured maximum reliability, rapid load times, and effortless HTTPS deployment on GitHub Pages.

---

## 3. What I Would Build Next
If extending this system for another production iteration, I would implement:
1. **Automated Pipeline Re-training:** Dynamic trigger functions that execute weekly model re-evaluations whenever search impression decay logs update.
2. **Real-Time Webhooks:** Instant Slack/Discord alerts notifying editorial teams when high-traffic pages hit the `PRIORITY_REFRESH` threshold.

---

## 4. Top 3 Transferable Skills Learned
1. **Edge-Case Diligence:** The practice of intentionally trying to break my own software before deployment, identifying fix-now issues vs. documented known limitations.
2. **Leakage-Free Validation:** Structuring machine learning data splits around logical grouping variables to prevent optimistic performance bias.
3. **Transparent AI Co-Creation:** Documenting exact boundaries of AI utility while verifying critical business logic manually to maintain complete technical accountability.
