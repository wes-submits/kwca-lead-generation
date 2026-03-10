# Healthcare Marketing Compliance Guide
## Intent Data & Privacy Requirements for Healthcare Audiences

**⚠️ DISCLAIMER**: This guide is for educational and sales enablement purposes only. It does not constitute legal advice. Always consult qualified healthcare privacy counsel for specific compliance decisions.

---

## Executive Summary

**The Core Question**: Can we legally use intent data for healthcare marketing?  
**The Answer**: Yes, with proper understanding of what intent data is (and isn't) under healthcare privacy laws.

**Key Distinction**:
- **PHI (Protected Health Information)**: Regulated by HIPAA — kwca does NOT use this
- **PII (Personally Identifiable Information)**: Various regulations — kwca does NOT use this
- **Intent Data (De-identified)**: Search behavior, keyword signals — kwca's product

**Bottom Line**: kwca's keyword-based intent data operates outside HIPAA's scope because it contains no identifiable health information linked to individuals.

---

## REGULATORY LANDSCAPE

### 1. HIPAA (Health Insurance Portability and Accountability Act)

**What HIPAA Regulates**:
- Protected Health Information (PHI)
- Individually identifiable health information
- Created or received by covered entities (healthcare providers, plans, clearinghouses)

**What is PHI?**
```
PHI = Health information + Personal identifiers

Examples of PHI:
- Medical records linked to a name
- Diagnosis + email address
- Treatment + phone number
- Prescription + device ID (if identifiable)

18 HIPAA Identifiers:
1. Names
2. Geographic data (smaller than state)
3. Dates (birth, admission, discharge, death)
4. Phone numbers
5. Fax numbers
6. Email addresses
7. SSN
8. Medical record numbers
9. Health plan beneficiary numbers
10. Account numbers
11. Certificate/license numbers
12. Vehicle identifiers
13. Device identifiers
14. Web URLs
15. IP addresses
16. Biometric identifiers
17. Full-face photos
18. Any other unique identifying number
```

**kwca's Position**:
- ✅ **NO PHI**: We don't have medical records, diagnoses, or treatments
- ✅ **NO Identifiers**: No names, emails, phone numbers, device IDs, IPs
- ✅ **NO Covered Entity Relationship**: We don't work with healthcare providers
- ✅ **De-identified Data**: Only keyword search patterns aggregated at scale

**What kwca Actually Has**:
```
kwca Data Elements:
├── Keyword search terms (e.g., "diabetes management tips")
├── Search category classifications (e.g., "Health & Wellness")
├── Intent scores (calculated engagement metrics)
├── Timestamp (when search occurred, not linked to person)
└── Anonymized audience segments (aggregated patterns)

What we DON'T have:
├── Names
├── Email addresses
├── Phone numbers
├── Medical record numbers
├── Specific diagnoses linked to individuals
├── Treatment histories
├── Doctor-patient relationships
└── Any information that could identify a specific person
```

---

### 2. FDA (Food and Drug Administration) Regulations

**FDA's Role in Healthcare Marketing**:
- Regulates prescription drug advertising (DTC)
- Requires fair balance (benefits + risks)
- Prohibits off-label promotion
- Requires indication-based marketing

**How This Applies to kwca**:

**Audience Targeting (kwca's role)**:  
✅ **Generally Permitted**: Reaching audiences interested in health topics  
⚠️ **Client Responsibility**: What they say in the ad (kwca doesn't control content)

**Key Distinctions**:

| Activity | Regulated By | kwca Involvement | Client Responsibility |
|----------|--------------|------------------|----------------------|
| **Audience Selection** | HIPAA/FDA (indirectly) | Provides intent data | Must ensure audience appropriate |
| **Ad Content** | FDA | None | Full responsibility for claims, fair balance |
| **Landing Pages** | FDA/FTC | None | Must include required safety info |
| **Data Handling** | HIPAA | De-identified only | N/A |

**FDA-Compliant Audience Strategy**:
```
✅ CAN Target (with kwca data):
- People searching for condition awareness terms
- Healthcare professionals seeking clinical information
- Patients researching treatment options (educational)
- Caregivers looking for support resources

⚠️ REQUIRES CARE:
- Direct-to-consumer drug advertising (must follow DTC guidelines)
- Patient recruitment for clinical trials (must follow FDA regulations)

❌ CANNOT Do (regardless of data source):
- Target based on specific prescription history
- Use patient lists from healthcare providers
- Target vulnerable populations inappropriately
- Make unsubstantiated efficacy claims
```

---

### 3. State Privacy Laws

**California Consumer Privacy Act (CCPA) / CPRA**:

**Applicability to kwca**:
- ✅ **Business-to-Business Exemption**: B2B marketing largely exempt
- ✅ **De-identified Data**: Not "personal information" under CCPA
- ✅ **No Sale of Data**: kwca delivers audiences to client buckets (not selling lists)

**Requirements**:
- Privacy policy disclosure (client responsibility)
- Opt-out rights (for personal info, not applicable to de-identified)
- Service provider agreements (kwca acts as service provider)

**Other State Laws**:
| State | Law | kwca Impact |
|-------|-----|-------------|
| Virginia | VCDPA | Minimal (B2B focus, de-identified) |
| Colorado | CPA | Minimal (de-identified exempt) |
| Connecticut | CTDPA | Minimal |
| Utah | UCPA | Minimal |
| Nevada | NRS 603A | Minimal |

**General Principle**: De-identified, aggregated intent data falls outside the scope of most state consumer privacy laws.

---

### 4. FTC (Federal Trade Commission) Guidelines

**Unfair or Deceptive Practices**:
- Prohibits false or misleading advertising
- Requires substantiation of claims
- Covers health claims specifically

**kwca's Role**:
- kwca provides **audience targeting** (who sees the ad)
- **Not responsible** for ad content, claims, or landing pages
- Client must ensure their messaging is FTC-compliant

**Red Flags to Watch For** (Client Education):
```
⚠️ Tell clients to avoid:
- "Miracle cure" language
- Unsubstantiated efficacy claims
- Before/after photos without disclaimers
- Testimonials without typicality disclosures
- Pressure tactics for medical decisions
```

---

### 5. Industry Self-Regulation

**Digital Advertising Alliance (DAA)**:
- Self-regulatory program for online behavioral advertising
- Requires notice and choice for interest-based advertising

**kwca Compliance**:
- kwca data is contextual (keyword-based), not behavioral tracking
- No cross-site tracking or profiling
- No retargeting based on browsing history
- **Likely exempt** from DAA requirements

**Network Advertising Initiative (NAI)**:
- Similar to DAA
- Focus on third-party cookies and tracking

**kwca Position**:
- kwca doesn't use cookies or device tracking
- No persistent identifiers
- **Outside NAI scope**

---

## HOW INTENT DATA IS DIFFERENT

### Intent Data vs. PHI: Side-by-Side

| Characteristic | PHI (Regulated) | kwca Intent Data (Not PHI) |
|----------------|-----------------|---------------------------|
| **Source** | Medical records, EHRs, insurance claims | Search engines, websites |
| **Identifiers** | Name, DOB, MRN, SSN | None (aggregated patterns) |
| **Health Info** | Diagnoses, treatments, prescriptions | Keywords ("diabetes diet") |
| **Linkability** | Can identify specific person | Cannot identify individuals |
| **HIPAA Coverage** | Yes | No |
| **Requires Authorization** | Yes | No |
| **Breach Reporting** | Required | N/A |
| **Retention Rules** | Strict | Standard business practices |

### The "Safe Harbor" Method

**HIPAA Safe Harbor for De-identification**:
```
Under HIPAA §164.514(b), data is de-identified if:
1. All 18 identifiers are removed, AND
2. The covered entity has no actual knowledge that the 
   remaining information could be used alone or in combination 
   to identify an individual

kwca exceeds this standard:
- ✅ Never had identifiers to begin with
- ✅ Data starts as anonymous search patterns
- ✅ No way to re-identify from kwca data alone
```

---

## COMMON OBJECTIONS & RESPONSES

### Objection 1: "Is this HIPAA-compliant?"

**Short Answer**: "kwca's intent data is not subject to HIPAA because it contains no Protected Health Information. We use keyword search patterns, not medical records or identifiable patient data."

**Detailed Response**:
```
"Great question—HIPAA compliance is critical in healthcare marketing.

kwca's data is NOT subject to HIPAA because:

1. We don't have Protected Health Information (PHI)
   - No medical records, diagnoses, or treatments
   - No names, emails, phone numbers, or device IDs
   - Only anonymous keyword search patterns

2. We don't work with covered entities
   - Not a healthcare provider, plan, or clearinghouse
   - Data comes from search behavior, not clinical settings

3. Our data is de-identified by design
   - Aggregated patterns across millions of searches
   - Cannot be linked back to any individual

Think of it like this: If someone searches 'diabetes diet tips' 
on Google, we might capture that keyword pattern—but we don't 
know WHO searched it, just that there's audience interest in 
that topic.

This is similar to how TV advertisers buy health-related 
programming without knowing individual viewers.

Your legal team can review our data dictionary—we're fully 
transparent about what we have (and don't have)."
```

---

### Objection 2: "Can we use this for DTC drug advertising?"

**Short Answer**: "Yes, intent data can be used for audience targeting in DTC campaigns, but ad content must follow FDA guidelines—that's your responsibility, not kwca's."

**Detailed Response**:
```
"Yes, kwca intent data can be used for DTC audience targeting, 
but with important distinctions:

What kwca provides (compliant):
- Audiences interested in condition awareness
- Healthcare professionals researching clinical topics
- Patients seeking educational information

What YOU control (your responsibility):
- Ad content and claims (must include fair balance)
- Landing pages (must include required safety information)
- Targeting parameters (must be appropriate for the indication)

FDA regulates WHAT you say in the ad.
kwca helps you reach WHO might benefit from seeing it.

For DTC campaigns, we recommend:
1. Targeting condition-awareness keywords (not treatment-specific)
2. Educational messaging approach
3. Appropriate frequency capping
4. Clear disclosure of data practices in privacy policy

We've worked with [reference pharma clients] on DTC campaigns—
happy to share how they navigated this."
```

---

### Objection 3: "Does this comply with state privacy laws like CCPA?"

**Short Answer**: "Yes. kwca's de-identified, B2B audience data is exempt from most state consumer privacy laws."

**Detailed Response**:
```
"Yes, kwca's data practices comply with state privacy laws:

CCPA/CPRA (California):
- B2B marketing has a broad exemption
- De-identified data is not 'personal information'
- We operate as a service provider, not a data seller

Other states (Virginia, Colorado, Connecticut, Utah):
- Similar exemptions for B2B use
- De-identified data outside scope
- No consumer-facing data collection

What kwca does:
- Delivers aggregated audience segments to your infrastructure
- No individual-level data
- No sale of personal information
- No direct consumer relationships

What you should do (for compliance):
- Include appropriate disclosures in privacy policy
- Ensure your use aligns with your stated practices
- Maintain data security on your end

We can provide standard contract language our other 
healthcare clients use for their legal teams."
```

---

### Objection 4: "How do we know patients consented to this?"

**Short Answer**: "Consent isn't required because kwca data doesn't identify individuals—it's aggregated search patterns, similar to TV ratings or market research."

**Detailed Response**:
```
"Consent requirements apply to personal data collection.

kwca's data is different:
- No individual is identified in our datasets
- We don't collect data 'about' specific people
- We identify aggregated patterns across millions of searches
- Similar to Nielsen TV ratings or market research

Analogy:
If a TV network knows '2 million people watched a health program,'
they don't need consent from each viewer to sell ads.

Similarly, kwca knows '300K people searched diabetes-related terms'
without knowing who those people are.

For transparency (best practice):
- Your privacy policy should mention use of third-party data
- Include standard industry disclosures
- Provide opt-out where applicable

But consent isn't required for aggregated, de-identified data—
just as you don't need consent to use Nielsen ratings or 
census data."
```

---

### Objection 5: "What about HCP targeting? Is that different?"

**Short Answer**: "Healthcare Professional targeting has fewer restrictions than patient targeting because HCPs are business professionals, not consumers with health privacy concerns."

**Detailed Response**:
```
"Healthcare Professional (HCP) targeting actually has FEWER 
complications than patient targeting:

Why HCP targeting is simpler:
1. HCPs are business professionals, not patients
2. B2B marketing exemptions apply broadly
3. Professional contact information is largely public (NPI registry)
4. HCPs expect professional marketing

kwca's HCP audiences:
- Based on professional behavior (clinical research, medical topics)
- Not derived from patient relationships
- No access to prescriber data or specific prescribing behavior
- Similar to targeting physicians through medical journals

What we provide:
- Audiences interested in medical education topics
- Professionals consuming clinical content
- Segments by specialty (based on content consumption, not NPI)

What we DON'T provide:
- Individual prescriber lists
- Prescribing behavior data
- Patient-HCP relationship data

Platform considerations:
- LinkedIn allows HCP targeting with professional filters
- Some platforms restrict HCP ads (kwca enables off-platform reach)
- Professional messaging has different standards than DTC

Our HCP audiences are particularly valuable because they work
outside platform restrictions."
```

---

## COMPLIANCE BEST PRACTICES

### For kwca (Internal)

1. **Data Minimization**
   - Only collect necessary data for audience building
   - Regular audits of data sources
   - No attempts to enrich with PII

2. **Access Controls**
   - Limit internal access to data
   - Audit logs of data handling
   - Employee training on privacy

3. **Vendor Management**
   - DPA (Data Processing Agreement) with d18, d3
   - Regular compliance reviews of data sources
   - Exit clauses for non-compliance

4. **Documentation**
   - Maintain data lineage records
   - Document de-identification processes
   - Legal opinion letters on file

5. **Security**
   - Encryption at rest and in transit
   - Secure S3 delivery to clients
   - Regular security audits

---

### For Clients (Recommendations)

1. **Privacy Policy Updates**
   - Disclose use of third-party audience data
   - Describe data sources at high level
   - Include opt-out mechanisms

2. **Contract Provisions**
   - Data Processing Addendum (DPA)
   - Business Associate Agreement (BAA) - NOT required for kwca but some clients request
   - Service Provider designation
   - Data deletion requirements

3. **Audience Use Guidelines**
   - Don't attempt to re-identify audiences
   - Don't combine with PHI
   - Use for marketing only (not clinical decisions)
   - Secure storage in client infrastructure

4. **Ad Content Review**
   - FDA approval for DTC (if applicable)
   - Fair balance in messaging
   - Required safety information
   - Substantiation of claims

5. **Documentation**
   - Maintain records of data sources
   - Document targeting criteria
   - Audit trail of audience use
   - Training records for marketing team

---

## COMPETITIVE COMPLIANCE POSITIONING

### kwca vs. Healthcare Data Providers

| Provider Type | Data Source | Compliance Complexity | kwca Advantage |
|---------------|-------------|----------------------|----------------|
| **Prescriber Data** (IQVIA, Symphony) | Pharmacy claims, prescribing | High (requires careful handling) | Lower risk, no PHI |
| **EHR Data** (Komodo, HealthVerity) | Electronic health records | Very High (HIPAA concerns) | No clinical data |
| **Claims Data** (various) | Insurance claims | High (regulatory scrutiny) | No claims involvement |
| **Survey Data** (Kantar, etc.) | Consumer surveys | Medium | More scalable |
| **kwca Intent Data** | Search behavior | Low | Simple, clean, compliant |

### Key Differentiators for Sales

```
"Unlike healthcare data providers who handle sensitive clinical 
information, kwca uses only anonymous search intent signals.

This means:
✅ No HIPAA compliance burden
✅ No BAA required
✅ No patient consent issues
✅ No regulatory reporting requirements
✅ Faster implementation (no legal review delays)
✅ Lower risk profile for your organization

You get the precision of intent-based targeting without the 
compliance complexity of clinical data."
```

---

## LEGAL REVIEW CHECKLIST

### Documents to Have Ready

For client legal teams:

1. **Data Dictionary**
   - Complete list of data elements
   - Clear statement of what is NOT included
   - Source documentation

2. **Technical Architecture**
   - Data flow diagrams
   - Security measures
   - De-identification processes

3. **Standard Contract Terms**
   - Data Processing Addendum (DPA)
   - Service Provider Agreement
   - Data Security Addendum
   - Indemnification clauses

4. **Compliance FAQ**
   - Pre-written answers to common questions
   - Regulatory citations
   - Industry precedent

5. **Reference Clients**
   - Other healthcare clients who have approved
   - Case studies with compliance notes
   - Willingness to speak with legal peers

---

## WHEN TO INVOLVE LEGAL COUNSEL

**Green Light** (kwca standard use):
- Audience targeting for awareness campaigns
- HCP professional marketing
- General condition-related messaging
- Educational content distribution

**Yellow Light** (consult counsel):
- DTC drug advertising (FDA review needed)
- Clinical trial recruitment
- Rare disease targeting (sensitivity)
- Combination with first-party patient data

**Red Light** (don't proceed):
- Client wants to combine with PHI
- Attempting to re-identify audience members
- Using for clinical decision-making
- Targeting based on specific medical history

---

## QUICK REFERENCE: COMPLIANCE BY USE CASE

| Use Case | HIPAA | FDA | CCPA | kwca Ready? |
|----------|-------|-----|------|-------------|
| HCP Awareness | ✅ Exempt | N/A | ✅ Exempt | ✅ Yes |
| Patient Education | ✅ Not PHI | ⚠️ Content only | ✅ Exempt | ✅ Yes |
| DTC Advertising | ✅ Not PHI | ⚠️ Review content | ✅ Exempt | ✅ Yes* |
| Clinical Trial Recruiting | ✅ Not PHI | ⚠️ FDA rules | ✅ Exempt | ✅ Yes* |
| Condition Awareness | ✅ Not PHI | N/A | ✅ Exempt | ✅ Yes |
| Competitor Conquesting | ✅ Not PHI | N/A | ✅ Exempt | ✅ Yes |

*Requires client legal review of ad content

---

*Generated: 2026-03-10*  
*Purpose: Sales enablement for healthcare compliance objections*  
*Disclaimer: Not legal advice—consult qualified healthcare counsel*
