# Legal Verification Prompts
## Questions for Legal AI Agent / Healthcare Privacy Counsel

**⚠️ CRITICAL NOTE**: You mentioned SHA256 hashes for Facebook upload. This changes the compliance analysis significantly. These prompts address hashed identifiers specifically.

---

## SECTION 1: QUESTIONS FOR YOUR LAWYER

### Copy-Paste These Prompts into Your Legal AI Agent

---

#### **PROMPT 1: SHA256 Hash Classification Under HIPAA**

```
I work with a company that receives SHA256 hashed email addresses and/or 
device identifiers from data vendors for the purpose of creating Facebook 
Custom Audiences. 

Context:
- We receive SHA256 hashes (not plain text emails or device IDs)
- We upload these hashes to Facebook's Custom Audience platform
- The original data comes from consumer search behavior (not healthcare providers)
- We do NOT have access to the unhashed/original identifiers
- We combine this with keyword search intent data
- Target use case: pharmaceutical DTC advertising on Facebook/Instagram

Questions:
1. Are SHA256 hashed email addresses considered PHI under HIPAA?
2. Are SHA256 hashed device identifiers (mobile ad IDs) considered PHI?
3. Does receiving hashed identifiers make us a "business associate" under HIPAA?
4. If the vendor provides hashes + health-related keywords, does the combination 
   create PHI where none existed before?
5. What documentation should we require from vendors to prove their hashing 
   methodology is HIPAA-compliant (if applicable)?

Please cite specific HIPAA regulations (45 CFR 164.514 for de-identification 
standards) in your analysis.
```

---

#### **PROMPT 2: Pseudonymous Data and State Privacy Laws**

```
Our company receives SHA256 hashed identifiers (email hashes, mobile ad ID hashes) 
combined with keyword search data for marketing purposes.

Questions:
1. Under CCPA/CPRA, are SHA256 hashed emails considered "personal information"?
2. What about hashed mobile advertising IDs (IDFA, GAID)?
3. Does hashing provide a "reasonable level of protection" under state privacy laws 
   or is it still considered personal data?
4. Are there different standards between:
   - One-way hashing (irreversible)
   - Salted hashing
   - Hashing with lookup tables available
5. If we receive hashed data and upload to Facebook (who may be able to match/resolve),
   what are our compliance obligations?
6. Does B2B marketing exemption apply if we're targeting healthcare professionals 
   using hashed identifiers?

Please address California, Virginia, Colorado, Connecticut, and Utah privacy laws.
```

---

#### **PROMPT 3: Facebook Custom Audiences and Health Data**

```
We upload SHA256 hashed identifiers to Facebook Custom Audiences for 
pharmaceutical/healthcare marketing campaigns.

Context:
- Facebook matches hashes to user accounts
- We also upload health-related targeting criteria (condition interest, keywords)
- Campaigns are DTC drug advertisements or HCP targeting

Questions:
1. Does Facebook's Custom Audience Terms of Service restrict health-related use 
   of hashed uploads?
2. Are there specific Facebook policies about pharmaceutical advertising using 
   Custom Audiences?
3. What is Facebook's classification of SHA256 hashed emails - do they treat 
   them as personal data?
4. If Facebook can resolve hashes to real users, does that make the hashes 
   "linkable" to individuals under privacy law?
5. What contractual obligations do we have to Facebook regarding the source 
   and permissioning of hashed data?
6. Are there restrictions on using Facebook Custom Audiences for clinical trial 
   recruitment?

Please reference Facebook's Business Tools Terms and Advertising Policies.
```

---

#### **PROMPT 4: FDA Regulations and Targeting Methods**

```
Our company provides audience data for pharmaceutical DTC advertising. 
Specifically, we enable targeting based on:
- SHA256 hashed identifiers (uploaded to Facebook)
- Keyword search behavior (e.g., "buy diabetes medication")
- Condition-based interest signals

Questions:
1. Does FDA consider the TARGETING METHOD (how we select audiences) as part of 
   their advertising regulations, or only the ad CONTENT?
2. Are there FDA restrictions on using "active search behavior" for prescription 
   drug advertising targeting?
3. Is targeting people who searched for "buy [drug name]" considered 
   "reminder advertising" or "help-seeking" under FDA guidance?
4. Do we have any liability exposure if a client uses our audiences for 
   off-label promotion (our contract prohibits this, but what's our risk)?
5. Are there specific restrictions for controlled substance advertising using 
   intent-based targeting?
6. What is the distinction between targeting "patients" vs "consumers" under 
   FDA guidance, and does our method fall into either category?

Please reference FDA DTC Advertising Guidance and any relevant warning letters.
```

---

#### **PROMPT 5: Vendor Liability and Contractual Protections**

```
We receive SHA256 hashed identifiers and keyword data from third-party vendors 
(d18, d3 - data aggregators).

Questions:
1. What contractual representations should we require from vendors regarding:
   - Their legal authority to provide hashed data
   - Consent/permissioning status of the original data subjects
   - Compliance with privacy laws in data collection
   - Indemnification for compliance violations
   
2. If a vendor misrepresented their data collection practices (e.g., lacked 
   proper consent), what is our liability exposure?

3. Should we require vendors to obtain and maintain cyber liability insurance 
   that names us as additional insured?

4. What audit rights should we have to verify vendor compliance?

5. If a vendor's data contains improperly obtained health information, and we 
   receive it as hashes, are we liable for their violation?

6. What "safe harbor" provisions can we include in contracts to minimize liability?

Please provide recommended contract language for these provisions.
```

---

#### **PROMPT 6: FTC and Unfair Practices Considerations**

```
Our marketing claims about data compliance:
- We tell clients our data is "HIPAA-compliant" and "no PII"
- We state data is "anonymized" and "de-identified"
- We claim "no PHI" in our audience data

Context:
- We receive SHA256 hashed identifiers
- We receive keyword search data including health terms
- We deliver to Facebook, DSPs, and client S3 buckets

Questions:
1. Are our "HIPAA-compliant" and "no PII" claims potentially misleading if we 
   receive SHA256 hashed identifiers?
2. Does FTC consider SHA256 hashed data "de-identified" or "anonymous" for 
   marketing purposes?
3. What substantiation do we need for compliance claims in our sales materials?
4. If we discover our vendor provided improperly sourced data, what are our 
   obligations under FTC Act Section 5 (unfair/deceptive practices)?
5. What disclosures should we include in our marketing to avoid FTC scrutiny?

Please reference FTC guidance on health claims, data practices, and substantiation.
```

---

#### **PROMPT 7: International Considerations (GDPR, PIPEDA)**

```
Our vendors may collect data internationally, and we may deliver audiences to 
pharmaceutical companies with global operations.

Context:
- Data vendors may collect search behavior from EU/UK/Canadian users
- We upload hashed data to Facebook (international data transfers)
- Clients may activate campaigns in multiple countries

Questions:
1. Does GDPR consider SHA256 hashed emails "personal data" under Article 4(1)?
2. What about "pseudonymized data" under GDPR - how is that treated differently?
3. Do we need a Data Processing Agreement (DPA) under GDPR Article 28 if we 
   receive hashed data?
4. What about Canada's PIPEDA - how does it classify hashed identifiers?
5. If we receive EU user data without appropriate legal basis (consent/Legitimate 
   Interest), what is our liability?
6. Should we restrict our data to US-only audiences to avoid international 
   compliance complexity?

Please address data transfer mechanisms (SCCs, adequacy decisions) if applicable.
```

---

#### **PROMPT 8: Practical Risk Assessment**

```
Given our business model, please provide a risk assessment:

Our Activities:
1. Receive SHA256 hashed emails and mobile ad IDs from data vendors
2. Receive keyword search data (including health terms like "diabetes," "weight loss")
3. Combine hashes + keywords to create "intent-based audiences"
4. Upload hashed audiences to Facebook Custom Audiences
5. Deliver audience files to client S3 buckets for DSP activation
6. Target: Pharmaceutical DTC campaigns, HCP marketing

Questions:
1. Rank-order the compliance risks from highest to lowest probability/severity
2. What is our worst-case regulatory enforcement scenario?
3. What is the likelihood of a class action lawsuit, and what would trigger it?
4. What insurance coverage do we need (cyber, E&O, D&O)?
5. What internal compliance program elements are essential vs. nice-to-have?
6. Should we pursue any regulatory pre-clearance or opinion letters?
7. What "red flags" would require immediate legal review?

Please provide practical, prioritized recommendations.
```

---

## SECTION 2: QUESTIONS FOR YOUR DATA VENDORS (d18, d3)

### Vendor Due Diligence Checklist

Send these questions to your data vendors and require written responses:

---

#### **DATA SOURCING AND COLLECTION**

```
1. ORIGIN OF DATA
   - What is the original source of the search behavior data you provide?
   - Do you collect directly from publishers/sites or purchase from intermediaries?
   - What jurisdictions do you collect data from (US-only or international)?

2. CONSENT AND NOTICE
   - What notice is provided to users whose search behavior is collected?
   - Do you obtain affirmative opt-in consent, or rely on implied consent/TOS?
   - Please provide copies of your consumer-facing privacy notices
   - Do you honor Global Privacy Control (GPC) or Do Not Track signals?

3. DATA MINIMIZATION
   - What specific data elements do you collect at the point of collection?
   - Do you collect any health information beyond search queries?
   - Do you collect precise geolocation data?
```

---

#### **HASHING AND IDENTIFIERS**

```
4. HASHING METHODOLOGY
   - Do you hash identifiers before transmitting to kwca, or do we receive raw data?
   - What hashing algorithm do you use (SHA256, MD5, etc.)?
   - Do you use "salting" in your hashing process?
   - Do you maintain lookup tables that can reverse the hashes?
   - How long do you retain the original (unhashed) identifiers?

5. IDENTIFIER TYPES
   - What specific identifiers do you provide (email hashes, MAID hashes, etc.)?
   - Are these deterministic or probabilistic identifiers?
   - Do you provide any cross-device linking or graph data?
   - What is the average match rate when these hashes are uploaded to Facebook?

6. PSEUDONYMIZATION CLAIMS
   - Do you classify your hashed data as "de-identified," "pseudonymized," or "anonymous"?
   - What legal basis supports this classification?
   - Have you obtained a legal opinion on the status of your hashed data under HIPAA?
```

---

#### **HEALTH DATA SPECIFICS**

```
7. HEALTH DATA HANDLING
   - Do you consider search queries about medical conditions to be "health information"?
   - Have you assessed whether your data constitutes PHI under HIPAA?
   - Do you have any Business Associate Agreements (BAAs) with healthcare entities?
   - Do you filter or exclude any sensitive health categories (HIV, mental health, abortion, etc.)?

8. PHARMACEUTICAL USE CASE
   - Are you aware that kwca uses your data for pharmaceutical DTC advertising?
   - Do you have any restrictions on use for prescription drug marketing?
   - Have you worked with other pharmaceutical marketers using this same data?

9. PROHIBITED DATA
   - Do you ever provide: medical records, prescription data, claims data, 
     or data from healthcare providers?
   - Do you work with any HIPAA-covered entities?
   - Do you obtain data from health apps or wearables?
```

---

#### **COMPLIANCE AND CERTIFICATIONS**

```
10. REGULATORY COMPLIANCE
    - Are you compliant with CCPA/CPRA? Please provide evidence.
    - Are you compliant with GDPR (if applicable)?
    - Have you completed a HIPAA risk assessment?
    - Do you have SOC 2 Type II certification?
    - Are you NAI or DAA compliant?

11. AUDIT AND VERIFICATION
    - Will you provide copies of your privacy policies and terms of service?
    - Can we review your data processing agreements?
    - Do you undergo third-party privacy audits?
    - Can we conduct our own audit of your practices (and what would that cost)?

12. INSURANCE
    - Do you carry cyber liability insurance?
    - What are your coverage limits?
    - Will you add kwca as additional insured?
```

---

#### **CONTRACTUAL TERMS**

```
13. INDEMNIFICATION
    - Will you indemnify kwca for violations arising from your data collection practices?
    - What is the cap on your indemnification liability?
    - Do you require us to indemnify you for anything?

14. REPRESENTATIONS AND WARRANTIES
    - Can you warrant that you have legal authority to provide this data?
    - Can you warrant that your data collection complies with all applicable laws?
    - Can you warrant that no PHI is included in the data provided?

15. AUDIT RIGHTS
    - Do we have the right to audit your data sources and practices?
    - How much notice is required?
    - Who bears the cost of the audit?

16. TERMINATION
    - What happens to data we've already received if you terminate?
    - Do we have to delete or return data upon termination?
    - What triggers immediate termination rights?
```

---

#### **OPERATIONAL QUESTIONS**

```
17. DATA QUALITY
    - What is the typical refresh frequency of your data?
    - How far back does the search behavior data go (lookback window)?
    - What is your methodology for determining "intent" vs. incidental searches?
    - What are your match rates to major platforms (Facebook, The Trade Desk)?

18. EXCLUSIONS AND FILTERS
    - Can you exclude data from users under 18?
    - Can you exclude sensitive health categories upon request?
    - Can you provide US-only data (exclude international users)?
    - Can you filter out healthcare professionals (if needed for consumer-only campaigns)?

19. TRANSPARENCY
    - Can you provide sample data for legal review?
    - Can you explain exactly how a record is created from collection to delivery?
    - Who are your upstream data providers (if any)?
```

---

## SECTION 3: RED FLAGS TO WATCH FOR

### Vendor Responses That Should Concern You

| Red Flag | What It Means | Action |
|----------|---------------|--------|
| "We don't need user consent" | May violate state privacy laws | Require documentation |
| "Our hashing is proprietary" | Can't verify security | Demand technical details |
| "We've never been audited" | No third-party validation | Require audit or walk away |
| "We can't share our privacy policy" | Hiding something | Major red flag |
| "This data isn't regulated" | Legal ignorance or willful blindness | Get legal review |
| "Everyone does it this way" | Not a legal defense | Not reassuring |
| Refuses to indemnify | Won't stand behind their data | Negotiate or walk |
| No insurance | No recourse if breach | Require coverage |
| Vague about sources | Could be improperly obtained | Require transparency |
| Won't answer specific questions | Likely non-compliant | Walk away |

---

## SECTION 4: DOCUMENTS TO REQUEST

### From Vendors

- [ ] Signed Data Processing Agreement (DPA)
- [ ] Business Associate Agreement (BAA) - if they claim HIPAA compliance
- [ ] Privacy Policy (consumer-facing)
- [ ] Data Processing Addendum
- [ ] SOC 2 Type II report
- [ ] Cyber liability insurance certificate
- [ ] Sample data dictionary
- [ ] Legal opinion letter (if available)
- [ ] List of upstream data providers
- [ ] Consent flow documentation

### For Your Records

- [ ] All vendor responses to due diligence questions
- [ ] Email chains documenting compliance discussions
- [ ] Legal review memos
- [ ] Internal risk assessment
- [ ] Insurance policies (yours and theirs)
- [ ] Incident response plan
- [ ] Data retention/deletion policies

---

## SECTION 5: IMMEDIATE ACTION ITEMS

### Priority 1 (This Week)

1. **Get legal review of SHA256 hash status** - This is your biggest open question
2. **Request vendor responses** to the due diligence questions above
3. **Review Facebook Business Tools Terms** regarding Custom Audiences
4. **Document current practices** in case of future audit

### Priority 2 (This Month)

1. **Update contracts** with vendors to include required provisions
2. **Review insurance coverage** (cyber, E&O, D&O)
3. **Create internal compliance documentation**
4. **Train sales team** on approved messaging (avoid overclaiming)

### Priority 3 (This Quarter)

1. **Consider privacy audit** by third party
2. **Evaluate US-only data restriction**
3. **Develop incident response plan**
4. **Create vendor monitoring program**

---

*Generated: 2026-03-10*  
*Purpose: Upstream legal verification for kwca data practices*  
*Critical Issue: SHA256 hashed identifiers and their regulatory classification*

**⚠️ REMINDER**: These are prompts for discussion with qualified legal counsel. This document does not constitute legal advice.
