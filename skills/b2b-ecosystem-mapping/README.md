# B2B Ecosystem Mapping Skill

Generate strategic ecosystem maps for B2B marketing activation. This skill transforms a client or competitor URL into a comprehensive 6-layer ecosystem visualization with LinkedIn-ready outreach strategies.

## What It Does

1. **Analyzes positioning** from target URL
2. **Maps 6 ecosystem layers**: End Customers → Orchestrators → Infrastructure → [Your Product] → Activation → Measurement
3. **Identifies competitors** and differentiation opportunities
4. **Creates integration workflows** showing how your product fits
5. **Generates LinkedIn scripts** tailored to each ecosystem role
6. **Builds target account list** with prioritization

## Quick Start

```yaml
client:
  company_name: "Your Company"
  company_url: "https://yoursite.com"
  target_url: "https://competitor.com"  # Or client you're pitching
  
context:
  industry: "healthcare"  # healthcare, fintech, sales_tech, etc.
  target_segment: "enterprise"
  ecosystem_focus: "marketing_technology"
  
options:
  include_competitors: true
  include_partners: true
  include_outreach_scripts: true
```

## Example Output

See [`examples/pharma_marketing_ecosystem_map.md`](examples/pharma_marketing_ecosystem_map.md) for a complete healthcare/pharma marketing ecosystem map demonstrating:
- 6-layer ecosystem visualization
- kwca's position as intent data layer
- Competitive landscape vs IQVIA, Veeva, Bombora
- LinkedIn outreach scripts for agencies, pharma brands, MarTech

## Use Cases

| Scenario | Input | Output |
|----------|-------|--------|
| **Competitive positioning** | Competitor URL | Ecosystem map showing where you fit vs them |
| **New market entry** | Industry leader URL | Full ecosystem with your insertion point |
| **Partner development** | Platform company URL | Integration workflow + partner pitch |
| **Sales enablement** | Prospect URL | Custom outreach referencing their stack |

## Supported Verticals

- Healthcare / Pharma
- Financial Services / Fintech
- Sales Technology
- Marketing Technology
- Data Infrastructure
- Custom (define your own)

## Files Generated

- `*_ecosystem_map.md` — 6-layer visualization
- `*_positioning_brief.md` — URL analysis
- `*_competitive_matrix.md` — Competitor comparison
- `*_workflows.md` — Integration diagrams
- `*_linkedin_scripts.md` — Outreach templates
- `*_target_accounts.csv` — Prioritized account list

## See Also

- Full skill documentation: [`SKILL.md`](SKILL.md)
- Example output: [`examples/`](examples/)
