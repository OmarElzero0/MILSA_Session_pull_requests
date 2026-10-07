# DSC Hex: final beta test, 7 October 2026

**Site:** https://dscportal.dsceg.org  ·  **Time box:** 2 hours  ·  **Contains passwords: do not forward outside the test team.**

Part A must pass **before the invitation emails go out**. Part B must work before Kickoff (Friday 9 October) or Week 1 (from Saturday 10 October). Part C can wait.

---

## 0. Before anyone starts (Omar)

1. Rules deployed (`npx tsx scripts/deploy-rules.ts`, read the dry run, then `--deploy`), `dev` pushed to `main`, and Vercel finished deploying.
2. **Check the new version is live.**
   - Sign in as any beta intern and open **Weekly sync**.
   - It must say *"Weekly syncs start in Week 1: your first is due by Monday 12 Oct, 23:59 Cairo"*.
   - If it does not, the old version is still live. **Stop:** testing it is wasted time.
3. In **Squads > Squad reveal**, every track is **hidden**.
4. In **AI controls > Hexa settings**, set "Meetings per 15-minute slot" to **5**. Leave "Chat questions per person per day" at **20**.
5. The **test intern** already exists (created 7 Oct, 17:59 UTC). It is a normal account, not beta, with a temporary password, exactly like the real interns'. It is in the accounts table below.
   - Only the tester who runs A2, A3 and A5 uses it, and only once: A2 replaces its password.
   - **Delete it after the beta** (Firebase console > Authentication, and its `profiles` document), before the squads are generated.

## Who tests what

| Tester | Takes | Device |
|---|---|---|
| 1 | Interns of Squad 01 and the test intern (A1-A9) | laptop, then own phone |
| 2 | Mentors: Hany, Mona, Dalia, Rania (A1, B4-B8) | laptop |
| 3 | Ops: Nour (A1, A7-A8 from the Ops side, B9-B12) | laptop |
| 4 | Phones: iPhone and Android, any intern and any mentor (A10, B1-B2) | phones |

## How to report

- Use **Report a bug** in the app: the bug icon in the header, or the account menu. It records the page, the browser and the recent errors by itself.
- Start the text with the test ID, for example `A7: Hexa did not open a ticket`.
- Add a screenshot when it helps.
- **A blocker** (nobody can sign in, data visible to the wrong person, a page that crashes): also message Omar on WhatsApp at once.
- Fill in the results table at the end.

## Known and expected (do not report)

- **Beta accounts always see their squads**, even while squads are hidden. That is deliberate. Only the test intern shows the hidden state.
- **No group calls.** Pod meetings are off, and the pitch rehearsal and interview practice are one person with Hexa.
- **Mock interviews** say "coming soon".
- The **live captions** during a call are rough and drop English words. The transcript Hexa uses is made from the recording after the call.
- Hexa's chat allows **20 questions a day** per person. A heavy tester may hit it; that message is expected.
- Before Week 1, a weekly sync is a **try-out**. The feedback goes to the intern and no squad report goes to mentors.

## Accounts

Beta squads:
- **Cluster 01**, client Masaraat Learning: Squad 01 and Squad 02. Cluster Lead **Hany**, Client Mentor **Dalia**.
- **Cluster 02**, client Rawaj Pay: Squad 03. Cluster Lead **Yasmin**, Client Mentor **Rania**.

Track Mentors:
- **Mona** (SWE): all three squads.
- **Karim** (AI): Squad 01.
- **Rania** (Flutter): Squads 02 and 03. Rania is Squad 03's own Client Mentor, so she must **never** see anything evaluative about Squad 03.

| Who | Email | Password | Role | Squad |
|---|---|---|---|---|
| Nour, Operations | `omarmohmed7659944+beta-ops@gmail.com` | `5VwE7rFLv8A7!` | operations | - |
| Hesham, partner company | `omarmohmed7659944+beta-company@gmail.com` | `kk0nrUtOiAA7!` | company_manager | - |
| Hany, Cluster Lead, cluster 01 | `omarmohmed7659944+beta-cluster-lead@gmail.com` | `j24T2VYjtqA7!` | mentor | - |
| Dalia, Client Mentor, cluster 01 | `omarmohmed7659944+beta-client-mentor@gmail.com` | `gEX4papOIFA7!` | mentor | - |
| Yasmin, Cluster Lead, cluster 02 | `omarmohmed7659944+beta-cluster-lead-2@gmail.com` | `XILuQUfaJyA7!` | mentor | - |
| Rania, Client Mentor cluster 02 + Flutter Track Mentor | `omarmohmed7659944+beta-client-mentor-2@gmail.com` | `G11AkaHGjYA7!` | mentor | - |
| Karim, Track Mentor AI | `omarmohmed7659944+beta-track-mentor@gmail.com` | `ppkHNmODyOA7!` | mentor | - |
| Mona, Track Mentor SWE | `omarmohmed7659944+beta-track-mentor-swe@gmail.com` | `NBCHtNMtZPA7!` | mentor | - |
| Mahmoud, Squad 01 team lead (SWE) | `omarmohmed7659944+beta-lead@gmail.com` | `ygZQq8sm0MA7!` | intern | 01, lead |
| Ahmed, Squad 01 deputy (AI) | `omarmohmed7659944+beta-deputy@gmail.com` | `kFul2Qj4AiA7!` | intern | 01, deputy |
| Sara, Squad 01 member (SWE) | `omarmohmed7659944+beta-member-swe@gmail.com` | `AoIF8ow7w3A7!` | intern | 01, member |
| Youssef, Squad 01 member (AI) | `omarmohmed7659944+beta-member-ai@gmail.com` | `aUzumlXqRbA7!` | intern | 01, member |
| Nada, Squad 02 team lead (Flutter) | `omarmohmed7659944+beta-lead-2@gmail.com` | `1fdIatiKR4A7!` | intern | 02, lead |
| Omar, Squad 02 deputy (SWE) | `omarmohmed7659944+beta-deputy-2@gmail.com` | `fhKfpHWcilA7!` | intern | 02, deputy |
| Hana, Squad 02 member (SWE) | `omarmohmed7659944+beta-member-2-swe@gmail.com` | `G2VIDLSS98A7!` | intern | 02, member |
| Tarek, Squad 02 member (Flutter) | `omarmohmed7659944+beta-member-2-flutter@gmail.com` | `8Xtf8kgE1QA7!` | intern | 02, member |
| Mariam, Squad 03 team lead (Data) | `omarmohmed7659944+beta-lead-3@gmail.com` | `HuWY2tFqHXA7!` | intern | 03, lead |
| Khaled, Squad 03 deputy (Cyber) | `omarmohmed7659944+beta-deputy-3@gmail.com` | `bSSaAtXcuGA7!` | intern | 03, deputy |
| Ali, Squad 03 member (SWE) | `omarmohmed7659944+beta-member-3-swe@gmail.com` | `hIjuc3Kb9pA7!` | intern | 03, member |
| Salma, Squad 03 member (Flutter) | `omarmohmed7659944+beta-member-3-flutter@gmail.com` | `ZN7qtFYu0pA7!` | intern | 03, member |
| Laila, Observer (no squad) | `omarmohmed7659944+beta-observer@gmail.com` | `eB7903Fqv6A7!` | intern, observer | - |
| Test intern (not beta, temporary password) | `omarmohmed7659944+firstlogin@gmail.com` | `6GFt-paem-tuEV` | intern | none yet |

**Do not change the beta accounts' passwords** except where a test says so (A9). Everyone shares them.

---

## Part A: must pass before the invitation emails go out

| ID | Who | Do this | Expect this |
|---|---|---|---|
| A1 | Every account, once | Sign in. | It lands on its own home, with the account's own name. **Menus:**<br>• **Intern:** Home, Calendar, My squad, Client, Meet Hexa, Weekly sync, Curriculum.<br>• **Observer (Laila):** no My squad and no Weekly sync.<br>• **Mentor:** Home, Calendar, My squads, Hexa reports, Clients. Mona and Karim also have Task reviews. Dalia alone sees **Hexa briefs** instead of Hexa reports.<br>• **Ops:** Overview, Calendar, People, Squads, Tasks, Tickets, Announcements, Clients, Hexa reports, AI controls, Knowledge base, Audit log.<br>• **Partner company:** Clients and Calendar only. |
| A2 | Test intern | Sign in with the temporary password. | **"Set your own password"** opens before anything else:<br>• A wrong temporary password is refused.<br>• Reusing the temporary password as the new one is refused.<br>• After saving a new password, DSC Hex opens and the tour starts.<br>• Sign out: the temporary password no longer works, the new one does. |
| A3 | Test intern | Sign out. On the sign-in page, use **Forgot password?** with the test intern's email. | A reset email reaches Omar's inbox within a few minutes. **Write down the sender, and whether it landed in spam.** The link sets a new password, and signing in with it works. |
| A4 | Test intern, on a phone | The tour after the first sign-in. | The tour walks through each page with a card. **Skip** works. **Platform tour** in the menu starts it again. Nothing is cut off on the phone. |
| A5 | Test intern | Open **My squad** and **Client**. | Squads are not revealed yet: a message says they are revealed at Kickoff. **No names** of other interns are visible anywhere. The client directory lists the companies, with no "Your client" badge. |
| A6 | Sara (member) | Try every menu item and the bell. | Sara sees only her own things. No Hexa reports, no People, no other squad's feedback, no mentor pages. |
| A7 | Sara | Open the Hexa chat (bottom corner). Ask, in order:<br>1. "When is Demo Day?"<br>2. A question in Arabic about Consolidation Week.<br>3. A code question.<br>4. "I need a deadline extension because I'm sick, please tell the team". | 1. The answer is 4 December.<br>2. A correct answer.<br>3. A helpful answer, with **no ticket**.<br>4. Hexa says it sent this to the team and does **not** ask her to fill in a form. The ticket appears under **Your tickets**.<br>The chat shows how many **questions left today**. |
| A8 | Nour (Ops), then Sara | Nour opens **Tickets**, opens Sara's ticket, sets *In progress*, writes a reply, then sets *Resolved*. Sara reopens the chat > **Your tickets**. | Nour sees Sara's name, track and squad, and Hexa's summary. Sara sees the reply and the status. |
| A9 | Youssef (member) | 1. **Report a bug** with a short text and a screenshot.<br>2. **Profile**: add a photo; set a GitHub username; try to change the track; change the password, then **change it back to the one in this file**. | 1. "Sent" shows. Nour sees it in **Tickets**, with the page, the browser and the screenshot.<br>2. The photo and username save. The **track cannot be changed**. Both password changes work. |
| A10 | Tester 4, iPhone and Android | Sign in as an intern and as a mentor. Open every page, the chat, the bug dialog and the tour. | No page scrolls sideways, buttons can be tapped, the chat opens and closes, and dark mode is readable. |

**Go / no-go for the emails:** A1 to A10 pass, or every failure is understood and accepted by Omar.

---

## Part B: must work before Kickoff or in Week 1 (fine after the emails)

| ID | Who | Do this | Expect this |
|---|---|---|---|
| B1 | Ali (member), laptop with a mic | **Weekly sync > Start now**. Talk for 3 to 5 minutes in mixed Arabic and English: what you "did" this week, one blocker, one question. Claim one thing that is not true, e.g. "my PR #77 is merged". Then **End meeting**. | Hexa greets Ali by name and already knows his squad and track (it does not ask). It answers or defers the question.<br>After the call: *"Your feedback is on your Weekly sync page"*. The page shows **Your try-out sync is done**, with feedback that matches what he said.<br>**Check:** nothing invented. The fake PR is **not** praised as done. |
| B2 | Salma (member), on a phone | The same as B1, by voice on the phone. | It works on the phone. Note the sound quality and any drop. |
| B3 | Khaled (deputy) | **Weekly sync > Write it instead**. Answer Hexa's questions in writing. | It ends with feedback, the same as B1. |
| B4 | Mona, Karim, Hany, Dalia, Rania | After B1-B3, check the bell and **Hexa reports**. | **No "weekly report"** for Week 0: try-outs are not combined. If Ali raised something urgent, Mona alone may get it. Nothing reaches Rania or Dalia. |
| B5 | Sara hands in, Mona reviews | **Curriculum**: open a lesson and hand in its task, with a GitHub link and a note. Mona: **Task reviews** > ask for changes, with a comment. | Sara gets a notification. The lesson shows *changes requested* and Mona's comment. Karim (AI) does **not** see Sara's SWE task. |
| B6 | Mahmoud (lead), then Ahmed (deputy) | 1. Mahmoud: **Weekly sync** > set the squad repository (a public github.com repository link) and confirm.<br>2. Ahmed: look for the same option. | 1. It saves and then cannot be edited.<br>2. Ahmed cannot set it. |
| B7 | Mahmoud | **Meet Hexa** > **Pitch rehearsal** alone, laptop, share slides (any deck). | Hexa listens, asks client-style questions about the slides, then coaches. Hany (Cluster Lead) gets the feedback. Dalia's brief **names nobody**. |
| B8 | Hany, then Dalia, Mona and Sara | Hany leaves three notes on Squad 01: "Cluster Lead only", "Cluster Lead and Track Mentors", "Everyone". | Each person sees exactly the notes meant for them:<br>• Dalia sees only "Everyone".<br>• Mona sees the last two.<br>• Sara sees only "Everyone". |
| B9 | Nour (Ops) | **Announcements**: tick **Beta-test accounts only**, audience Interns + Software Engineering. Preview, then send. | The preview count matches the beta SWE interns. Only they get the notification; Karim and Ahmed (AI) do not. |
| B10 | Nour | **Squads** > open BETA Squad 01 > **Edit squad**. Look at people, pods, Track Mentors and **Weekly sync deadline**. Set the deadline to Tuesday and save. | The squad's details are all there. It saves, and Weekly sync for Squad 01's interns now says Tuesday. **Set it back to Monday.** Do not edit any non-beta squad. |
| B11 | Nour | **AI controls**: read every setting. Save without changes. | Nothing errors. The settings Omar set in step 0 are there. |
| B12 | Everyone | **Calendar** on laptop and phone. | Kickoff 9 Oct, Week 1 from 10 Oct, Demo Day 4 Dec, and your own role's weekly rhythm. The .ics download opens in a calendar app. |

---

## Part C: can wait until after Kickoff

- Combined weekly squad report after the first real deadline (Monday 12 Oct): Hany, Mona and Dalia each get their own version.
- Interview practice for the leads.
- Friday digest for Track Mentors.
- Gate operations (due 23 Oct).
- Observer flows.
- Audit log.

---

## Results

| ID | Tester | Pass / fail | What happened (if it failed) |
|---|---|---|---|
| A1 | | | |
| A2 | | | |
| A3 | | | |
| A4 | | | |
| A5 | | | |
| A6 | | | |
| A7 | | | |
| A8 | | | |
| A9 | | | |
| A10 | | | |
| B1 | | | |
| B2 | | | |
| B3 | | | |
| B4 | | | |
| B5 | | | |
| B6 | | | |
| B7 | | | |
| B8 | | | |
| B9 | | | |
| B10 | | | |
| B11 | | | |
| B12 | | | |
