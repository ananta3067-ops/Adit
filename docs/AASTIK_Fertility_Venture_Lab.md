---
title: "Aastik Fertility: Venture Lab Simulation (Parts 1–7)"
date: 23 November 2026
prepared_for: Dr. Aditya Soni, Founder, Aastik Ayurveda Pvt. Ltd.
status: Working draft for investor-grade challenge. Not legal, tax or clinical advice.
---

# Aastik Fertility: Venture Lab Simulation

**Prepared:** 23 Nov 2026. **Roles simulated:** VC Investment Committee, healthcare entrepreneur, CFO, Chief Growth Officer, market researcher, operations consultant, regulatory researcher, sceptical investment banker.

---

## 0. Read this first

### 0.1 What I could and could not inspect

**Update, 23 Nov 2026 (second pass):** a dedicated network environment was created to reach these sites. Results:

| Asset / source | Status | Consequence |
|---|---|---|
| Google Maps listing (`maps.app.goo.gl/WmjLY88Hthatshca6`) | **Partly accessed.** Google serves only its "limited view" to a signed-out cloud browser: name, rating, category, address, hours, phone, website and the latest owner post. The **review count and review texts are hidden** without sign-in. | Facts in 1.2. **I have still not read any individual review.** The 30–50 review analysis needs a Business Profile export or a signed-in screenshot set. |
| Instagram `@aastikayurveda` | **Not accessed.** Every signed-out request is redirected to the login page. I did not try to bypass the login. | No follower, post or engagement data. 1.3 stays a framework. |
| YouTube patient story (`_pVvoGZpF7Y`) | **Metadata only.** The oEmbed endpoint gave the title and channel. The watch page returned Google's bot-check page to this cloud IP, so I could not get the description, view count or transcript. A permission check also stopped a call to YouTube's internal player API. | Title: **"The Child We Prayed For: A Blind Couple's Journey with Ayurveda"**, channel `@aastikayurveda`. I have **not** watched it. See 1.4. |
| aastikayurveda.com (linked from Maps) | **Accessed** (8 pages) | New 1.2A, with **one critical security finding**. |
| gynoveda.com | **Accessed directly** (home, clinics, Pune clinics, how-it-works, product, refund policy, IVF comparison, about) | 4.1 rewritten from first-hand page text. |
| Earlier Aastik documents in this repo | Read | Founder background and clinic location only. **Aastik Fertility is a separate business** from the curcumin venture (see 0.4). |
| Web search (press, regulators, PubMed, NABH, listings) | Accessed | Everything else in this report. |

To complete Part 1 properly, I need one of the following: (a) a network allowance for those hosts, or (b) you paste in a Google Business Profile export, Instagram Insights screenshots for the last 90 days, and the YouTube video's transcript plus its Studio analytics. Either takes about 30 minutes.

### 0.2 The verdict in one table

| Question | Answer |
|---|---|
| Is "Aastik Fertility" investable **today** at ₹10 Cr? | **No.** There is no fertility-specific revenue, no outcome data and no proof of acquisition cost, and the clinic it would pilot in is only about 9 months old. Raise after the pilot gate (Section 9.3), into a new entity (0.4). |
| Is it worth a **₹12–18 lakh pilot inside the Katraj clinic**? | **Yes**, under the conditions below. The downside is small, and the data it produces is what makes the business financeable later. |
| Best initial wedge | **Neither "body detox" nor IVF support.** Start with a **time-boxed couple programme for couples trying to conceive (TTC) for 6–24 months**, with the woman under 35 and no absolute indication for IVF. Run it with **mandatory diagnostics, male-partner evaluation and a hard referral clock.** Preconception care for couples not yet trying becomes the lower-priced, content-led entry tier. |
| Your ₹1.0 L / ₹1.5 L prices | **₹1.5 L for Ayurveda-led infertility support fails** against a ₹1.0–1.8 L IVF cycle and a ₹18–48 k Gynoveda kit. Recommended prices: **₹39 k (3-month), ₹79 k (6-month) and ₹1.25 L (Signature, high-touch).** |
| 5–10 bed hospital first? | **No.** Fertility care does not need beds. Indian health insurance generally **excludes infertility treatment**, so beds do not unlock reimbursement. Model C means ₹1.8–3 Cr of capex for no demand advantage. |
| NABH | Start with **NABH Entry-Level Ayush Centre certification** (OPD, about ₹11 k + GST per the NABH FAQ; verify the current fee). Move to the **Ayush Treatment & Wellness Centre standards (effective 1 Apr 2025)** later. NABH is a quality mark. It does **not** authorise any service. |
| Defensible advantage | Gynoveda, a local gynaecologist and an IVF chain each lack the same four things: **(1) couple-level care, with male factor treated as half the problem; (2) an in-person Ayurveda procedure capability; (3) a published, denominator-based outcomes registry; (4) an enforced, IVF-friendly referral clock that turns gynaecologists and IVF centres into referrers rather than enemies.** |
| ₹1,000 Cr enterprise value | **Not credible within 5 years.** At a 5× revenue multiple it needs about ₹200 Cr revenue. The best-funded Ayurveda fertility player, Gynoveda, reported about ₹67 Cr revenue and a ₹3 Cr loss in FY24 after a $10 M Series A. A credible 3-year milestone is **₹10–15 Cr revenue with published outcomes**, which supports roughly a ₹60–120 Cr valuation. Section 8 has the long-path math. |

### 0.3 Investment Committee: reasons to reject (stated plainly)

1. **Founder bandwidth.** Aastik Fertility is a separate company, but the founder still runs the Aastik Ayurveda clinic and the products business. Investors will ask who works full-time on Aastik Fertility. The answer has to be a named founder or CEO with time committed in writing.
2. **No base to scale from.** The clinic is about 9 months old and turns over about ₹2 L a month (unverified). Nothing yet proves that Aastik can acquire fertility patients at a viable cost.
3. **Evidence is thin.** The Ayurveda infertility literature is mostly small, single-arm and unblinded (Section 2.4). Every marketing claim will have to be modest.
4. **The law restricts advertising.** The Drugs & Magic Remedies (Objectionable Advertisements) Act 1954 schedules **"sterility in women"** and **"sexual impotence"**. You cannot advertise a drug as a remedy for them. Acquisition therefore has to be built on education, referrals and services, which is slower than Gynoveda-style performance ads.
5. **Strong incumbents.** Gynoveda has capital, brand, ads, 50+ clinics and **3 Pune clinics, one in Kondhwa about 4–5 km from Katraj**, with a ₹2,000 couple consultation (gynoveda.com, 23 Nov 2026). Indira IVF reports 165+ centres, including 7 in Pune with one in Baner. Nova and Oasis run clinics in Kondhwa/Lulla Nagar, about 5–8 km from Katraj.
6. **Founder dependency.** Delivery currently rests on one MD.
7. **Asymmetric harm.** Delaying IVF for a 37-year-old woman with low AMH is a real clinical and reputational risk. A single public case can damage the brand.

**What would flip the IC to "invest":** 50 or more enrolled couples, under 15% refunds or drop-outs, audited CAC below 20% of ticket, a published 6-month outcome report, and at least 5 active gynaecologist or IVF referral partners. Sections 8–9 set this out as a 9-month gate.

### 0.4 Entity structure: Aastik Fertility is a separate business

The founder's instruction (23 Nov 2026): **Aastik Fertility is entirely separate from the curcumin venture.** It gets its own entity, its own investors and its own pitch.

| Item | Recommendation |
|---|---|
| Legal form | **Private Limited Company, not an LLP**, if you plan to raise equity. Indian VCs and angel networks invest through equity or CCPS (compulsorily convertible preference shares) in a company. LLPs cannot issue shares or ESOPs, and foreign investment into LLPs has extra conditions. An LLP suits only a two- or three-doctor partnership that will never raise money. |
| Name | e.g. "Aastik Fertility Pvt Ltd" or a distinct brand. Run trademark searches in classes 44 (medical services) and 5 (medicines) first. |
| Relationship with Aastik Ayurveda Pvt Ltd | Written, arm's-length agreements: (1) a **brand licence** (or a fully distinct brand); (2) a **supply agreement** for medicines at a documented transfer price; (3) a **sublease or service agreement** for using the Katraj clinic and therapy rooms. Investors will treat every one of these as a related-party transaction to diligence. |
| Founder | DPIIT startup recognition for the new entity. Founder shares with 4-year vesting and a 1-year cliff (investors will ask). Reserve a 10% ESOP pool for a second doctor, a clinic head and a growth lead. |
| Clinical licences | They follow the entity: establishment registration, biomedical waste authorisation and NABH entry-level certification in the new company's name once it runs the service. |

---

## PART 1 — EXISTING BUSINESS AND ASSET AUDIT

### 1.1 What is known

| Item | Status |
|---|---|
| Entity | Aastik Ayurveda Pvt. Ltd. |
| Founder | MD Ayurveda (Rasa Shastra & Bhaishajya Kalpana). This is pharmaceutics, not Prasuti Tantra/Stree Roga, which matters for clinical credibility (see 1.6). |
| Centre | **Aastik Ayurveda & Panchakarma Centre (आस्तिक आयुर्वेद & पंचकर्म सेंटर), ISKCON NVCC Temple Campus, Tilekar Nagar, Katraj, Pune 411048** (Plus code CVXJ+F8). Confirmed from the Google Maps listing. |
| Operating since | Feb 2026 |
| Revenue | ~₹2 L/month (unverified, user-supplied) |
| Existing product capability | Nine licensed SKUs and formulation expertise (from the earlier playbook). This is a real **cost advantage on medicines**, which are the largest direct cost line in every package below. |

### 1.2 Google Maps listing

**What the listing shows** (Google's limited signed-out view, accessed 23 Nov 2026):

| Field | Value | Comment |
|---|---|---|
| Name | Aastik Ayurveda & Panchakarma Centre / आस्तिक आयुर्वेद & पंचकर्म सेंटर | Good: the bilingual name helps local search |
| Rating | **4.9★** | Strong. The review count is hidden in the limited view, so it is unknown. |
| Category | **"Alternative medicine practitioner"** | **Weak.** Change the primary category to "Ayurvedic clinic" and add "Panchakarma centre" as secondary. The "alternative medicine" label hurts credibility with gynaecologists and premium patients. |
| Address | ISKCON NVCC Temple Campus, Tilekar Nagar, Katraj, Pune 411048 | The temple campus is a strong landmark and trust signal for one audience, and neutral or negative for a secular, cosmopolitan one (see 7.5) |
| Hours | Opens 9:30 AM (shown on a Monday, "Opens Tue"), so **closed on Mondays** | Fine. Fertility couples will want evening and Sunday slots. |
| Contact | +91 70572 05677, a WhatsApp link, aastikayurveda.com | Good: WhatsApp is the right conversion path |
| Latest owner post | "Take a break from daily stress… relaxation, better sleep, mental peace, overall wellness", posted 9 hours before access | Active posting, but **wellness/relaxation positioning, not clinical** |
| Photos | A photos section exists; count not visible | |

**Still needed** (export it, or take screenshots while signed in): review count, star distribution, the latest 30–50 reviews, owner reply rate, and photo count. Use the template below.

| Metric | Value | Benchmark to compare against |
|---|---|---|
| Rating / review count | _?_ | Oasis Fertility Kondhwa shows **4.9 from 756 reviews** (Oasis website, accessed Nov 2026). IVF chains routinely carry 500–3,000 reviews per centre. |
| Review distribution (5★…1★) | _?_ | Over 10% one- and two-star reviews is a red flag. |
| Reviews mentioning fertility, PCOS or conception | _count?_ | This is the real test of whether the listing helps a fertility launch. |
| Reviews in the last 90 days | _?_ | Velocity matters more than the total. |
| Owner reply rate | _?_ | Target 100% within 48 h. |
| Primary category | _?_ | Should read "Ayurvedic clinic". Do **not** switch to "Fertility clinic" until the service exists and is compliant. |
| Photos (owner / visitor) | _?_ | You need a clean procedure room, the doctor's face, consult room, reception and exterior. |
| Services listed | _?_ | Remove any disease-cure wording. |

**Review coding.** Tag each review on Doctor explanation, Results, Therapist skill, Cleanliness, Waiting time, Price/value, Staff behaviour and Follow-up. Count positive and negative mentions per tag. The two tags that predict fertility conversion are **doctor explanation** and **follow-up**.

**Benchmark that matters most:** Gynoveda's **Kondhwa clinic (Lulla Nagar, 99 Avenue Complex)** is about 4–5 km from your centre. Its listing shows **4.8★**, and the brand shows **4.7★ across 27,433+ Google reviews** (gynoveda.com, accessed 23 Nov 2026). Your 4.9★ competes on quality, not volume.

### 1.2A Website audit: aastikayurveda.com (accessed 23 Nov 2026)

| Finding | Severity | Detail | Fix |
|---|---|---|---|
| **The blog is full of casino/gambling spam** | **CRITICAL, fix this week** | All 12 posts visible on `/blog/` are online-casino articles in Croatian, Greek, Swedish, Dutch, Turkish and English (e.g. "Unlocking Profit: Discover the Most Lucrative Casino Games Today", "Discover the Exciting World of Amazon Slots UK"). All are attributed to the author account "Sneha Loni", with no Ayurveda content. This usually means a **compromised WordPress account or plugin, or a paid-link injection**. | (1) Take the blog offline. (2) Have the developer (footer: "Yuvmedia") audit admin users, reset all passwords, enable 2FA, update or remove plugins, and scan for injected code. (3) Delete the spam posts and request removal in Google Search Console. (4) Confirm whether "Sneha Loni" is a real team member whose account was taken over. Until it is clean, **no gynaecologist, investor or premium couple should be sent to this site**, and Google may down-rank or flag it. |
| Inconsistent trust numbers | High | The homepage claims "**10,000+ Patients**", "4.9/5 Rating" and "**⭐ 5.0+ Patient Reviews**" (a meaningless figure), while the animated counters render as "**0+ Years Experience / 0+ Patients Treated / 0+ Products**". The centre opened in Feb 2026. | If 10,000+ is a career total, say "Dr. Soni has treated 10,000+ patients across his career". Otherwise remove it. Fix the counters. Use the live Google review count. An unverifiable number is a consumer-protection risk (CCPA misleading-ad guidelines). |
| "Evidence-Based Ayurveda" positioning | Positive, if substantiated | The hero says "Evidence-Based Ayurveda for Modern Healthcare", with DPIIT-recognised startup and IIT Delhi alumni badges. Real clinical practice. | This is the right brand promise for Aastik Fertility, but it **must be backed by an outcomes page**. Today the site has none. |
| Fertility already listed | Opportunity | Clinical protocols list "**PCOS & Women's Hormonal Health**" and "**Male Fertility & Reproductive Health**"; the ticker shows "MALE FERTILITY"; the shop sells **LEUCOJIT® (women's health)**. | Fertility is a natural extension of the existing brand, which supports the endorsed sub-brand approach (1.3). |
| Claim wording | Medium | Therapy copy uses "**deep detoxification and systemic rejuvenation**" (Abhyanga) and "**Detoxifying** decoction-based therapy" (Niruha Basti). Shop product names pair with diseases ("Hyperacidity & Gastritis", "Constipation", "Immunity & Viral Fever Support"). | Replace "detoxification" with classical terms plus a neutral description. Check SKU disease wording against the DMR Act and the product licences. |
| No prices for therapies | Medium | Every therapy uses "ENQUIRE NOW" | For a premium fertility programme, publish package prices. Transparency is a differentiator against Gynoveda's "call us". |
| Team | Positive / gap | Dr. Aditya Soni (BAMS, MD Ayurveda; interests: Panchakarma, gut, lifestyle disease); Dr. Nachiket Patil and Dr. Hema B. C. (both MD Manasa Roga, pursuing). Advisory council (IGAC): Dr. Amit Deshpande (Agnivesh Healthcare, WHO-GMP), Dr. Suhas Shetty (Principal, KLE Ayurveda College, Belgaum), Dr. Soumya Basu, Dr. Pavel Peresypkin. | **No Prasuti Tantra/Stree Roga specialist and no OBG.** Confirms the gap in 1.6. The two counsellors (Manasa Roga) are a real asset for the stress and counselling component of the fertility programme. |
| Religious framing | Note | The Therapies page opens with a Radha–Krishna shloka; the Contact page says "Visit Our Sanctuary… serene spiritual ambiance of ISKCON NVCC". | Authentic for the current audience. Keep the Aastik Fertility pages clinically neutral (7.5). |
| Product pricing | Info | 9 SKUs at ₹210–360 per pack (e.g. VAJRAORTHO™ ₹360/30 tablets) | Confirms low-cost in-house medicines, which supports the medicine cost assumptions in 5.1 |

### 1.3 Instagram: audit framework (data not accessed)

| Dimension | What to measure (last 20 posts and top 5 ever) | Fertility-readiness test |
|---|---|---|
| Followers / reach | Followers, 30-day accounts reached, % non-followers reached | Under 2 k followers is not an asset. It is a starting point. |
| Format | Reels vs. static vs. carousel, and median views per reel | Fertility education works on reels and carousels. |
| Founder visibility | % of posts with the doctor on camera | Fertility buyers buy the doctor. Target over 50%. |
| Content mix | Pain/Panchakarma/general wellness vs. women's health | If under 10% is women's or reproductive health, the account does not yet carry fertility credibility. |
| Trust signals | Credentials, procedure hygiene, consent-backed stories | |
| Conversion paths | Link in bio, WhatsApp CTA, booking flow | |
| Risky content | Any "cure", "guaranteed", "detox" or disease-claim wording | Clean these up before a fertility launch draws scrutiny. |

**Brand recommendation (independent of the data):** create **a separate sub-brand handle, "Aastik Fertility" or "Aastik Conception Clinic"**, endorsed by and linked from `@aastikayurveda`.

- A general Panchakarma and pain audience is not a fertility audience.
- Fertility patients value discretion. Many will not follow a public account but will save posts and DM.
- It isolates regulatory risk: fertility content needs stricter claim review.
- Keep **one Google listing and one legal entity**. The split is in brand communication only.

**Content-gap list** (likely gaps; confirm against the account):

1. Male-factor education. Most Indian fertility content ignores men.
2. "When to see an IVF specialist" content. This counter-intuitive, trust-building content gets gynaecologists to refer.
3. The diagnostic pathway explained: AMH, semen analysis to WHO 6th edition, HSG, thyroid, prolactin.
4. A procedure-room hygiene tour.
5. Founder-to-camera myth-busting: what Ayurveda can and cannot do.
6. Outcome transparency posts, once data exists.
7. Couple-together content: diet, sleep, stress, alcohol and smoking (this is where the evidence is strongest).

### 1.4 YouTube patient story: assessment protocol (title only; video not watched)

**Retrieved:** title **"The Child We Prayed For: A Blind Couple's Journey with Ayurveda"**, channel `@aastikayurveda` (YouTube oEmbed, 23 Nov 2026). The description, views, duration and transcript were not retrievable.

**What the title implies, and why it needs care:** your brief says not to present the story as proof that Aastik can "prevent inherited conditions". Together with a title about a **blind couple**, that suggests the video may imply Ayurveda helped them have a **sighted child**, or influenced whether a hereditary condition was passed on. If so, this is the highest-risk claim in the whole business:
- Whether a child inherits a condition depends on the genetics of that specific condition (many causes of blindness are not hereditary at all). **No Ayurvedic preconception care has been shown to change genetic transmission.**
- It also involves **disability-sensitive representation**. Frame the couple's courage and parenthood, not "overcoming" blindness through treatment.
- The safe framing: "A couple's journey to parenthood, and how we supported them". Do not claim a link between the intervention and the child's health status. Add an on-screen disclaimer, and have a genetic counsellor or OBG review it if inheritance is mentioned at all.

Apply these tests before using it anywhere:

| Test | Rule |
|---|---|
| Testimonial vs. evidence | One story is **never** evidence of efficacy. It shows only that one couple was satisfied. |
| Inherited-condition claims | **No Ayurvedic intervention has been shown to prevent a genetic or inherited disorder.** Classical *beeja dosha* concepts are not evidence. Garbh Sanskar groups claiming "gene repair" or "customised babies" have faced public scientific criticism and a High Court challenge (Kolkata, 2017). Any such implication must be removed or explicitly disclaimed. |
| Sex-selection signals | Any hint of influencing the baby's sex is a **criminal-risk area under the PCPNDT Act**, which covers pre-conception sex selection and its advertisement. Avoid products and messages associated with "son" outcomes. |
| Claims about drugs | Under the DMR Act, the video cannot advertise a medicine as a remedy for female sterility or impotence. |
| Consent | A written, specific, revocable consent covering platform, duration, identifiability and right to withdraw. Under the **DPDP Act 2023 and its Rules**, health data is personal data, so consent must be free, specific, informed and withdrawable. |
| Documentation | Keep the case file: baseline investigations, interventions with dates, other treatments taken (letrozole, IUI and so on), pregnancy confirmation, and outcome. If the couple also used allopathic treatment, the story must say so. |
| Professional conversion | Re-cut as **"A couple's journey"**: their problem in their words, what the work-up found, the shared plan with the gynaecologist, the experience, and the outcome stated with "individual results vary; this is not typical or guaranteed". Have a doctor explain the pathway, not the outcome. |

### 1.5 Asset scorecard (score only after the data is collected)

Scale 1–5. Pre-filled entries are **my prior expectations, not observations**, flagged "E".

| Asset | Brand value | Patient trust | Marketing potential | Clinical credibility | Conversion potential | Must improve |
|---|---|---|---|---|---|---|
| Katraj clinic (physical) | 3 E | 3 E | 3 E | 3 E | 4 E | A procedure room fit for sterile procedures, a couple-consult room, waiting-area privacy |
| Google listing | 4 (bilingual name, landmark) | 4 (4.9★; count unknown) | 3 | 2 ("Alternative medicine practitioner" category) | 4 (WhatsApp, phone) | Change category; fertility-relevant reviews, photos and Q&A; review volume against Gynoveda Kondhwa |
| Website | 2 | **1 (casino spam on the blog)** | 2 | 2 (claims unsubstantiated, counters at "0+") | 2 | **Remove the spam and secure the site first**; fix claims; add an outcomes page and prices |
| Instagram | _?_ (login wall) | _?_ | _?_ | _?_ | _?_ | Founder on camera, a separate fertility handle |
| YouTube story | 3 E (title is emotionally strong) | 3 E | 3 E | 1 (testimonial only) | 3 E | Consent, documentation, **no hereditary-outcome implication**, disability-sensitive edit |
| Founder (MD, Rasa Shastra) | 4 E | 4 E | 4 E | 3 E | 4 E | Add a Prasuti Tantra/Stree Roga consultant and a visiting gynaecologist |
| In-house formulations | 3 E | 3 E | 3 E | 3 E | 3 E | COA per batch, shelf-life data |

### 1.6 Credibility gap to close

The founder's MD is in Rasa Shastra (pharmaceutics), a real strength for medicine quality. A fertility programme, however, needs either a **Prasuti Tantra & Stree Roga MD** (part-time is fine) or a **visiting MBBS/MS OBG**. Both matter for clinical governance and for gynaecologist trust. Budget ₹30–60 k/month for a visiting consultant.

### 1.7 Money and time saved by piloting at Katraj (Model A vs. a new clinic, Model B)

| Item | New premium clinic (B) | Katraj pilot (A) | Saved |
|---|---|---|---|
| Deposit + fit-out + equipment | ₹45–75 L | ₹6–9 L (upgrades only) | **₹40–65 L** |
| Fixed monthly burn before revenue | ₹6–8 L | ₹2.3–2.8 L incremental | **₹4–5 L/month** |
| Time to first patient | 4–7 months (lease, fit-out, registrations) | 6–10 weeks | **3–5 months** |
| Reviews / local SEO | Starts at zero | Existing listing | 6–12 months of review building |
| Registrations | New Shop & Establishment, biomedical waste, possibly PMC | Mostly already held; amend scope | ₹0.5–1 L plus weeks |

---

## PART 2 — THE OPPORTUNITY

### 2.1 Drop "body detox before pregnancy"

| Problem with "detox" | Why it matters |
|---|---|
| No defined, measurable "toxin" being removed | Fails ASCI substantiation, and invites "pseudoscience" coverage |
| It implies the couple's body is "toxic" | Fear- and shame-based, which goes against your own brief |
| It suggests Panchakarma is the product | It pushes procedures onto people who do not need them |
| It conflicts with the evidence | The interventions with proven preconception benefit are **folic acid, stopping smoking and alcohol, weight optimisation, diet, physical activity and managing chronic disease** (preconception care reviews; Cochrane: periconceptional folic acid reduces neural tube defect risk by about 72%) |

**Recommended language:**

- Category: **"Preconception health programme for couples"**
- Brand line: **"Conscious Conception — a 90-day couple preparation programme"**
- Why 90 days: sperm take about 74 days to develop, and the final phases of follicle growth take months. This makes 90 days a **physiologically sensible preparation window**. Say exactly that. Do not claim the programme *improves egg or sperm quality*.
- Ayurveda's role: "*Ayurveda-led lifestyle, diet and individual assessment, with classical therapies where your doctor judges them appropriate.*"
- Use "Shodhana" or Panchakarma by name, with "traditional cleansing therapy" as a description, never as a medical claim.

### 2.2 Clinical triage: which conditions Ayurveda can support and which need referral

| Condition | Ayurveda's role | Parallel specialist needed? | Refer promptly when |
|---|---|---|---|
| Couple planning, not yet TTC | **Primary**: lifestyle, diet, stress, assessment | No (OBG for routine preconception tests) | Chronic disease or abnormal baseline tests |
| PCOS / anovulation | Adjunct: weight, insulin resistance, lifestyle, cycle regularity | **Yes.** The international PCOS guideline (2023) makes **letrozole first-line** for ovulation induction. | No confirmed ovulation after 3 cycles; woman ≥35; TTC ≥12 months |
| Irregular cycles, cause unknown | After work-up only | **Yes**: TSH, prolactin, AMH, ultrasound first | Abnormal endocrine results |
| Endometriosis | Symptom support only (pain, quality of life) | **Yes** | Moderate or severe disease, endometrioma, infertility of 6+ months |
| Tubal factor | **Do not position as treatment.** Uttarbasti for tubal block rests on tiny single-arm studies (e.g. AYU 2010, n = 16). | **Yes** | **Bilateral block means immediate IVF referral.** Unilateral block or hydrosalpinx means a specialist decides. |
| Diminished ovarian reserve (low AMH) | Supportive only | **Yes, urgently** | Immediately. Time is the treatment. |
| Mild low count or motility | Reasonable adjunct: lifestyle, heat/smoking/alcohol, ashwagandha (small RCT, n = 46) | Andrology review advised | No improvement on repeat semen analysis at 3 months |
| Severe OAT, azoospermia, very poor morphology | Not appropriate as primary care | **Yes**: urologist/andrologist, hormones, karyotype, Y-microdeletion | Immediately |
| Varicocele, infection, erectile or ejaculatory dysfunction | Adjunct only | **Yes**: urology | At diagnosis |
| Unexplained, woman <35, TTC <12 months | **Good fit** | OBG baseline | Woman reaches 35, or TTC reaches 12 months |

**Hard referral clock** (company policy, written into every consent form): woman ≥35 and TTC ≥6 months, or woman <35 and TTC ≥12 months, means a **parallel** REI/IVF consultation is mandatory. Aastik care continues alongside it only if the specialist agrees. This follows standard fertility-society practice and is the core of the "safe Ayurveda" positioning.

### 2.3 The three propositions, scored

Scale 1–5; higher is better. For regulatory risk and CAC, a higher score means **lower** risk or cost.

| Criterion | A. Premium preconception | B. TTC couple programme (narrowed) | C. Integrative IVF support |
|---|---|---|---|
| Demand / urgency | 2 (preventive, deferrable) | **5** | 3 |
| Ability and willingness to pay | 3 | **4** | 4 (but the money goes to IVF) |
| Clinical feasibility | **5** | 4 (with triage) | 3 (IVF centre sets the rules) |
| Competitive intensity (5 = low) | 4 | 2 (Gynoveda) | 4 |
| Regulatory risk (5 = low) | **5** | 3 (DMR Act limits ads) | 3 |
| Gross margin | 4 | 4 | 3 |
| CAC (5 = low) | 2 (must create demand) | 3 | 4 if referral-led, 1 if not |
| Repeat / expansion revenue | 3 (leads into antenatal) | **4** | 2 |
| Scalability | 4 | 4 | 2 (depends on partners) |
| Time to first revenue | 4 | **5** | 1 (6–12 months to sign partners) |
| **Total / 50** | **36** | **38** | **29** |

**Decision: primary entry is B, narrowed**: couples TTC 6–24 months, woman under 35 (or 35–38 with REI co-management), with a full diagnostic work-up for both partners. A is the **entry tier and content engine**; it is low-risk, but people do not urgently buy prevention. **C waits** until Aastik has 12 months of outcome data and at least two IVF partners. Even then, frame it as stress, sleep, diet and adherence support, with **no IVF success claims**.

### 2.4 Evidence summary (what you may and may not say)

| Claim | Evidence | Permitted wording |
|---|---|---|
| Lifestyle changes before conception matter | Strong for smoking, alcohol, BMI, folic acid | "Evidence-based preparation for pregnancy" |
| Ayurveda improves PCOS symptoms | A scoping review (57 papers, 13 RCTs) found results "promising", with gaps | "May help manage symptoms; studied in small trials" |
| Ayurveda treats infertility | A Cureus 2024 systematic review covered 14 studies and 248 patients, mostly weak designs | Do not claim it |
| Ashwagandha improves sperm | One n = 46 RCT in oligospermia (90 days) plus one 8-week RCT in healthy men (n = 76), largely from one research group | "Studied in small trials" only, never "boosts fertility" |
| Uttarbasti opens tubes | Single-arm studies, n ≈ 15–16 | Do not claim it |
| Improves IVF success | No adequate evidence found | Do not claim it |

**This is also the opportunity.** An Ayurveda fertility provider that publishes honest, denominator-based outcomes would be **the only one doing so**, and that is a moat. Register an observational outcomes study on CTRI, with ethics committee approval through a partner institution. Your IIT Delhi and AIIA academic links can help find an ethics committee and co-investigators.

---

## PART 3 — CUSTOMERS AND VALIDATION

### 3.1 Testing "couples who spent ₹25 L+ on weddings"

**Verdict: it is a poor targeting variable.**

| Wedding spend | Fertility spend |
|---|---|
| Usually family-funded | Couple-funded, often private |
| Status signalling, public | Private, often stigmatised |
| One-off, planned years ahead | Urgent, triggered by time and anxiety |
| Not targetable in ad platforms after the event | Targetable through intent (searches, content) and referrals |

It also tells you nothing about the actual purchase driver: **months trying to conceive, the woman's age, a prior failed treatment, and a gynaecologist's recommendation.** Couples already spending ₹1–2 L per IVF cycle out of pocket (infertility is a standard health-insurance exclusion) are a far better proof of willingness to pay than a wedding budget. The wedding audience is useful only for **segment A content** (newly married couples planning pregnancy in 1–2 years), through wedding and lifestyle influencers, at low intensity.

### 3.2 Segments

| Segment | Age / stage | Geography | HH income / capacity | Core problem | Emotion | Alternatives | Objections | Decision | Price sensitivity | Best channel |
|---|---|---|---|---|---|---|---|---|---|---|
| **S1 TTC 6–24 months, woman <35** (PRIMARY) | 26–34, married 1–5 yrs | Pune urban, PCMC | ₹15–50 L dual income | No pregnancy yet; often PCOS or irregular cycles | Anxiety, family pressure, hope | Gynoveda, local OBG + letrozole, "wait and see" | "Does Ayurveda work?", "Will it delay IVF?", time cost | Woman researches, couple decides, family influences | Medium | Search (intent keywords), YouTube education, OBG referral |
| S2 Planning in 6–12 months | 25–32, newly married | Pune IT belts (Hinjewadi, Kharadi, Baner) | ₹20–60 L | Wants to "do it right" | Aspiration, control | Nothing, Google, apps | "Not needed yet" | Couple | High | Instagram, wedding/lifestyle creators, corporate wellness talks |
| S3 Multiple failed consultations | 30–38 | Pune + Maharashtra | ₹15–40 L | Fatigue with conventional care, wants a holistic second opinion | Frustration | IVF, more OBG visits | Cost, scepticism, time | Couple | Medium–low | Referral, YouTube, testimonials (compliant) |
| S4 Male factor | 28–40 | Pune | ₹15–50 L | Abnormal semen analysis | Embarrassment | Urologist, supplements online | Privacy, stigma | Man, often prompted by partner | Medium | Search, discreet WhatsApp, andrologist referral |
| S5 Going through IVF (later) | 30–40 | Pune | ₹20 L+ | Stress, side effects, wants to "do everything" | Fear of failure | Acupuncture, counselling | IVF doctor disapproval | Couple + IVF doctor | Low (already spending) | IVF centre partnerships only |
| S6 NRI / international | 28–40 | US, UK, Gulf, with Pune family roots | High | Wants authentic Ayurveda + care while visiting India | Trust | Kerala centres | Logistics, time | Couple | Low | Diaspora content, ISKCON global networks (see 7.4) |

**No fear or stigma.** Never use "Are you infertile?", "biological clock" countdowns or before-and-after baby imagery. Target intent ("planning pregnancy", "PCOS and conception"), not affliction.

### 3.3 Primary research programme

**Method:** 30 couple interviews (20 in S1/S3, 10 in S2), 8 OBGs, 5 IVF specialists, 6 Ayurveda physicians and 6 referral partners, over 6 weeks. Then run a **paid pre-sale test**: a ₹2,000 refundable deposit for a "founding cohort" slot. A deposit is the only reliable willingness-to-pay signal.

**Confidentiality:** recruit through opt-in forms, not the patient register. Obtain written consent. Do not record without permission. Store notes pseudonymised (C-01, C-02…). Keep no diagnostic details in interview notes. Delete audio after transcription. Have a non-treating team member conduct the interview so patients do not feel obliged.

**20 questions for prospective couples** (behavioural, not "would you like…?"):
1. How long have you been planning or trying to conceive?
2. Walk me through every step you have taken so far, in order.
3. Which doctors, apps or products have you used? What did each cost?
4. What did you spend on fertility or pregnancy preparation in the last 12 months?
5. What made you choose the last provider you paid?
6. What disappointed you about it?
7. Who in the family knows, and who influences decisions?
8. Have you both been tested? If not, what stopped the male partner?
9. What would make you trust an Ayurveda doctor with this?
10. What would make you distrust one?
11. If a programme required both of you to attend in person every 2 weeks, could you?
12. What would make you stop a programme halfway?
13. When you hear "Panchakarma", what do you imagine?
14. Have you considered IVF? At what point would you go?
15. If an Ayurveda clinic told you "see an IVF specialist now", would you trust it more or less?
16. How do you usually pay for health services: upfront, EMI, card?
17. (Price ladder) At what price would a 6-month couple programme be so cheap you would doubt it? A bargain? Expensive but worth considering? Too expensive? (Van Westendorp)
18. Here is a ₹39 k / ₹79 k / ₹1.25 L option. Which would you pick, and what would you remove to make it cheaper?
19. Would you put down a ₹2,000 refundable deposit today for a founding-cohort place? (Record the actual yes or no.)
20. Who else do you know in your situation? (Referral potential)

**10 for gynaecologists:**
1. How many TTC couples do you see per month, and what share are under 35?
2. What share ask you about Ayurveda or supplements?
3. Where do you see Ayurveda helping, and where has it harmed your patients?
4. What would an Ayurveda clinic have to do for you to refer patients?
5. What reporting would you want back from us, and how often?
6. What is your current first-line plan for PCOS anovulation?
7. At what point do you refer to IVF?
8. Would you co-manage a patient on letrozole while they receive Ayurveda lifestyle care?
9. What worries you about Panchakarma or Uttarbasti specifically?
10. Would you be a visiting consultant or protocol reviewer, and on what terms?

**10 for IVF specialists:**
1. How many patients disclose Ayurveda or herbal use during IVF?
2. Which herbs or procedures do you ask patients to stop, and when?
3. Which patient problems do you lack time for (stress, diet, adherence)?
4. Would a structured, non-pharmacological support programme be useful?
5. What evidence would you need to recommend it?
6. What would make you refuse to work with us?
7. Where do patients waste time before reaching you?
8. Would you accept referrals from us under a written referral clock?
9. How do you want communication handled: shared notes, letters?
10. Would you co-author an observational outcomes paper?

**10 for Ayurveda physicians:**
1. Which fertility protocols do you actually use, and why?
2. How do you decide Panchakarma eligibility for a TTC patient?
3. Uttarbasti: indications, complications seen, sterility practice?
4. How do you document outcomes?
5. What do patients typically pay you, and for what?
6. Which referral rules do you follow?
7. Biggest patient drop-out reasons?
8. Medicines: in-house or branded? Typical monthly cost to the patient?
9. Would you join a protocolised network with outcome reporting?
10. What would you never do in fertility care?

**10 for referral partners** (yoga studios, dietitians, diagnostic labs, corporate HR, wedding planners, ISKCON programme leads):
1. How often do your clients raise pregnancy planning?
2. What do you currently recommend?
3. What would make you comfortable recommending a clinic?
4. What content or events would your audience attend?
5. How do you prefer to collaborate (talks, co-branded workshops)?
6. What has gone wrong with past health partners?
7. What does your audience spend on wellness each month?
8. Is there an audience segment you would never market to?
9. Would you host a free educational session in the next 60 days?
10. What would you need from us to measure the partnership?

**Fee-sharing note:** do not pay commissions for patient referrals to doctors or clinics. Professional ethics codes for Indian Systems of Medicine practitioners prohibit rebates and commissions, and so does the NMC code for allopaths. Partnerships should be content, events and clinical co-management, each billed directly.

---

## PART 4 — COMPETITOR INTELLIGENCE

### 4.1 Gynoveda (direct, scaled Ayurveda fertility)

**First-hand findings from gynoveda.com (accessed 23 Nov 2026):**

| Item | What the site says |
|---|---|
| Footprint | "**50+ Clinics Across India, 100+ Doctors**"; Mumbai 6, Delhi 4, Bengaluru 3, plus Jaipur, Vadodara, Nagpur, Amritsar, Hyderabad and others. About page: "**200+ chain of ayurveda fertility clinics planned in the next 3 years**". HQ Mumbai, founded 2019. |
| **Pune** | **3 clinics: Viman Nagar** (Nyati Empress, near Phoenix Marketcity), **Pimple Saudagar** (PK Hillcrest) and **Kondhwa** (99 Avenue Complex, Lulla Nagar, next to Atithi Hotel). Each shows 4.8★. Open 10 AM–8 PM, Tue–Sun. **Kondhwa is about 4–5 km from Aastik Katraj.** |
| Consultation | **₹2,000** in Pune ("50+ health parameters, root cause analysis, diet suggestions"). "**Pay after consultation**". "**40-min consultation**", "**Consult as couple**". Booking by call-back (7240000700). |
| Model | 3 steps: doctor consult → Ayurveda tablets ("Improve egg quality. Increase sperm count.") → Gynoveda diet + follow-up. Online or in-clinic. |
| Hero fertility product | "Fertility Ayurvedic Tablets", **Putranjivak + Shivlingi + 15 herbs** (incl. Shilajit, Shatavari, Ashwagandha, Ashoka, Lodhra, Shuddha Kasis, Bang Bhasma, Shuddha Tankan). **1 month ₹2,063; 2 months ₹3,375; 3 months ₹4,125** (MRP ₹7,031); 2,231+ reviews; dose 2 tablets twice daily; "take for minimum 6 months". The PCOS range starts at ₹2,400. |
| Who they target | "Couples planning a baby… Failed IUI, IVF history… Advised to do IUI, IVF… Low AMH… One Tubal Block… Pregnancy Loss" |
| Scale claims | "4.7★ / 27,433+ Google Reviews", "6L+ Happy Customers", "**20000+ Babies born naturally**" (source: "Gynoveda internal outcome study"), "**40% Male Infertility Cases Solved**", brand ambassador Taapsee Pannu since 2023, a large Facebook community ("Circle of Sisterhood") |
| **Claim inconsistency** | The clinic page headline says "**85%\* Women Conceived in 3 Months**, Source: EJPMR, 2023". The FAQ on the same page and the product page describe the same study as "**85% of women… ovulated on time**". **An ovulation statistic is presented as a conception statistic.** |
| Ingredient claims | "Putranjivak **ensures healthy implantation**", "Shivlingi **improves egg quality**", "Shatavari **prevents early pregnancy loss**" |
| IVF positioning | Positions itself **as an alternative to IVF**: "Want to Conceive without IVF?", stories titled "No IVF…", "Told to Try IVF, She Chose Ayurveda". The comparison page lists IVF side effects as "Severe / Surgical / High" and Ayurveda as "**Hormonal Changes: None**", and labels months 0–3 "**Herbal Detox**". It quotes Ayurveda cost as **₹3,000–30,000** for 3–12 months against ₹1.5–2.5 L per IVF cycle. |
| Low AMH / tubal advice | Product FAQ: low AMH → "chances… compromised a bit", take the tablets. One blocked tube → can take; both blocked → "will not help". |
| **Refund policy** | Returns only for damaged, incomplete, wrong or wrong-quantity **unused** products, notified within 5 business days. **Consumed product: no refund**; COD orders only "in exceptional cases"; "All decisions… shall be final and binding. You agree not to challenge such a decision." |

**Implications for Aastik:**
1. Gynoveda **already runs a couple-consultation clinic model in Pune, including 4–5 km from Katraj**. Aastik is not first to clinic-based Ayurveda fertility. It must win on **procedures, a published outcome method, the IVF referral clock and transparent refunds**.
2. Its "ovulation → conception" headline, "no hormonal changes", "prevents pregnancy loss" and IVF-alternative framing are the exact claims Aastik should **publicly not make**. Being visibly more careful is a credible position with gynaecologists.
3. The ₹2,000 consult and a ₹4,125 three-month medicine pack set the **local price anchor**. Aastik's ₹2,500–3,000 first couple consultation is acceptable if it is longer (75 min vs 40) and is credited on enrolment.
4. Its refund terms are restrictive and non-negotiable. Aastik's pro-rata refund and pregnancy-conversion policy (5.2) is a concrete, advertisable difference.

**Third-party data:**

| Item | Finding | Source / date |
|---|---|---|
| Founders | Rachana Gupta and Vishal Gupta | FemTech Insider; Entrepreneur India, Mar 2023 |
| Funding | **$10 M Series A (Mar 2023)** led by India Alternatives Fund, with Wipro Enterprises, RPG Ventures, Dharampal Satyapal, Alteria Capital and Fireside Ventures. About $11 M total per Inc42. | Entrepreneur India; Inc42 |
| Revenue | Claimed ₹100 Cr annualised (2023). Aggregators report **FY24 revenue ₹67.16 Cr, expenses ₹70.29 Cr, loss ₹3.13 Cr**, and **FY25 ₹68.1 Cr**, i.e. roughly flat growth. **Unaudited; check MCA filings.** | TheKredible; Inc42 Datalabs (accessed Nov 2026) |
| Physical footprint | Second Pune fertility clinic opened (date unclear); a stated target of 100+ clinics, reported as "100 by 2027" | Digital Health News; FemTech Insider |
| Core product | Herbal tablet kits, e.g. **"Jeehv" (Putrajeevak beej + Shivlingi beej)** fertility tablets. Shop page: 1 month ₹2,063, 2 months ₹3,375, 3 months ₹4,125 (per product). | shop.gynoveda.com (indexed) |
| Your price observations | 3-month male/female ₹11 k, couple ₹18 k; 6-month ₹29 k; 9-month ₹38 k; 12-month ₹48 k | **User-supplied, not verified** (the site is blocked here) |
| Distribution | D2C website, Amazon, Flipkart, Hyugalife, clinics | Marketplace listings |
| Reviews | Mixed. Positive stories of conceiving after 1–3 months. Negatives: "no change in cyst", "aggravated PCOS", "slow efficacy". A Quora user reports no refund of remaining medicine if the customer conceives early (anecdotal). | Flipkart, Quora, tenereteam (2024–26) |
| Refund | No official programme refund policy found. Marketplace returns cover only damaged or wrong items. | Amazon.in |
| Claims risk | "Natural pregnancy" positioning plus the names Putrajeevak and Shivlingi. Putrajeevak has historically drawn "son-giving" controversy (PCPNDT concerns), a reputational risk in this category. | Press 2015; general |

**Why it works commercially:** a low entry ticket (₹4–18 k), a simple kit, a tele-doctor funnel, high ad spend and women-first emotional branding.

**Weaknesses you can exploit:**
1. Medicine-led, little in-person care or procedures.
2. Women-first. Male factor is under-served.
3. No published outcome denominators.
4. Growth appears to have stalled at about ₹68 Cr, which suggests rising CAC and a churn ceiling for the kit model.
5. Its scale makes a "don't delay IVF" referral policy commercially awkward. That is exactly your opening.

**What to copy:** the WhatsApp/tele-consult funnel, plain-language education, EMI-friendly pricing ladders and the clinic + D2C hybrid.

### 4.2 Landscape, classified

| Class | Players | Notes (sources in Section 10) |
|---|---|---|
| **1. Direct Ayurveda fertility** | Gynoveda; **AyurVAID (Apollo AyurVAID)**, which runs infertility and reproductive "whole health" programmes and Uttarbasti content and is expanding pan-India in FY26; Pune independents: **Aatreya Ayurvedic Panchakarma & Infertility Clinic (Baner)**, **Aasha Ayurveda** (offers Uttarbasti), **Ayurgarbh Ayurvedic Chikitsalay & Panchakarma (Undri, about 6–8 km from Katraj)**, **Shree Sai Ayurvedic Infertility Research Clinic (Nigdi)**, Shree Aarogyam (Pimple Gurav) | Independents are fragmented, rarely publish prices, and are founder-dependent. |
| **2. Conventional IVF** | **Indira IVF**: 165+ centres, FY25 operating income ~₹1,605 Cr, PAT ~₹298 Cr (Kotak Neo, unverified), 7 Pune centres including Baner, IPO in process. **Nova IVF**: ~120 clinics; Pune at Kharadi, Baner, Lulla Nagar (Kondhwa). **Birla Fertility & IVF**: "all-inclusive" IVF package ₹1.70 L. **Oasis Fertility**: Kondhwa, 4.9★ from 756 reviews. **Cloudnine** Pune fertility. **Progenesis** (Aundh). **Manipal** Pune. **Gaudium IVF**: ₹104 Cr revenue, IPO, 19 new centres. | IVF price in Pune: Indira from ₹1.0 L, Nova ₹1.8 L/cycle, Birla range ₹1.4–3.4 L; drugs often ₹40–80 k extra. |
| **3. Integrated** | Apollo AyurVAID (hospital model); some IVF centres offer yoga/diet add-ons | No Pune player combines an Ayurveda couple programme, an OBG/REI referral clock and published outcomes. |
| **4. Digital** | Pinky Promise (women's hybrid care, first clinic in Mumbai), Gynoveda tele-consults, app-based cycle trackers. Allo Health (sexual health, relevant to men) per general knowledge; verify. | Low-cost, high-reach. Aastik should not compete on price here. |
| **5. Indirect** | Local OBG + letrozole (consult ₹550–1,400 in Pune per Practo), Ashwagandha/Shatavari OTC, Garbh Sanskar classes, yoga studios, "do nothing" | "Do nothing" is the biggest competitor for segment A. |

### 4.3 Comparison matrix

| Parameter | **Aastik (proposed)** | Gynoveda | IVF chains | Other Ayurveda clinics |
|---|---|---|---|---|
| Business model | Clinic-based couple programme + own medicines + referral network | D2C kits + tele-doctors + clinics | Procedure revenue (IVF/ICSI/IUI/PGT) | Fee-for-service OPD + Panchakarma |
| Core customer | TTC 6–24 months couples <35; planners | Women with PCOS/irregular periods/TTC | Diagnosed infertility, 30–42 | Walk-in, local |
| Price | ₹39 k / ₹79 k / ₹1.25 L | ₹4–48 k (per kit/plan; partly unverified) | ₹1.0–3.4 L per cycle + drugs | Rarely published; ₹20–60 k typical (estimate) |
| Duration | 3 or 6 months, fixed review points | 3–12 months | 4–6 weeks per cycle | Open-ended |
| Medicines | Own GMP-made SKUs, batch COA | Own branded tablets | Allopathic hormones | Mixed brands |
| Panchakarma | Yes, only on documented indication | No or limited | No | Yes, often routine |
| Physical clinics | 1 (Katraj) | 50+ nationally, **3 in Pune** (Viman Nagar, Pimple Saudagar, Kondhwa); 200+ planned | 7+ Indira, 3 Nova in Pune | 1 each |
| Doctor involvement | Founder MD + Prasuti Tantra consultant + visiting OBG | Tele-consult BAMS doctors | REI specialists, embryologists | One BAMS/MD |
| Diagnostics | **Mandatory couple work-up** (via partner lab) | Patient-reported or optional | Full | Variable |
| IVF integration | **Written referral clock + co-management** | Positioned as an alternative | Core | Usually none |
| Online consults | Follow-ups only; first visit in person | Core | Some | Rare |
| Brand positioning | "Safe, accountable Ayurveda for couples" | "Natural pregnancy" | "Science and success rates" | Tradition |
| Marketing channels | Search, YouTube education, OBG referrals, community talks | Meta/Google performance ads, marketplaces | Search, TV, referral | Word of mouth |
| Clinical evidence | Will publish an outcomes registry (CTRI) | Not found | ART registry data, published rates | None |
| Customer reviews | _To build_ | Mixed (efficacy complaints) | Strong per-centre review volume | Thin |
| Scalability | Medium (doctor-bound; protocolise) | High (product) | High (capital-heavy) | Low |

### 4.4 Why a couple would choose Aastik

- **Over Gynoveda:** "Both of us are examined in person. My husband's semen report is treated as half the problem. I get procedures when indicated. And they will tell me in writing when to go to IVF."
- **Over a local gynaecologist:** "My gynaecologist gives me letrozole and 8 minutes. Aastik gives us a 75-minute couple consultation, a diet, sleep and stress plan, follow-ups every 2 weeks, and coordinates with my gynaecologist instead of replacing her."
- **Over an IVF chain:** "We are under 35 and have tried for 9 months. We are not ready for IVF. Aastik gives us a structured 6-month window with a clear exit point, rather than jumping to a ₹1.5 L cycle."

**The defensible advantage is the system, not "personalisation":** couple-level protocol + in-house standardised medicines + procedure capability + **an outcomes registry with denominators** + **a referral clock**. The clock turns gynaecologists and IVF centres into a referral channel, which no medicine-led D2C competitor can credibly match without cannibalising itself.

---

## PART 5 — PACKAGE ARCHITECTURE

### 5.1 Cost assumptions (CFO)

| Driver | Assumption | Basis |
|---|---|---|
| Doctor cost | ₹350/h (₹60 k/month ÷ ~180 productive h) | Your staffing assumption |
| Therapist / nurse | ₹140/h (₹25 k ÷ 180 h) | Your assumption |
| Coordinator / counsellor | ₹170–200/h | ₹30–35 k/month |
| Medicines at cost | ₹700/person/month (V1), ₹1,000 (V2/V3) | In-house SKUs; **validate against actual COGS** |
| Diagnostics | Excluded in V1/V2 (billed by the lab directly). V3 includes repeat tests at B2B rates (~₹3,000). | Prevents margin erosion and keeps the conflict of interest clean |
| Payment gateway | 2% | |
| CAC | ₹10–18 k per enrolled couple (year-1 target; actual year 1 will be higher) | Section 9 |
| GST | Healthcare services by a clinical establishment or authorised practitioner are generally exempt. Medicines bundled into a package raise composite-supply questions. **Get a CA opinion before pricing.** | |

### 5.2 Three versions

| | **V1 Conservative: "Foundations" (3 months)** | **V2 Premium: "Couple Programme" (6 months)** | **V3 Signature: "Aastik Conscious Conception" (6 months)** |
|---|---|---|---|
| Eligibility | Planners (A) or TTC <12 months; woman <35; no red flags | TTC 6–24 months; woman <35, or 35–38 with REI co-management; work-up done | A or B couples wanting high-touch care; same clinical gates |
| Consultations | 75-min couple assessment + 6 fortnightly follow-ups (in person or tele) | Assessment + 12 fortnightly follow-ups + 2 formal reassessments (month 3 and month 6) | V2 + **founder-led** reviews + a named care coordinator (WhatsApp, same-day reply) |
| Medicines | 1–2 SKUs per partner (~₹700/person/month at cost) | 2–3 SKUs per partner, adjusted at reassessment | As V2 |
| Panchakarma | None included (add-on on indication) | **One shodhana block per partner**, e.g. Yoga Basti (8 bastis) + 4 Abhyanga–Swedana, or outpatient Virechana for a suitable male partner | **Two blocks per partner** + private suite + couple-scheduled sessions |
| Uttarbasti | Not included | **Add-on only** on documented indication | Included **only if indicated** (budgeted at a 40% probability × 6 sessions) |
| Diagnostics | Review of existing reports; tests ordered and billed separately | Same + coordination with OBG and lab | **Includes** month-3 repeat semen analysis, D21 progesterone and HbA1c/HOMA-IR via a partner lab |
| Lifestyle | Diet plan, 12 online group yoga sessions, 1 counselling session | Dietitian 4 h, counselling 2 sessions, yoga | Private couple yoga ×8, dietitian 6 h, counselling ×4 |
| Staff time (approx.) | Doctor 3.75 h, coordinator 2 h, yoga (group) | Doctor 6.25 h, coordinator 6 h, therapists ~17 h | Doctor 8 h, coordinator 12 h, therapists ~35 h |
| **Direct cost** | **~₹7,800** | **~₹29,500** | **~₹51,300** |
| **Recommended price (couple)** | **₹39,000** (single partner ₹24,000) | **₹79,000** | **₹1,25,000** |
| Gross margin | ~80% | ~63% | ~59% |
| CAC (target) | ₹10,000 | ₹12,000 | ₹18,000 |
| **Contribution after CAC** | **~₹21,200 (54%)** | **~₹37,500 (47%)** | **~₹55,700 (45%)** |
| Payment schedule | 100% upfront, or 2 × ₹19,500 | 40% at enrolment / 30% at day 45 / 30% at day 90; 0% EMI via a partner | 40/30/30; EMI |
| Exclusions | Diagnostics, specialist fees, allopathic drugs, Uttarbasti, pregnancy care | Same + Uttarbasti | Specialist fees, ART procedures |
| Refund / cancellation | Within 7 days and before medicines are dispensed: full refund minus the ₹3,000 assessment fee. After that: pro-rata refund of **unused services**; dispensed medicines are non-refundable. | Same | Same |
| If pregnancy occurs mid-programme | Unused value converts to an Ayurveda-supported antenatal follow-up credit, or a pro-rata refund of unused procedures. **This turns Gynoveda's reported weak point into a trust signal.** | Same | Same |
| Follow-up policy | Missed follow-ups get rescheduled within 14 days; tele allowed | Same; 2 in-person reassessments mandatory | Same |
| Clinical review points | Day 0, day 45, day 90 | Day 0, day 45, **day 90 (formal)**, day 135, **day 180 (formal + outcome capture)** | Same + an MDT case review with the visiting OBG |
| Referral criteria | The referral clock (2.2) + any red flag | Same | Same |
| Outcome language | "Programme fee covers services, not results. **No guarantee of conception, pregnancy or live birth.**" | Same | Same |

**Commercial viability without pregnancy:** every package is priced so that margin comes from delivered services and medicines, not success fees. No outcome-linked refunds: they imply a promise and create perverse incentives.

### 5.3 Testing your price hypotheses

| Your hypothesis | Verdict | Why |
|---|---|---|
| Healthy Conception ₹1,00,000 | **Too high for the mass of segment A.** Viable only as V3 "Signature" for about 10% of the mix. | No urgency. The comparison is "do nothing" or a ₹3–5 k OBG preconception visit. |
| Infertility Support ₹1,50,000 | **Reject.** | It equals or exceeds an IVF cycle in Pune (₹1.0–1.8 L), which has measurable success rates. A rational couple at ₹1.5 L chooses IVF. |
| Recommended ladder | **₹39 k / ₹79 k / ₹1.25 L** | That is 2–4× Gynoveda's ticket for in-person, couple-level, procedure-capable care, and below an IVF cycle. Validate with Van Westendorp plus the deposit test (3.3). |

---

## PART 6 — PANCHAKARMA AND PROCEDURE ECONOMICS

### 6.1 The "NCISM rate" question

- **I found no NCISM notification setting procedure rates for Uttarbasti or other Panchakarma procedures.** NCISM documents found cover curriculum (the BAMS Panchakarma syllabus) and college ratings. NCISM regulates education and practitioners, not private fees.
- If you have seen a rate list, it is most likely one of: (a) the **CGHS rate list for empanelled Ayush hospitals** (a government reimbursement schedule for CGHS beneficiaries only); (b) a **state Ayush hospital user-fee schedule**; or (c) an insurer or TPA tariff. **None of these caps what a private clinic may charge.** Send me the document and I will classify it.
- **TPA / insurance:** IRDAI rules allow Ayush in-patient treatment to be covered, but only in an "Ayush hospital" meeting the regulatory definition (registered, with minimum in-patient beds and qualified staff). Separately, **"sterility and infertility" is on IRDAI's standard list of exclusions.** So Uttarbasti for infertility is **effectively not reimbursable** even in an inpatient setting. Verify against the current IRDAI master circular and specific policy wordings.
- **Private pricing:** a private clinic sets its own fees. In Maharashtra, the pending **Maharashtra Clinical Establishments (Registration and Regulation) Bill, 2026** may introduce rate display and transparency obligations. Track its status.
- **Documentation:** indication, contraindication screen, informed consent (procedure-specific, in Marathi/Hindi/English), pre-procedure vitals, the batch number of the medicated oil, the sterile pack lot, the operator, and adverse event notes.
- **Who may perform it:** a registered Ayurveda practitioner (MCIM-registered in Maharashtra) performs it, with a trained female nurse or therapist present (chaperone). Female Uttarbasti should be done by a female doctor or with a female chaperone, as clinic policy.
- **Infection control:** single-use sterile cannula or catheter, sterile gloves and drapes, an autoclaved or disposable speculum, oil/ghee from **sterile, single-patient aliquots** (never a shared bottle), hand hygiene, and biomedical waste segregation under the BMW Rules 2016. Pre-screening: HIV, HBsAg, VDRL, urine routine, and exclusion of genital infection and abnormal bleeding (as in CTRI/2024/04/065704's exclusion criteria).

### 6.2 Uttarbasti: your ₹300 cost is materials only

| Cost line (per female session) | ₹ |
|---|---|
| Sterile cannula/catheter | 80–150 |
| Sterile gloves ×2, drape | 100–120 |
| Speculum (disposable or autoclave share) | 60–100 |
| Sterile medicated oil/ghee aliquot | 50–100 |
| Pre-procedure local Abhyanga–Swedana (materials) | 60–100 |
| Doctor time 30 min | 175 |
| Nurse/therapist 45 min | 105 |
| BMW, autoclave, utilities | 50 |
| **Direct cost** | **≈ ₹700–1,000** |
| One-time pre-screening panel (billed separately) | ₹1,500–2,500 |
| **Recommended price** | **₹2,500–3,500/session**; a course of 6–9 sessions over 2–3 cycles |
| Margin | ~65–75% |

**Male (urethral) Uttarbasti:** risk of urethral trauma and UTI, and even weaker evidence. **Do not offer it in the pilot.**

**Clinical governance rule:** Uttarbasti is never a package line item. It appears only after a documented indication, a contraindication screen, consent and, for tubal indications, an HSG on file and specialist sign-off. Track utilisation monthly. **If over 40% of enrolled women receive it, audit for overuse.**

### 6.3 Procedure and service unit economics

| Service | Direct cost (₹) | Price (₹) | Margin | Time (doctor / therapist) |
|---|---|---|---|---|
| First couple consultation (75 min) | ~520 | 2,500–3,000 standalone (credited on enrolment) | ~80% | 75 min / — |
| Follow-up (20–25 min) | ~150 | 800–1,000 | ~83% | 25 min / — |
| Abhyanga + Swedana (60 min, 2 therapists) | ~550 | 1,800–2,500 | ~70–78% | 5 min / 120 min |
| Anuvasana / Matra Basti | ~250 | 800–1,200 | ~70–80% | 5 min / 30 min |
| Niruha Basti | ~400 | 1,200–1,800 | ~67–78% | 15 min / 45 min |
| Yoga Basti course (8 bastis) | ~2,450 | 9,000–12,000 | ~73–80% | |
| Outpatient Virechana course (snehapana + prep + virechana day) | ~4,000–5,000 | 12,000–18,000 | ~65–72% | 2 h / 4 h |
| Female Uttarbasti session | ~700–1,000 | 2,500–3,500 | ~65–75% | 30 / 45 min |
| Medicines (per person per month) | 700–1,000 | 2,500–3,500 if sold separately | ~65–75% | |

### 6.4 Capacity limits (where the pilot will break)

- **Therapy rooms:** 2 rooms × ~8 slots/day × 26 days ≈ **416 slots/month**. A V2 couple uses about 3–4 procedure slots a month. **About 110–120 active couples saturates 2 rooms**, roughly 20 new V2 enrolments a month in steady state.
- **Doctor time:** about 1 h per active couple per month, so 120 active couples ≈ 120 doctor-hours, about 70% of one full-time doctor. **Hire the second doctor when you pass 60 active couples.**
- **Uttarbasti** is limited by cycle timing (post-menstrual window): bunching around cycle days 5–12. Schedule it with a booking engine, not ad hoc.
- **Founder time** is the hardest limit. Founder-led consults should be reserved for V3 and the first assessment only.

---

## PART 7 — LOCATION, CLINIC AND HOSPITAL STRATEGY

### 7.1 Three models compared

| | **A. Katraj pilot** (recommended) | B. Dedicated premium OPD (Baner/Aundh/Kharadi) | C. 5–10 bed Ayurveda fertility hospital |
|---|---|---|---|
| Space | Existing + 1 procedure-room upgrade | 1,200–1,800 sq ft | 3,500–6,000 sq ft |
| Rent | Existing | ₹1.2–2.0 L/month (your ₹40–80 k is realistic for Katraj, low for street-front Baner/Aundh; Pune Grade-A commercial averages ~₹82/sq ft/month per Knight Frank) | ₹3–6 L/month |
| Deposit | — | ₹8–15 L | ₹20–40 L |
| Fit-out + equipment | ₹4–6 L (autoclave, procedure couch, sterile storage, couple-consult room, hand-wash, CCTV in common areas) | ₹35–55 L | ₹1.2–2.0 Cr (incl. beds, nurse station, fire systems, patient toilets, Panchakarma suites, pharmacy) |
| Tech, brand, content, legal | ₹5–7 L | ₹8–10 L | ₹10–15 L |
| Staffing (monthly) | +₹1.2 L (coordinator, therapist, visiting OBG/PTSR) | ₹3.0–3.5 L (your list: receptionist ₹20 k, 2 doctors ₹1.0–1.4 L, 2 nurses ₹50 k, helper ₹5–10 k, + coordinator and therapists) | ₹8–12 L (24×7 nursing in 3 shifts, RMO cover, housekeeping, kitchen) |
| Marketing (monthly) | ₹1.25 L | ₹2–3 L | ₹3–5 L |
| Licences | Amend existing; BMW authorisation; Shop & Establishment | New Shop & Establishment, BMW, signage, possibly PMC | **Nursing home registration (Bombay Nursing Homes Registration Act 1949 + 2021 rules) with PMC**, fire NOC, BMW, lift and occupancy, pharmacy licence for non-patient sales |
| Total capex + 6 months' working capital | **₹12–18 L** | **₹75 L–1.1 Cr** | **₹2.5–4 Cr** |
| Time to first fertility patient | 6–10 weeks | 4–7 months | 9–15 months |
| Break-even (incremental) | ~6–7 V2-equivalent couples/month | ~14–18/month + OPD | Needs 60–70% bed occupancy. **Fertility patients do not need beds**, and insurance excludes infertility. |
| Verdict | **Do now** | Do when Katraj passes about 15 enrolments/month for 3 months, or when outcome data proves the model | **Do not build.** Revisit only for a residential Panchakarma retreat business, which is a different model. |

### 7.2 NABH: what applies

| Programme | Applies to | Use for Aastik |
|---|---|---|
| **Entry-Level Ayush Centres Certification** | Ayush centres without inpatient services (clinics, polyclinics) | **Step 1, within 6–9 months.** FAQ fee ₹11,000 + GST, valid 2 years, assessments can be virtual or hybrid. Verify current fees. |
| **Accreditation Standards for Ayush Treatment & Wellness Centres (1st ed., effective 1 Apr 2025)** | Covers Panchakarma clinics, replacing the 2017 Panchakarma clinic standards | **Step 2, year 2.** A strong "accredited Panchakarma" trust signal. |
| Entry-Level Ayush Hospital / **Ayush Hospital accreditation** (Ayurveda hospital standards, 2nd ed.: 98 standards, 590 objective elements) | Inpatient facilities | Only if Model C is ever built |

**NABH does not license any service.** Legality comes from your practitioner registration (MCIM), establishment registration, drug licences and applicable Acts. NABH certifies quality systems only.

### 7.3 Maharashtra / India compliance checklist

| Area | Requirement | Status to confirm |
|---|---|---|
| Practitioner | Registration with the **Maharashtra Council of Indian Medicine** for every Ayurveda doctor; MMC registration for any visiting OBG | |
| Establishment | Shop & Establishment (Gumasta). The **Bombay Nursing Homes Registration Act 1949** applies only if you admit patients. The **Maharashtra Clinical Establishments Bill 2026** (pending) would require registration for all clinical establishments, including OPDs. | |
| Biomedical waste | BMW Management Rules 2016: MPCB authorisation, colour-coded segregation, CBWTF contract | |
| Medicines | Dispensing to **your own patients** by a registered practitioner is generally exempt from a sale licence. **Sale to non-patients or online needs a licence.** In-house manufacturing needs an Ayush manufacturing licence (state licensing authority) and GMP. | |
| Advertising | **DMR Act 1954** (sterility in women and impotence are scheduled); **Rule 170 omitted** (Supreme Court vacated the stay, Aug 2025), but the DMR Act, the CCPA misleading-advertisement guidelines (2022) under the Consumer Protection Act 2019, ASCI healthcare guidelines and the **Supreme Court's self-declaration requirement for advertisers (2024)** all still apply. Also the practitioner ethics regulations on self-promotion. | |
| Sex selection | **PCPNDT Act**: no messaging or products implying sex selection. Ultrasound on premises needs PCPNDT registration; outsource it instead. | |
| ART | The **ART (Regulation) Act 2021** governs ART clinics, including IUI. **Do not perform IUI** or handle gametes. Uttarbasti is not ART, but never describe it as an IVF/IUI alternative. | |
| Data | **DPDP Act 2023 + Rules**: consent notices, purpose limitation, a breach process; specific consent for testimonials and photos | |
| Tax | GST exemption for healthcare services; medicines as composite supply (CA opinion) | |
| Insurance | Professional indemnity for each doctor; clinic public liability | |

### 7.4 Location comparison

| Location | Catchment fit | Competition | Rent | Role |
|---|---|---|---|---|
| **Katraj** (existing) | South Pune, mid-income families, Kondhwa/Bibwewadi/Dhankawadi/Satara Road; adjacent to ISKCON NVCC footfall; Bharati Vidyapeeth hospital nearby | **Gynoveda Kondhwa (Lulla Nagar, ~4–5 km)**; Oasis and Nova at Kondhwa–Lulla Nagar (~5–8 km); Ayurgarbh (Undri) | Low | **Pilot and procedure hub** |
| **Baner / Aundh** | Most affluent western belt, young professionals | Indira IVF Baner, Nova Baner, Aatreya Ayurvedic Infertility Clinic, Progenesis (Aundh) | High | **Location 2** (Model B), ideally as a consult-only satellite first |
| **Wakad / Hinjewadi** | 3 L+ IT workforce, young couples, high planner (segment A) density | Fewer specialist fertility clinics (verify) | Medium–high (~₹69/sq ft Grade-A) | Corporate wellness talks; a later satellite |
| **Kharadi / Viman Nagar** | IT plus NRIs, airport access (segment S6) | Nova Kharadi | High | Location 3 |
| Kothrud | Established Marathi middle-upper class, strong Ayurveda affinity | Many independents | Medium | An alternative to Baner |

**Hub-and-spoke recommendation:** keep **all procedures at Katraj** (one sterile room, one governance system). Open **consult-only satellites** (a rented doctor cabin 2 half-days a week, ₹15–30 k/month) in Baner and Wakad once Katraj demand is proven. Couples travel 30–40 minutes for procedures, which is acceptable for 6–10 visits.

### 7.5 ISKCON partnership (Katraj NVCC; Hinjewadi)

- **Verified:** ISKCON NVCC (Katraj–Kondhwa Road) lists "yoga, naturopathy and Ayurvedic consultation" among its allied services and has large weekly footfall and a guest house. **Not verified:** a dedicated ISKCON Hinjewadi temple. One travel blog lists a Hinjewadi address; other sources place the main temple in Kondhwa. Confirm directly with ISKCON Pune.
- **What works:** monthly **"Preparing for Parenthood" talks** (Garbh Sanskar is a culturally familiar entry point for this audience), healthy-pregnancy diet workshops, a satvik nutrition partnership, and access to ISKCON's international congregation for segment S6.
- **Guardrails:**
  1. No commission or fee-splitting on patients.
  2. **Keep Aastik Fertility's clinical brand secular and evidence-led.** A religious association can alienate the cosmopolitan Baner/Kharadi buyer and invites "pseudoscience" framing.
  3. No Garbh Sanskar claims about the baby's intelligence, character, sex or genetics.
  4. Written MoU covering co-branding, data and content approval.
- **Commercial value:** treat it as a **low-CAC channel** (perhaps 15–25% of segment-A leads), not a location strategy.

---

## 8. THE ₹1,000 CRORE QUESTION (sceptical banker)

**Math:** EV ₹1,000 Cr ≈ ₹200 Cr revenue × 5× (healthcare services multiple for a profitable, growing chain), or ₹120–150 Cr × 7–8× with 20%+ EBITDA and a product engine.

| Engine | What it takes to reach the number |
|---|---|
| Clinics | A mature clinic doing 30–40 new couples/month at ~₹68 k average plus OPD and medicines ≈ ₹3–3.5 Cr/year. **About 35–40 clinics ≈ ₹120 Cr.** |
| Medicines (own SKUs, prescribed in-programme and repeat purchases) | ₹40–60 Cr |
| Digital tier (tele-led V1 for non-Pune couples) | ₹20–40 Cr, but this means competing with Gynoveda on CAC |
| **Total** | ₹180–220 Cr in **year 7–9**, with ₹80–150 Cr of cumulative capital |

**Reality check:** Gynoveda, with ~$11 M raised and 7+ years of trading, reports about ₹68 Cr revenue and a small loss. That is the category ceiling evidence so far. **₹1,000 Cr is a 10-year outcome if three things hold:** the outcomes registry proves meaningfully better-than-baseline results, gynaecologist/IVF referral partnerships scale beyond Pune, and the doctor model is protocolised enough that clinics run without the founder.

**Credible valuation steps:**

| Milestone | Valuation range |
|---|---|
| End of pilot (month 9): 50+ couples, outcome report | Not a raise event. Self-funded. |
| Year 2: ₹3–5 Cr fertility revenue, 2–3 Pune sites | ₹25–50 Cr pre-money (angel/seed) |
| Year 3–4: ₹10–15 Cr, 6–10 sites across 2 cities, published outcomes | ₹60–120 Cr |
| Year 6+: ₹60–100 Cr, 25+ sites | ₹350–600 Cr |

---

## 9. PILOT PLAN AND 12-MONTH NUMBERS (Model A)

### 9.1 Assumptions

- Mix: 40% V1 / 50% V2 / 10% V3. **Average ticket ₹67,600; average direct cost ₹23,000.**
- Enrolments ramp 0, 1, 2, 3, 4, 5, 6, 7, 8, 8, 9, 10 (months 1–12) = **63 couples**.
- Funnel: lead → first consult 15–25%; consult → enrolment 25–35%. For 10 enrolments/month you need about 30–40 consults and about 150–250 qualified leads.
- Incremental fixed costs: marketing ₹1.25 L/month; other ₹1.2 L/month (coordinator ₹30 k, therapist ₹25 k, visiting OBG/PTSR ₹30 k, tools/content ₹20 k, misc ₹15 k).

### 9.2 Year-1 result (bookings basis, ₹ L)

| Line | ₹ L |
|---|---|
| Programme bookings (63 × ₹67.6 k) | 42.6 |
| Direct costs (63 × ₹23 k) | (14.5) |
| Marketing | (15.0) |
| Other incremental fixed | (14.4) |
| **Operating contribution, year 1** | **≈ (1.3)** |
| Capex (Model A) | (6–9) |
| Working capital and buffer | (4–6) |
| **Total cash needed** | **₹12–18 L** |
| Year-1 effective CAC | ₹15 L ÷ 63 ≈ **₹23.8 k** (should fall to ₹12–15 k by month 12) |
| **Month-12 run-rate** | Bookings ₹6.8 L − direct ₹2.3 L − fixed ₹2.45 L ≈ **+₹2.0 L/month** |

**Funding:** founder capital, friends & family and grants into the **new Aastik Fertility entity**. Raise from outside investors only after the month-9 gate. The curcumin venture's money and investors stay completely separate (0.4).

### 9.3 Gate at month 9 (go / no-go for Model B)

| Metric | Go threshold |
|---|---|
| Enrolled couples (cumulative) | ≥ 40 |
| Consult → enrolment | ≥ 25% |
| Effective CAC | ≤ 20% of average ticket |
| Drop-out / refund | ≤ 15% |
| Referral-clock compliance | 100% (audited) |
| Adverse events from procedures | 0 serious |
| Active OBG/IVF referral partners | ≥ 5 |
| NPS (month-3 survey) | ≥ 50 |
| Outcome registry completeness | ≥ 90% of enrolled couples with baseline + 6-month data |

### 9.4 First 90 days

1. **Weeks 1–2:** fix the Part 1 data gap (Maps, Instagram, YouTube exports). Clean all claims. Draft consent forms, refund policy and the referral-clock SOP.
2. **Weeks 2–4:** sign a visiting OBG and a Prasuti Tantra consultant. Partner lab B2B rates. Upgrade the procedure room. Start the CTRI observational registry protocol via your AIIA/IIT network.
3. **Weeks 3–6:** run 30 couple + 25 professional interviews (3.3). Launch the ₹2,000 deposit founding-cohort test (target 15 deposits).
4. **Weeks 6–8:** soft-launch V1/V2. Two ISKCON NVCC talks, 2 corporate talks in Hinjewadi, 8 OBG clinic visits, and 12 education reels on a separate fertility handle.
5. **Week 12:** first internal metrics review against 9.3.

---

## 10. SOURCES (accessed via web search, 23 Nov 2026)

**First-hand page reads (headless browser, 23 Nov 2026):**
- Google Maps listing (limited view): [maps.app.goo.gl/WmjLY88Hthatshca6](https://maps.app.goo.gl/WmjLY88Hthatshca6)
- YouTube oEmbed for [_pVvoGZpF7Y](https://youtu.be/_pVvoGZpF7Y) (title and channel only)
- Aastik site: [home](https://aastikayurveda.com/), [therapies](https://aastikayurveda.com/therapies/), [about](https://aastikayurveda.com/about-us/), [IGAC](https://aastikayurveda.com/innovation-growth-advisory-council-igac/), [blog (spam)](https://aastikayurveda.com/blog/), [shop](https://aastikayurveda.com/shop/)
- Gynoveda: [home](https://gynoveda.com/), [clinics](https://gynoveda.com/pages/gynoveda-clinic-near-me/), [Pune clinics](https://gynoveda.com/pages/clinics-available/pune/), [how it works](https://gynoveda.com/pages/gynoveda-fertility-clinic-how-it-works/), [fertility tablets](https://shop.gynoveda.com/products/fertility-support-ovulation-for-pregnancy), [refund policy](https://gynoveda.com/pages/returns-refunds-policy/), [IVF vs Ayurveda](https://gynoveda.com/compare-ivf-vs-ayurveda/), [about](https://gynoveda.com/pages/about/)
- Not readable: Instagram (login wall), YouTube watch page (bot check), Google reviews (sign-in required)

**Gynoveda**
- Series A: [Entrepreneur India](https://india.entrepreneur.com/news-and-trends/gynoveda-raises-10-million-in-series-a-funding-round/447816), [Inc42](https://inc42.com/buzz/fireside-ventures-backed-gynoveda-secures-10-mn-funding-to-strengthen-its-offline-play), [FemTech Insider](https://femtechinsider.com/gynoveda-series-a/), [Indian Startup News](https://indianstartupnews.com/news/femtech-startup-gynoveda-raises-10m-in-a-series-a-round-led-by-india-alternatives-fund)
- Financials: [Inc42 company page](https://inc42.com/company/gynoveda/captable/), [TheKredible](https://thekredible.com/company/gynoveda/overview), [CB Insights](https://www.cbinsights.com/company/gynoveda-femtech/financials)
- Pune clinics: [Digital Health News](https://www.digitalhealthnews.com/femtech-startup-gynoveda-unveils-second-clinic-in-pune), [FemTech Insider](https://femtechinsider.com/gynoveda-pune-clinic/), [Digital Terminal](https://digitalterminal.in/health-tech/gynoveda-opens-second-fertility-clinic-in-pune)
- Products and reviews: [Gynoveda shop page](https://shop.gynoveda.com/products/fertility-support-ovulation-for-pregnancy), [Flipkart reviews](https://www.flipkart.com/gynoveda-jeehv-ayurvedic-fertility-supplement-ovulation-natural-pregnancy-240-tablets/product-reviews/itm853097a710789?pid=AYDGAYN9V39WHZRA&lid=LSTAYDGAYN9V39WHZRAXJE8QC&cat=OverTheCounterMedicine&vert=FemaleDisorders), [Amazon.in](https://www.amazon.in/Gynoveda-Ayurvedic-Management-Imbalance-Pregnancy/dp/B09CDBWYMW), [Quora](https://www.quora.com/Is-the-Gynoveda-medicine-good-for-PCOS-Can-I-take-this), [Tenereteam](https://gynoveda.tenereteam.com/)

**IVF market and chains**
- Pune IVF pricing: [Indira IVF Pune cost](https://www.indiraivf.com/ivf-cost-in-pune), [Nova IVF Pune cost](https://www.novaivffertility.com/ivf-cost/ivf-cost-in-pune), [Birla Fertility](https://birlafertility.com/?p=10939), [Oasis](https://oasisindia.in/blog/ivf-treatment-cost-in-pune)
- Indira IVF and Gaudium: [Kotak Neo](https://www.kotakneo.com/ipo/indira-ivf-ltd-ipo/), [Business Standard](https://www.business-standard.com/markets/ipo/indira-ivf-refiles-draft-ipo-via-confidential-route-gaudium-to-follow-125071600610_1.html), [Gaudium expansion](https://www.indianpharmapost.com/healthcare/gaudium-ivf-begins-19-clinic-expansion-outlined-in-ipo-roadmap-20981)
- Pune centres: [Oasis Kondhwa](https://oasisindia.in/ivf-fertility-centres/pune/kondhwa/), [Nova Lulla Nagar](https://novaivffertility.com/ivf-centre/pune/fertility-clinic-lulla-nagar), [Indira IVF Baner](https://www.punekarnews.in/indira-ivf-inaugurates-new-fertility-centre-in-baner-pune/), [Practo Pune infertility](https://www.practo.com/pune/infertility-specialist)
- Market size: [IMARC](https://www.imarcgroup.com/india-in-vitro-fertilization-market), [BioSpectrum 2026 trends](https://www.biospectrumindia.com/public/news/17/27214/top-trends-driving-indias-ivf-industry-in-2026.html), [SCMP](https://www.scmp.com/week-asia/health-environment/article/3256105/indian-couples-are-struggling-conceive-why-worlds-most-populous-nation-facing-challenge), [Pinky Promise](https://www.indianpharmapost.com/healthcare/pinky-promise-opens-first-physical-clinic-in-mumbai-expands-womens-hybrid-healthcare-model-19753)

**Ayurveda competitors**
- [AyurVAID infertility programmes](https://ayurvaid.com/diseases/infertility/), [Apollo AyurVAID FY26 expansion](https://www.deccanherald.com/amp/story/business%2Fcompanies%2Fapollo-ayurvaid-to-expand-pan-india-in-fy26-3628389)
- Pune independents: [Aatreya (Baner)](https://www.practo.com/pimpri-chinchwad/clinic/aatreya-ayurvedic-panchakarma-infertility-clinic-baner/), [Ayurgarbh (Undri)](https://www.practo.com/pune/clinic/ayurgarbh-ayurvedic-chikitsalay-and-panchkarma-center-undri), [Shree Sai (Nigdi)](https://www.practo.com/pune/clinic/shree-sai-ayurvedic-panchakarma-clinic-infertility-research-clinic-nigdi), [Aasha Ayurveda](https://aashaayurveda.blogspot.com/2025/09/ayurvedic-care-for-female-infertility.html)

**Evidence**
- [PCOS scoping review](https://researchers.westernsydney.edu.au/en/publications/a-scoping-review-of-ayurveda-studies-in-women-with-polycystic-ova/), [Ayurveda infertility systematic review (Cureus 2024)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11073818/), [Female reproductive health review](https://pubmed.ncbi.nlm.nih.gov/38558676/)
- [Ashwagandha oligospermia RCT](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3863556/)
- [Uttarbasti tubal block study (AYU 2010)](https://pmc.ncbi.nlm.nih.gov/articles/PMC3202247)
- Preconception care: [Evidence-based preconceptional lifestyle interventions](https://pubmed.ncbi.nlm.nih.gov/23985430/), [UCL clinical review](https://discovery.ucl.ac.uk/id/eprint/10127080/3/Stephenson_A%20wake-up%20call%20for%20preconception%20health-%20a%20clinical%20review_AAM.pdf), [RACGP](https://www.racgp.org.au/ajgp/2018/july/preconception-care)
- Garbh Sanskar criticism: [The Wire](https://science.thewire.in/law/rss-kolkata-super-baby/), [Business Standard](https://business-standard.com/article/current-affairs/from-cure-in-cow-urine-to-superior-child-pseudoscience-inviting-research-118030200581_1.html)

**Regulation**
- DMR Act: [India Code](https://www.indiacode.nic.in/indiacode/bitstream/123456789/1412/1/A1954-21.pdf), [ASCI 2019 report](https://www.ascionline.in/wp-content/uploads/2022/09/asci-march-2019-ccc-recom-1.pdf), [Delhi AYUSH notice](https://ayush.delhi.gov.in/sites/default/files/ayush/important-news/ad_merge.pdf)
- Rule 170: [LiveLaw (stay vacated)](https://www.livelaw.in/amp/top-stories/supreme-court-vacates-stay-on-ayush-ministrys-notification-that-permitted-advertisements-of-ayurvedic-unani-siddha-drugs-300536), [SC Observer](https://www.scobserver.in/journal/patanjali-contempt-case-blatant-violations-expanded-scope-repeated-scoldings-and-the-flip-flip-on-rule-170/), [AZB Partners](https://www.azbpartners.com/?p=87501)
- NABH: [Ayush Treatment & Wellness Centre standards](https://portal.nabh.co/images/Standards/NABH%20Accreditation%20Standards%20for%20Ayush%20Treatment%20and%20Wellness%20Centres%20-%201st%20Edition.pdf), [Entry-level Ayush centres](https://nabh.co/programmes/entry-level-ayush-centres-certification-programme/), [Entry-level Ayush hospitals](https://nabh.co/programmes/entry-level-ayush-hospitals-certification-programme/), [FAQ](https://portal.nabh.co/Images/pdf/FAQ%20Ayush%20Entry%20Hospital%20&%20Center.pdf), [Ayurveda brochure](https://testing.nabh.co/wp-content/uploads/2025/07/General-Information-Brochure_Ayurveda.pdf)
- Maharashtra: [Clinical Establishments Bill 2026 (PRS)](https://prsindia.org/bills/states/the-maharashtra-clinical-establishments-registration-and-regulation-bill-2026), [PMC notices (Medical Dialogues)](https://medicaldialogues.in/state-news/maharashtra/pune-37-private-hospitals-get-notices-over-regulatory-violations-162244)
- NCISM: [BAMS Panchakarma curriculum](https://ncismindia.org/2.%20NCISM_IIIBAMS_AyUG-PK.pdf) (no rate schedule found)

**Location and ISKCON**
- [ISKCON Pune](https://www.iskconpune.com/?p=10722), [ISKCON centres directory](https://centres.iskcon.org/centre/iskcon-pune-sri-sri-radha-kunjabihari-temple/), [Hinjewadi temples blog](https://tripxl.com/blog/temples-in-hinjewadi/)
- [Cushman & Wakefield Pune](https://www.cushmanwakefield.com/en/India/insights/pune-marketbeat), [Punekar News (Knight Frank rents)](https://www.punekarnews.in/?p=239647), [Sobha Pune workforce](https://www.sobha.com/blog/pune-workforce-residential-housing-demand/), [HomeBazaar](https://homebazaar.com/knowledge/pune-real-estate)

**From my training, not re-verified this session (confirm before relying):** IRDAI's standard exclusion of sterility/infertility and its Ayush-hospital definition; the details of the international PCOS guideline (2023); WHO semen analysis 6th edition; PCPNDT advertising provisions; DPDP Rules; GST exemption entries; ethics rules on referral commissions.
