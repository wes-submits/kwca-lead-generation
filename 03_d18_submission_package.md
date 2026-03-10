# d18 Custom Audience Submission Package
## Keyword Custom Audiences — Healthcare & Pharmaceutical Marketing

---

## d18 Premade Audience Recommendations

Based on d18 taxonomy analysis, these premade audiences align with kwca's target market:

| d18 ID | Audience Name | Category | Est. Intent | Use Case |
|--------|---------------|----------|-------------|----------|
| 4eyes_500560 | Physician Segmentation & Targeting | Business Services/Marketing | ⭐⭐⭐⭐⭐ | **PRIMARY**: Healthcare marketers seeking physician targeting solutions |
| 4eyes_500557 | Pharma Commercial Analytics | Business Services/Marketing | ⭐⭐⭐⭐⭐ | **PRIMARY**: Pharma companies seeking commercial analytics/data |
| 4eyes_500558 | Pharma Sales Performance Metrics | Business Services/Marketing | ⭐⭐⭐⭐⭐ | **PRIMARY**: Pharma sales & marketing leadership |
| 4eyes_500566 | Market Access & Patient Journey Mapping | Business Services/Marketing | ⭐⭐⭐⭐ | Patient journey targeting interest |
| 4eyes_500564 | Physician Engagement Insights | Business Services/Marketing | ⭐⭐⭐⭐ | Healthcare orgs improving physician outreach |
| 4eyes_500565 | KOL Influence & Network Analytics | Business Services/Marketing | ⭐⭐⭐⭐ | Pharma KOL/analytics interest |
| 4eyes_501235 | Clinical Trial Management & CRO Services | Professional Services | ⭐⭐⭐ | Clinical research outsourcing (FSPs, MSPs, CROs) |
| 4eyes_500254 | Strategic IT Decision-Makers in Healthcare Systems | Business | ⭐⭐⭐ | Hospital/health system IT leaders |

### Premade Audience Pilot Selection (2 audiences)

**Priority 1: Physician Segmentation & Targeting (4eyes_500560)**
- **Why**: Direct match for HCP targeting use case
- **Target**: Healthcare marketers, pharma marketing directors
- **Keywords**: physician segmentation, physician targeting, healthcare marketing, pharmaceutical companies, provider segments
- **Expected overlap**: High with custom audiences 1 & 2

**Priority 2: Pharma Commercial Analytics (4eyes_500557)**
- **Why**: Targets pharma decision-makers actively seeking analytics/data solutions  
- **Target**: Commercial analytics teams, marketing leadership at pharma
- **Keywords**: pharma commercial analytics, pharmaceutical analytics, data analytics, commercial effectiveness, market access
- **Expected overlap**: High with custom audience 1

---

## Custom Audience Submissions (2 audiences)

### Custom Audience #1: Pharma Marketing High Intent

```yaml
custom_audience:
  internal_name: "kwca_pharma_high_intent_202603"
  display_name: "Pharma Marketing High Intent"
  description: >
    Marketing decision-makers at pharmaceutical, biotechnology, and life sciences 
    companies actively researching audience data solutions, HCP targeting platforms, 
    and intent data for healthcare marketing. These individuals are seeking data 
    providers to improve pharmaceutical marketing ROI, reach healthcare providers 
    more effectively, and access privacy-compliant audience targeting solutions 
    for DTC and HCP campaigns.
    
  criteria:
    primary_keywords:
      - "pharma marketing data"
      - "pharmaceutical audience"
      - "drug marketing audience"
      - "pharma DTC"
      - "buy pharma audience"
      - "pharma media buying"
      - "prescription drug marketing"
      - "pharmaceutical consumer data"
      - "pharma marketing platform"
      - "pharma audience targeting"
      
    secondary_keywords:
      - "pharma marketing database"
      - "drug marketing data"
      - "pharmaceutical marketing data providers"
      - "pharma audience segments"
      - "DTC pharmaceutical marketing"
      - "pharma marketing analytics"
      - "pharmaceutical media planning"
      - "drug advertising audience"
      - "pharma marketing solutions"
      - "pharmaceutical data vendor"
      
    contextual_signals:
      url_patterns:
        - "*pharma*"
        - "*pharmaceutical*"
        - "*drug-marketing*"
        - "*dtc*"
        - "*audience-data*"
        - "*intent-data*"
        
      page_title_signals:
        - "pharma marketing"
        - "pharmaceutical audience"
        - "drug marketing"
        - "pharmaceutical data"
        - "healthcare marketing"
        - "HCP targeting"
        
      content_keywords:
        - "pharmaceutical"
        - "drug marketing"
        - "audience data"
        - "intent signals"
        - "HCP"
        - "healthcare providers"
        - "DTC"
        - "compliance"
        
  filters:
    geography: ["United States"]
    
  expected_size: "85k-140k"
  refresh_frequency: "daily"
  data_retention: "90_days"
  priority: 1
```

### Custom Audience #2: HCP Targeting Solutions

```yaml
custom_audience:
  internal_name: "kwca_hcp_targeting_202603"
  display_name: "HCP Targeting Solutions Seekers"
  description: >
    Healthcare marketers and pharmaceutical companies actively searching for 
    Healthcare Provider (HCP) targeting data and physician audience solutions. 
    Includes professionals seeking to reach physicians, specialists, nurse 
    practitioners, and other healthcare providers with targeted marketing campaigns. 
    These users are looking for prescriber data, physician email lists, and 
    clinical audience targeting platforms to improve their healthcare marketing ROI.
    
  criteria:
    primary_keywords:
      - "HCP targeting"
      - "physician audience"
      - "healthcare provider data"
      - "prescriber audience"
      - "medical professional targeting"
      - "specialist physician lists"
      - "nurse practitioner data"
      - "clinical audience"
      - "doctor targeting"
      - "physician email lists"
      
    secondary_keywords:
      - "HCP data providers"
      - "physician marketing database"
      - "healthcare professional lists"
      - "medical audience targeting"
      - "prescriber marketing"
      - "physician segmentation"
      - "healthcare provider outreach"
      - "clinical decision makers"
      - "medical specialty targeting"
      - "healthcare audience data"
      
    contextual_signals:
      url_patterns:
        - "*hcp*"
        - "*physician*"
        - "*prescriber*"
        - "*healthcare-provider*"
        - "*doctor-data*"
        - "*clinical*"
        
      page_title_signals:
        - "HCP targeting"
        - "physician audience"
        - "healthcare provider data"
        - "prescriber marketing"
        - "medical professional"
        - "clinical audience"
        
      content_keywords:
        - "HCP"
        - "physician"
        - "healthcare provider"
        - "prescriber"
        - "clinical"
        - "medical professional"
        - "audience data"
        - "targeting"
        
  filters:
    geography: ["United States"]
    
  expected_size: "65k-110k"
  refresh_frequency: "daily"
  data_retention: "90_days"
  priority: 2
```

---

## 4-Audience Pilot Stack Summary

| Priority | Audience Name | Source | Type | Est. Size | LinkedIn Overlay |
|----------|---------------|--------|------|-----------|------------------|
| 1 | Physician Segmentation & Targeting | d18 Premade | Premade | Check d18 | 50k-90k |
| 2 | Pharma Commercial Analytics | d18 Premade | Premade | Check d18 | 40k-75k |
| 3 | Pharma Marketing High Intent | d18 Custom | Custom | 85k-140k | 60k-100k |
| 4 | HCP Targeting Solutions Seekers | d18 Custom | Custom | 65k-110k | 45k-80k |

### Total Reach Estimates

| Metric | Estimate |
|--------|----------|
| **Raw d18 audience** | 190k-340k |
| **After LinkedIn overlay** | 140k-240k (job titles + industries) |
| **Expected unique reach** | 120k-200k (accounting for overlap) |
| **Expected CTR** | 0.8-1.2% (B2B healthcare) |
| **Expected CPC** | $12-$22 |
| **Expected CPL** | $95-$165 |

---

## d18 Dashboard Submission Format

### CSV for Bulk Upload

```csv
audience_name,description,primary_keywords,secondary_keywords,url_patterns,title_signals,expected_size,refresh_frequency
"Pharma Marketing High Intent","Marketing decision-makers at pharmaceutical companies actively researching audience data solutions, HCP targeting platforms, and intent data for healthcare marketing...","pharma marketing data;pharmaceutical audience;drug marketing audience;pharma DTC;buy pharma audience","pharma marketing database;drug marketing data;pharmaceutical marketing data providers;pharma audience segments;dtc pharmaceutical marketing","*pharma*;*pharmaceutical*;*drug-marketing*;*dtc*","pharma marketing;pharmaceutical audience;drug marketing;healthcare marketing","85k-140k","daily"
"HCP Targeting Solutions Seekers","Healthcare marketers seeking Healthcare Provider targeting data and physician audience solutions for reaching physicians, specialists, and nurse practitioners...","HCP targeting;physician audience;healthcare provider data;prescriber audience;medical professional targeting","HCP data providers;physician marketing database;healthcare professional lists;medical audience targeting;prescriber marketing","*hcp*;*physician*;*prescriber*;*healthcare-provider*","HCP targeting;physician audience;healthcare provider data;prescriber marketing;medical professional","65k-110k","daily"
```

---

## Internal Tracking Sheet

| Internal ID | Display Name | Type | Status | Est. Size | Daily Records | S3 Path | Actions |
|-------------|--------------|------|--------|-----------|---------------|---------|---------|
| kwca_pharma_high_intent_202603 | Pharma Marketing High Intent | Custom | Pending Submission | 85k-140k | TBD | s3://kwca-audiences/pharma/ | [Submit to d18] |
| kwca_hcp_targeting_202603 | HCP Targeting Solutions Seekers | Custom | Pending Submission | 65k-110k | TBD | s3://kwca-audiences/pharma/ | [Submit to d18] |
| 4eyes_500560 | Physician Segmentation & Targeting | Premade | Available | TBD | TBD | s3://kwca-audiences/pharma/ | [Order from d18] |
| 4eyes_500557 | Pharma Commercial Analytics | Premade | Available | TBD | TBD | s3://kwca-audiences/pharma/ | [Order from d18] |

---

## 72-Hour Monitoring Checklist

After submission:

- [ ] **Hour 0**: Submit both custom audiences to d18 dashboard
- [ ] **Hour 24**: Check for initial size estimates
- [ ] **Hour 48**: Validate audience sizes (should be 50k-400k range)
- [ ] **Hour 72**: If sizes too large, add more specific keywords; if too small, broaden
- [ ] **Hour 72**: Order premade audiences 4eyes_500560, 4eyes_500557
- [ ] **Day 7**: Export all audiences to S3, deliver to client bucket

### Size Adjustment Triggers

| Condition | Action |
|-----------|--------|
| Size > 400k | Add more specific keywords (e.g., add "buy" + brand terms) |
| Size < 50k | Broaden keywords (e.g., add "healthcare marketing", "pharmaceutical advertising") |
| Overlap > 60% between audiences | Differentiate keyword sets more distinctly |

