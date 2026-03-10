# Pharmaceutical Marketing Ecosystem Map
## How Keyword Custom Audiences Fits Into Enterprise Pharma Marketing

---

## Executive Summary

This map visualizes the current pharmaceutical marketing technology stack, showing where **Keyword Custom Audiences (kwca)** fits as a **new intent data layer** that bridges the gap between raw healthcare data and actionable marketing audiences.

**kwca's Position**: Intent signal provider → Audience builder → Delivery layer  
**Target Users**: Pharma brands, healthcare agencies, MarTech platforms  
**Value Proposition**: Keyword-level intent data delivered as ready-to-use audiences

---

## Ecosystem Layers

```
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 1: PHARMACEUTICAL BRANDS (The Buyers)                                │
├─────────────────────────────────────────────────────────────────────────────┤
│  • Global Pharma (Pfizer, Novartis, J&J, Roche, Merck)                     │
│  • Specialty Pharma (Biogen, Gilead, Regeneron)                            │
│  • Biotech (Moderna, BioNTech, Vertex)                                      │
│  • Generic Manufacturers (Teva, Mylan, Sandoz)                              │
│                                                                             │
│  Marketing Teams: Brand Managers, Digital Marketing Directors,             │
│  Media Directors, Data Strategy Leads, Market Access Teams                 │
└─────────────────────────────────────────────────────────────────────────────┘
                                      ↓
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 2: HEALTHCARE MARKETING AGENCIES (The Orchestrators)                │
├─────────────────────────────────────────────────────────────────────────────┤
│  • Full-Service Healthcare Agencies:                                       │
│    - CDM (Groupe CDM)                                                      │
│    - Ogilvy Health                                                         │
│    - Harrison & Star                                                       │
│    - Havas Health & You                                                    │
│    - Wunderman Thompson Health                                             │
│    - Klick Health                                                          │
│    - Intouch Group                                                         │
│                                                                             │
│  • Media Agencies with Healthcare Practice:                                │
│    - Mindshare Health                                                      │
│    - Publicis Health Media                                                 │
│    - Omnicom Health Group                                                  │
│    - IPG Health                                                            │
│                                                                             │
│  Role: Strategy, creative, media planning/buying, data orchestration       │
└─────────────────────────────────────────────────────────────────────────────┘
                                      ↓
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 3: DATA & IDENTITY LAYER (The Plumbing)                            │
├─────────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐         │
│  │ IDENTITY RESOLUTION                                     │         │
│  ├──────────────────┤  ├──────────────────┤  ├──────────────────┤         │
│  │ • LiveRamp       │  │ • Throtle        │  │ • InfoSum        │         │
│  │ • Neustar        │  │ • Tapad          │  │ • Epsilon        │         │
│  │ • Experian       │  │ • Crosswise      │  │ • Acxiom         │         │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘         │
│                                                                             │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐         │
│  │ HEALTHCARE DATA SPECIALISTS                             │         │
│  ├──────────────────┤  ├──────────────────┤  ├──────────────────┤         │
│  │ • IQVIA          │  │ • Komodo Health  │  │ • Definitive HC  │         │
│  │ • Veeva Systems  │  │ • Datavant       │  │ • HealthLink     │
│  │ • Symphony Health│  │ • PurpleLab      │  │ • DMD Healthcare │         │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘         │
│                                                                             │
│  Function: Link identities, resolve NPIs, segment HCPs/patients            │
└─────────────────────────────────────────────────────────────────────────────┘
                                      ↓
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 4: INTENT DATA LAYER ← KEYWORD CUSTOM AUDIENCES ENTERS HERE         │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │  INCUMBENT INTENT PROVIDERS                                         │   │
│  ├─────────────────────────────────────────────────────────────────────┤   │
│  │  • Bombora          (B2B topic intent)                              │   │
│  │  • Demandbase       (Account-based intent)                          │   │
│  │  • 6sense           (Account engagement)                            │   │
│  │  • G2 Intent        (Software category intent)                      │   │
│  │                                                                     │   │
│  │  Limitations:                                                       │   │
│  │  • Topic-level only (not keyword-level)                             │   │
│  │  • Limited healthcare taxonomy                                      │   │
│  │  • Not built for pharma compliance                                  │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │  ★ KEYWORD CUSTOM AUDIENCES (kwca) ★                               │   │
│  ├─────────────────────────────────────────────────────────────────────┤   │
│  │                                                                     │   │
│  │  Position: Keyword-level intent data → Healthcare audiences         │   │
│  │                                                                     │   │
│  │  Inputs:                                                            │   │
│  │  ┌──────────┐  ┌──────────┐  ┌──────────┐                          │   │
│  │  │ d18      │  │ d3       │  │ Custom   │  (Raw intent signals)   │   │
│  │  │ 23K+     │  │ 20K+     │  │ Keywords │                          │   │
│  │  │ topics   │  │ topics   │  │          │                          │   │
│  │  └────┬─────┘  └────┬─────┘  └────┬─────┘                          │   │
│  │       └──────────────┼──────────────┘                                │   │
│  │                      ↓                                               │   │
│  │              ┌───────────────┐                                       │   │
│  │              │  kwca Engine  │  • Keyword extraction                 │   │
│  │              │               │  • Intent scoring                     │   │
│  │              │  • Canonical  │  • Privacy compliance                 │   │
│  │              │    schema     │  • Audience segmentation              │   │
│  │              └───────┬───────┘                                       │   │
│  │                      ↓                                               │   │
│  │  Outputs:         ┌──────────────┐                                   │   │
│  │                   │  S3 Delivery │  → Client buckets                 │   │
│  │                   │  (Daily)     │  → Facebook/LinkedIn upload       │   │
│  │                   │              │  → Programmatic activation        │   │
│  │                   └──────────────┘                                   │   │
│  │                                                                     │   │
│  │  Differentiation:                                                   │   │
│  │  ✓ Keyword-level granularity (not just topic)                       │   │
│  │  ✓ 23,000+ healthcare premade audiences                             │   │
│  │  ✓ HIPAA-aware delivery (S3, not PII)                               │   │
│  │  ✓ 24-48 hour turnaround                                            │   │
│  │  ✓ Custom audience creation from keyword criteria                   │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
                                      ↓
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 5: ACTIVATION PLATFORMS (Where Audiences Are Deployed)              │
├─────────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐         │
│  │ PROGRAMMATIC DSPs                                       │         │
│  ├──────────────────┤  ├──────────────────┤  ├──────────────────┤         │
│  │ • The Trade Desk │  │ • DV360          │  │ • Xandr          │         │
│  │ • MediaMath      │  │ • Amazon DSP     │  │ • Yahoo DSP      │         │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘         │
│                                                                             │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐         │
│  │ SOCIAL PLATFORMS                                        │         │
│  ├──────────────────┤  ├──────────────────┤  ├──────────────────┤         │
│  │ • LinkedIn       │  │ • Meta (FB/IG)   │  │ • Twitter/X      │         │
│  │ • TikTok         │  │ • Reddit         │  │ • Pinterest      │         │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘         │
│                                                                             │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐         │
│  │ DIRECT CHANNELS                                         │         │
│  ├──────────────────┤  ├──────────────────┤  ├──────────────────┤         │
│  │ • Email (ESP)    │  │ • Direct Mail    │  │ • CTV/Streaming  │         │
│  │ • SMS/Mobile     │  │ • Audio/Podcast  │  │ • DOOH           │         │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘         │
│                                                                             │
│  Note: Platform restrictions limit HCP targeting → kwca provides          │
│  off-platform reach (email, programmatic, direct mail)                     │
└─────────────────────────────────────────────────────────────────────────────┘
                                      ↓
┌─────────────────────────────────────────────────────────────────────────────┐
│  LAYER 6: MEASUREMENT & ATTRIBUTION                                        │
├─────────────────────────────────────────────────────────────────────────────┤
│  • IQVIA (sales data, ROI measurement)                                     │
│  • Crossix (healthcare marketing analytics)                                │
│  • ClosedLoop (healthcare-specific attribution)                            │
│  • Google Analytics / Adobe Analytics                                      │
│  • Internal CRM (Salesforce, Veeva CRM)                                    │
│                                                                             │
│  Function: Connect audience exposure to prescription lift, brand awareness │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## kwca Integration Points

### 1. kwca → Healthcare Agencies
**Use Case**: Agencies use kwca to differentiate their data offering to pharma clients

```
Agency Workflow:
┌──────────────┐    ┌──────────────┐    ┌──────────────┐
│   Strategy   │ →  │ kwca Intent  │ →  │ Audience     │
│   (Client    │    │   Data       │    │   Build      │
│   Brief)     │    │              │    │              │
└──────────────┘    └──────────────┘    └──────┬───────┘
                                               ↓
                                        ┌──────────────┐
                                        │  Activation  │
                                        │  (DSP/Social)│
                                        └──────────────┘
```

**Agency Value Props**:
- "Intent-based audiences vs. demographic-only"
- "Faster turnaround than traditional data brokers"
- "Keyword-level granularity for precise targeting"

---

### 2. kwca → Pharma Brands (Direct)
**Use Case**: Pharma brands bypass agencies and build audiences in-house

```
Pharma Brand Workflow:
┌──────────────┐    ┌──────────────┐    ┌──────────────┐
│  Brand Team  │ →  │   kwca API   │ →  │  Audience    │
│  (Marketing  │    │   /Portal    │    │  Segments    │
│   Director)  │    │              │    │              │
└──────────────┘    └──────────────┘    └──────┬───────┘
                                               ↓
                                        ┌──────────────┐
                                        │  Internal    │
                                        │  Activation  │
                                        │  (DSP/CDP)   │
                                        └──────────────┘
```

**Pharma Brand Value Props**:
- "Privacy-compliant HCP targeting outside platform walls"
- "Condition-specific patient journey audiences"
- "Integration with existing CDP/DMP"

---

### 3. kwca → MarTech Platforms
**Use Case**: Data platforms embed kwca as an intent data layer

```
MarTech Integration:
┌──────────────┐    ┌──────────────┐    ┌──────────────┐
│   Customer   │ →  │   kwca       │ →  │  Enriched    │
│   Platform   │    │   Intent     │    │  Profiles    │
│   (CDP/DMP)  │    │   Feed       │    │              │
└──────────────┘    └──────────────┘    └──────┬───────┘
                                               ↓
                                        ┌──────────────┐
                                        │  Activation  │
                                        │  (All Channels)│
                                        └──────────────┘
```

**MarTech Value Props**:
- "Intent signal enrichment for identity graph"
- "API-accessible healthcare audiences"
- "Differentiated data partnership"

---

## Current Pain Points (kwca Solves)

| Pain Point | Current State | kwca Solution |
|------------|---------------|---------------|
| **Platform Restrictions** | LinkedIn/Meta heavily limit HCP targeting | Off-platform audiences (email, programmatic, direct mail) |
| **Data Quality** | Demographic targeting (job title ≠ intent) | Intent-based (what they're searching for right now) |
| **Vendor Management** | Managing 5-10 data vendors | Single intent layer, multiple delivery options |
| **Speed to Market** | 2-4 weeks for custom audiences | 24-48 hour turnaround |
| **Compliance Complexity** | Most vendors lack healthcare expertise | HIPAA-aware delivery, S3-only (no PII exposure) |
| **Audience Overlap** | Everyone buying from same 3 providers | Custom keyword criteria = unique audiences |

---

## Competitive Landscape

### Incumbent Data Providers
| Company | Offering | kwca Differentiation |
|---------|----------|---------------------|
| **IQVIA** | HCP data, prescribing data, claims | kwca adds intent layer on top |
| **Veeva** | CRM, closed-loop marketing | kwca provides off-CRM activation |
| **Komodo Health** | Healthcare map, analytics | kwca is intent signal, not just identity |
| **Bombora** | B2B intent data | kwca is keyword-level + healthcare-specific |
| **LiveRamp** | Identity resolution, data onboarding | kwca is upstream data provider |
| **Crossix** | Healthcare marketing measurement | kwca feeds into Crossix for attribution |

### Agency Partners (Potential)
| Agency | Why kwca Fits |
|--------|---------------|
| **CDM** | Differentiator for pitch decks |
| **Ogilvy Health** | Intent data for DTC campaigns |
| **Klick Health** | Digital-first, data-hungry |
| **Intouch Group** | Tech-enabled, integration-friendly |

---

## Target Accounts by Segment

### Tier 1: Enterprise Pharma (Direct)
- Pfizer, Novartis, J&J, Roche, Merck
- Target: VP Digital Marketing, Data Strategy Leads
- Use Case: In-house audience building for DTC campaigns

### Tier 2: Top Healthcare Agencies (Partners)
- CDM, Ogilvy Health, Harrison & Star, Klick Health
- Target: Data Strategy Directors, Media Directors
- Use Case: Client offering differentiation

### Tier 3: MarTech Platforms (Integrations)
- LiveRamp, InfoSum, HealthLink Dimensions
- Target: Partnership Managers, Product Teams
- Use Case: Intent data API integration

### Tier 4: Specialty Pharma / Biotech (Growth)
- Biogen, Gilead, Regeneron, Vertex, Moderna
- Target: Digital Marketing Managers
- Use Case: Competing with big pharma data budgets

---

## LinkedIn Outreach Strategy

Using this ecosystem map, kwca's LinkedIn outreach should:

1. **Reference the ecosystem** — "I work with healthcare agencies like CDM to add intent data to their pharma marketing stack"
2. **Name the pain** — "Are you hitting LinkedIn's HCP targeting restrictions?"
3. **Position the solution** — "We provide keyword-level intent audiences delivered to your S3 bucket"
4. **Offer value** — "I can send you a sample audience for [condition] targeting to evaluate"

### Outreach Script (Based on Ecosystem Map)

```
Hi {{first_name}},

Quick question about your pharma marketing stack:

Most {{job_title}}s I talk to are working with [IQVIA/Veeva] for HCP data 
and [LiveRamp] for identity—but they're still struggling to reach physicians 
outside platform walls.

Keyword Custom Audiences fills that gap:
→ Intent signals from 23,000+ healthcare topics
→ Keyword-level granularity (not just "physician")
→ Delivered to your S3 bucket (HIPAA-aware)

We're working with agencies like CDM and brands like [reference] to add 
this intent layer to their campaigns.

Worth a 15-minute conversation?

[Yes, let's talk] [Send me a sample] [Not now]
```

---

## Next Steps

1. **Validate ecosystem map** — Confirm players, relationships, pain points
2. **Identify priority targets** — Which Tier 1-4 accounts to pursue first
3. **Build case studies** — Map specific client wins to ecosystem layers
4. **Create partner materials** — Agency one-pager, MarTech integration guide
5. **Launch LinkedIn campaigns** — Targeted by job title, company, ecosystem role

---

*Generated: 2026-03-10*  
*Purpose: LinkedIn direct outreach strategy for kwca*  
*Format: Ecosystem map + integration workflows + competitive landscape*
