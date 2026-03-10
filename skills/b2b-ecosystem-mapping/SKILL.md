# Skill: B2B Ecosystem Mapping
# Generate strategic ecosystem maps for B2B marketing activation

## Purpose
Transform a client's (or competitor's) website into a comprehensive B2B marketing ecosystem map. This skill analyzes positioning, identifies ecosystem layers, maps competitors/partners, and creates LinkedIn-ready outreach strategies based on ecosystem positioning.

## Inputs

```yaml
client:
  company_name: "Keyword Custom Audiences"           # Required: Your company/brand
  company_url: "https://keywordcustomaudience.com"   # Required: Your website
  target_url: "https://example-competitor.com"       # Required: Client or competitor to analyze
  
context:
  industry: "healthcare"                             # Required: Industry vertical
  target_segment: "enterprise"                       # Options: smb, midmarket, enterprise
  ecosystem_focus: "marketing_technology"            # Ecosystem type (see below)
  
options:
  include_competitors: true                          # Map competitive landscape
  include_partners: true                             # Map partnership opportunities
  include_outreach_scripts: true                     # Generate LinkedIn scripts
  output_format: ["markdown", "mermaid"]             # Mermaid diagram support (future)
```

### Ecosystem Focus Types

| Type | Description | Example Players |
|------|-------------|-----------------|
| `marketing_technology` | MarTech stack, data, activation | DSPs, CDPs, intent data, agencies |
| `sales_infrastructure` | Sales tools, enablement, CRM | CRMs, sales engagement, analytics |
| `data_infrastructure` | Data platforms, identity, compliance | Data warehouses, identity resolution |
| `financial_services` | Fintech, banking, insurance | Payment processors, lending, regtech |
| `healthcare_tech` | Healthcare IT, pharma, life sciences | EHRs, data providers, clinical platforms |
| `custom` | Define your own layers | Any B2B vertical |

## Process

### Phase 1: Positioning Analysis (Input URL)

Analyze the target URL to extract:
- **Value proposition**: What they claim to solve
- **Target audience**: Who they sell to (job titles, company types)
- **Key differentiators**: Unique claims vs competitors
- **Pricing signals**: Premium, mid-market, or budget positioning
- **Integration mentions**: Who they connect with (partners, platforms)

**Output**: Positioning Brief (Markdown)

```markdown
# Positioning Analysis: [Target Company]

## Value Proposition
[Extracted from homepage/hero]

## Target Audience
- Primary: [Job titles, company types]
- Secondary: [Additional segments]

## Competitive Claims
- "Better than X because..."
- "Only solution that..."

## Ecosystem Position
- Layer: [Where they sit in stack]
- Connections: [Integrations mentioned]
```

### Phase 2: Ecosystem Layer Mapping

Build 5-7 layer ecosystem map based on vertical:

```
Layer 1: END CUSTOMERS (The Buyers)
├── Who pays: [Company types, segments]
├── Job titles: [Decision makers]
└── Pain points: [What drives purchase]

Layer 2: ORCHESTRATORS (Agencies, Consultants)
├── Who manages: [Agencies, SIs, consultants]
├── Their role: [Strategy, implementation, management]
└── Their incentive: [Fees, margins, differentiation]

Layer 3: INFRASTRUCTURE (Data, Identity, Plumbing)
├── Identity resolution: [LiveRamp, Neustar, etc.]
├── Data providers: [Vertical-specific data sources]
├── Compliance: [Security, privacy, regulatory]
└── Connectivity: [APIs, integrations, protocols]

Layer 4: [CLIENT] POSITION ← YOUR PRODUCT HERE
├── Incumbents: [Current players in this space]
├── Your position: [How you fit]
├── Inputs: [What feeds into your product]
└── Outputs: [What your product feeds]

Layer 5: ACTIVATION (Where Value Is Deployed)
├── Platforms: [DSPs, social, direct channels]
├── Tactics: [Email, ads, direct mail, events]
└── Reach: [How customers are reached]

Layer 6: MEASUREMENT (ROI, Attribution)
├── Analytics: [Tools that measure success]
├── Attribution: [How credit is assigned]
└── Optimization: [Feedback loops]
```

### Phase 3: Competitive Landscape Mapping

For each layer, identify:
- **Incumbents**: Established players
- **Challengers**: New entrants, disruptors
- **Your differentiation**: Why you're different/better

| Company | Offering | Your Differentiation |
|---------|----------|---------------------|
| [Competitor A] | [What they do] | [Why you're better] |
| [Competitor B] | [What they do] | [Why you're better] |

### Phase 4: Integration Workflows

Map how your product integrates with each ecosystem layer:

**Workflow 1: Client → You → Activation**
```
[End Customer] → [Your Product] → [Activation Platform]
     ↓                                        ↓
   Brief                                   Campaign
```

**Workflow 2: Agency Partnership**
```
[Agency] → [Your Product] → [Client Value]
   ↓              ↓
Strategy    Differentiation
```

**Workflow 3: Platform Integration**
```
[Platform] → [Your Product] → [Enriched Output]
    ↓                               ↓
 Data In                      Enhanced Data Out
```

### Phase 5: LinkedIn Outreach Strategy

Generate outreach scripts for each ecosystem role:

**Script Template**:
```
Hi {{first_name}},

Quick question about your {{ecosystem_role}}:

Most {{job_title}}s I talk to are working with [Incumbent A] for 
[capability] and [Incumbent B] for [capability]—but they're still 
struggling with [pain point your product solves].

[Your Company] fills that gap:
→ [Benefit 1]
→ [Benefit 2]
→ [Benefit 3]

We're working with [reference companies] to add this [capability] 
to their [ecosystem layer].

Worth a 15-minute conversation?

[Yes, let's talk] [Send me info] [Not now]
```

## Outputs

### Output A: Ecosystem Map (Markdown)

Complete 6-layer ecosystem visualization with ASCII diagram showing:
- All layers with descriptions
- Your product's position (highlighted)
- Data flows between layers
- Key players at each layer

### Output B: Positioning Brief (Markdown)

Analysis of the input URL:
- Value proposition extraction
- Target audience identification
- Competitive positioning
- Integration landscape

### Output C: Competitive Matrix (Markdown Table)

| Company | Layer | Offering | Differentiation |
|---------|-------|----------|-----------------|
| ... | ... | ... | ... |

### Output D: Integration Workflows (Markdown)

3+ workflow diagrams showing how your product fits:
- Direct client workflow
- Agency partnership workflow
- Platform integration workflow

### Output E: LinkedIn Outreach Scripts (Markdown)

Customized scripts for:
- **Tier 1 Targets**: Enterprise buyers
- **Tier 2 Targets**: Agencies/consultants
- **Tier 3 Targets**: Platform partners
- **Tier 4 Targets**: Growth/SMB segment

Each script includes:
- Opening hook referencing ecosystem
- Pain point articulation
- Value proposition
- Soft CTA with button options

### Output F: Target Account List (CSV)

| Company | Tier | Ecosystem Role | Priority | LinkedIn Strategy |
|---------|------|----------------|----------|-------------------|
| ... | 1 | End Customer | High | Conversation Ad |
| ... | 2 | Agency | High | Sponsored Content |
| ... | 3 | Platform | Medium | Partner outreach |

## Usage Examples

### Example 1: Healthcare Marketing (Pharma)

```yaml
client:
  company_name: "Keyword Custom Audiences"
  company_url: "https://keywordcustomaudience.com"
  target_url: "https://www.iqvia.com"  # Analyze competitor
  
context:
  industry: "healthcare"
  target_segment: "enterprise"
  ecosystem_focus: "marketing_technology"
  
options:
  include_competitors: true
  include_partners: true
  include_outreach_scripts: true
```

**Output**: Full pharma marketing ecosystem map (as demonstrated in workflow)

### Example 2: Fintech Infrastructure

```yaml
client:
  company_name: "DataVault"
  company_url: "https://datavault.io"
  target_url: "https://plaid.com"  # Analyze adjacent player
  
context:
  industry: "financial_services"
  target_segment: "midmarket"
  ecosystem_focus: "data_infrastructure"
```

**Output**: Fintech data infrastructure ecosystem with Plaid as reference

### Example 3: Sales Enablement

```yaml
client:
  company_name: "PitchAI"
  company_url: "https://pitchai.com"
  target_url: "https:// Gong.io"  # Analyze leader
  
context:
  industry: "technology"
  target_segment: "enterprise"
  ecosystem_focus: "sales_infrastructure"
```

**Output**: Sales tech ecosystem map with Gong as competitive reference

## Workflow Steps

When executing this skill:

1. **Read target URL**: Extract positioning, claims, integrations
2. **Research ecosystem**: Identify players at each layer for the vertical
3. **Map layers**: Build 6-layer ecosystem visualization
4. **Position client**: Insert client's product in correct layer
5. **Map competition**: Identify incumbents and differentiators
6. **Build workflows**: Show integration points with each layer
7. **Create scripts**: Generate LinkedIn outreach for each tier
8. **Compile targets**: Build account list with prioritization

## Integration Points

- **Input from**: Company website, competitor analysis
- **Output to**: LinkedIn campaign strategy, sales playbook, partner materials
- **Feeds into**: LinkedIn Conversation Ads, ABM campaigns, sales outreach

## File Naming Convention

```
[client]_[industry]_ecosystem_map.md
[client]_[industry]_positioning_brief.md
[client]_[industry]_competitive_matrix.md
[client]_[industry]_workflows.md
[client]_[industry]_linkedin_scripts.md
[client]_[industry]_target_accounts.csv
```

## Notes

- Ecosystem maps are industry-specific — use vertical expertise
- Competitor analysis reveals white space opportunities
- LinkedIn scripts should reference specific ecosystem layers/players
- Target account tiers reflect deal size and sales cycle complexity
- Update quarterly as ecosystem evolves (new entrants, M&A, shifts)

## Future Enhancements

- [ ] Mermaid diagram generation for visual ecosystem maps
- [ ] Automatic competitor discovery via web crawling
- [ ] Integration with LinkedIn Sales Navigator for account enrichment
- [ ] CRM sync for target account list upload
- [ ] Ecosystem map versioning (track changes over time)
