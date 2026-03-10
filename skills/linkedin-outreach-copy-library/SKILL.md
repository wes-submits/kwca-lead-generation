# Skill: LinkedIn Outreach Copy Library
# Generate channel-specific LinkedIn outreach copy for B2B sales

## Purpose
Create personalized, high-converting LinkedIn outreach copy for B2B sales teams. This skill generates conversation ads, connection requests, follow-up sequences, and objection handlers tailored to the prospect's channel focus, industry, and pain points.

## Inputs

```yaml
client:
  company_name: "Your Company"              # Required: Your brand name
  company_url: "https://yoursite.com"       # Required: Your website
  product_niche: "intent data"              # Required: Your product category
  
target:
  industry: "healthcare"                    # Required: Target industry
  sub_niche: "pharma"                       # Optional: Specific vertical
  target_titles: ["VP Marketing", "Media Director"]  # Required: Job titles
  primary_channel: "facebook"               # Options: facebook, programmatic, ctv, multi
  
case_study:
  client_name: "Example Brand"              # Required: Reference client
  result_metric: "40% lower CAC"            # Required: Key result
  specific_example: "Detailed example"      # Required: Concrete use case
  
options:
  include_compliance_note: true             # Add privacy/compliance disclaimer
  include_pilot_offer: true                 # Include 48-hour pilot CTA
  tone: "professional"                      # Options: professional, casual, aggressive
```

## Process

### Phase 1: Channel Positioning

Determine messaging angle based on primary channel:

**Facebook Positioning**:
- Hook: Post-iOS14 degradation
- Pain: Rising CPMs, poor lookalikes, audience fatigue
- Solution: Intent-based Custom Audiences
- Proof: CAC/ROAS improvements

**Programmatic Positioning**:
- Hook: Data quality uncertainty, cookie deprecation
- Pain: CTV targeting limits, cross-channel frequency
- Solution: Keyword-intent audiences across DSPs
- Proof: Completion rates, viewability

**CTV Positioning**:
- Hook: Premium inventory, weak targeting
- Pain: Demo targeting inefficiency, measurement gaps
- Solution: Intent-based CTV audiences
- Proof: Completion rate lift

### Phase 2: Industry Customization

**Healthcare/Pharma Specifics**:
- Emphasize compliance (HIPAA-safe, no PHI)
- Use specific drug/condition examples
- Reference DTC advertising opportunities
- Highlight HCP targeting capabilities
- Include anonymized data disclaimer

### Phase 3: Copy Generation

Generate 4 core components:
1. **Conversation Ads** (Message Ads) - 3 variations
2. **Connection Requests** - 3 templates
3. **Follow-Up Sequence** - 3-touch nurture
4. **Objection Handlers** - Common responses

### Phase 4: Case Study Integration

Weave specific example throughout copy:
- Opening hook reference
- Mid-message proof point
- Closing CTA reinforcement

## Outputs

### Output A: Conversation Ad Scripts (Markdown)

3 variations for Message Ads:
- Version 1: Direct problem/solution
- Version 2: Case study lead
- Version 3: Short/punchy (mobile)

### Output B: Connection Request Templates (Markdown)

3 approaches:
- Value-first
- Question hook
- Community/reference

### Output C: Follow-Up Sequence (Markdown)

3-touch sequence:
- Day 0: Connection acceptance
- Day 3: Value add
- Day 7: Soft close/breakup

### Output D: Objection Handlers (Markdown)

Responses to:
- "We're happy with current setup"
- "No budget"
- "Using competitor"
- "Send me info"

### Output E: Compliance-First Outreach (Optional)

Scripts that proactively address:
- Privacy concerns
- Data sourcing questions
- Regulatory compliance

## Usage Examples

### Example 1: Pharma Facebook

```yaml
client:
  company_name: "Keyword Custom Audiences"
  product_niche: "intent-based audience data"
  
target:
  industry: "healthcare"
  sub_niche: "pharma"
  primary_channel: "facebook"
  
case_study:
  client_name: "GLP-1 Brand"
  result_metric: "40% lower cost per result"
  specific_example: "Built audience of 'buy tirzepatide' searchers, showed ads to high-intent prospects"
```

### Example 2: Enterprise Programmatic

```yaml
client:
  company_name: "DataVault"
  product_niche: "audience data platform"
  
target:
  industry: "cpg"
  primary_channel: "programmatic"
  
case_study:
  client_name: "Fortune 500 CPG"
  result_metric: "2.3x CTV completion rates"
  specific_example: "Replaced demo targeting with intent-based audiences"
```

## Notes

- Always include compliance disclaimer for regulated industries
- Make case study specific and concrete (not generic)
- Use prospect's language (channel-specific terminology)
- Keep mobile readability in mind (short paragraphs)
- Test variations and iterate based on response rates

## Integration

- Input from: Ecosystem mapping, ICP research, case studies
- Output to: LinkedIn Campaign Manager, sales enablement
- Feeds into: ABM campaigns, sales outreach sequences
