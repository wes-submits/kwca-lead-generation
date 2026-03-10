# Ad Spend Intelligence Guide
## Estimating Competitor & Prospect Ad Spend

---

## Executive Summary

**The Challenge**: Ad spend data is largely private. Direct spend figures are rarely public.  
**The Solution**: Triangulate estimates from multiple data sources, proxies, and signals.

**Three Methods Covered**:
1. **Third-Party Intelligence Services** (paid tools)
2. **Programmatic Spend Estimation** (DSP data, bid streams, public signals)
3. **Facebook Ad Library Scraping** (free, manual + automated)

**Accuracy Expectations**:
- **Directionally accurate**: ±30-50% of actual spend
- **Relative comparison**: Which competitor spends more (reliable)
- **Trend detection**: Spend increasing/decreasing (reliable)
- **Exact figures**: Rarely possible without insider access

---

## PART 1: AD SPEND INTELLIGENCE SERVICES

### Tier 1: Enterprise Intelligence (High Cost, High Detail)

#### **Pathmatics** (now part of Sensor Tower)
- **Cost**: $$$$ ($50K+ annually)
- **Coverage**: Digital display, video, social, mobile
- **Data Source**: ISP panel data, publisher direct relationships
- **Best For**: Enterprise competitive analysis, agency planning
- **Accuracy**: High for top spenders, directional for mid-market
- **kwca Use Case**: Identify which competitors are investing heavily in programmatic

**What You Get**:
- Estimated monthly spend by brand
- Creative rotation analysis
- Publisher/site-level placement data
- Device and geography breakdown
- Spend trends over time

**Limitations**:
- Expensive for small teams
- Limited coverage outside top markets
- Lag time (2-4 weeks)

---

#### **Sensor Tower** (acquired Pathmatics)
- **Cost**: $$$ ($20K-50K annually)
- **Coverage**: Mobile apps, mobile advertising
- **Data Source**: App intelligence + mobile ad networks
- **Best For**: Mobile-first brands, app developers
- **Accuracy**: High for mobile ad spend

**What You Get**:
- Mobile ad spend estimates
- App download intelligence
- Ad network distribution
- Creative analysis

---

#### **SEMrush .Trends** / **Advertising Research**
- **Cost**: $$ ($200-500/month)
- **Coverage**: Google Ads, display advertising
- **Data Source**: Clickstream panel, keyword data
- **Best For**: PPC-heavy brands, B2B companies
- **Accuracy**: Good for Google Ads, directional for display

**What You Get**:
- Estimated PPC spend
- Keyword bidding analysis
- Display ad placement data
- Competitor traffic estimates

---

### Tier 2: Mid-Market Tools (Moderate Cost, Moderate Detail)

#### **SocialPeta**
- **Cost**: $$ ($500-2K/month)
- **Coverage**: Facebook, Instagram, TikTok, Google, more
- **Data Source**: Ad creative scraping, engagement analysis
- **Best For**: Creative intelligence + spend estimation
- **Accuracy**: Directional, better for volume than exact figures

**What You Get**:
- Creative library (millions of ads)
- Estimated impressions/spend by creative
- Competitor creative strategy
- Platform distribution

**kwca Use Case**: Identify DTC brands scaling Facebook spend (high intent need)

---

#### **SpyFu**
- **Cost**: $ ($39-299/month)
- **Coverage**: Google Ads, organic search
- **Data Source**: Keyword scraping, SERP tracking
- **Best For**: PPC keyword research, budget estimation
- **Accuracy**: Good for PPC, limited for display

**What You Get**:
- Estimated PPC budget
- Keyword buying history
- Ad copy variations
- Organic vs. paid mix

---

#### **WhatRunsWhere** (now part of Pathmatics)
- **Cost**: $$ ($300-1K/month)
- **Coverage**: Display advertising
- **Data Source**: Publisher/ad network relationships
- **Best For**: Display creative + placement intelligence

---

### Tier 3: Free/Low-Cost Signals (DIY Intelligence)

#### **Facebook Ad Library** (Free)
- **Coverage**: Facebook, Instagram, Messenger, Audience Network
- **Data**: Active ads, estimated audience size, spend range
- **Limitations**: Only active ads, ranges not exact figures
- **Method**: Manual search or scraping (see Part 3)

**Spend Data Available**:
- "Amount Spent" range (e.g., "$0-$999" or "$100K+" for political)
- "Impressions" range
- Audience size estimate

---

#### **LinkedIn Ad Library** (Free)
- **Coverage**: LinkedIn ads
- **Data**: Active ads, estimated impressions
- **Limitations**: Limited spend data

---

#### **Google Ads Transparency Center** (Free)
- **Coverage**: Google Search, YouTube, Display
- **Data**: Active ads, advertiser identity
- **Limitations**: No spend figures

---

#### **TikTok Creative Center** (Free)
- **Coverage**: TikTok ads
- **Data**: Top ads, creative trends
- **Limitations**: No spend data

---

### Tier 4: Proxy Signals (DIY Estimation)

#### **BuiltWith** / **Wappalyzer**
- **Cost**: $ ($300-1K/month for BuiltWith)
- **What It Shows**: Marketing tech stack
- **Spend Proxy**: More tools = higher sophistication = likely higher spend

**Correlation Signals**:
- Enterprise analytics (Adobe, GA4 360) = $500K+ likely
- Multiple DSPs = $1M+ likely
- CDP + identity resolution = sophisticated operation

---

#### **Job Posting Analysis**
- **Free**: LinkedIn, Indeed, company career pages
- **Spend Proxy**: Hiring spree for marketing roles = budget increase

**Signals to Track**:
- "Paid Social Manager" roles
- "Programmatic Trader" positions
- "Marketing Analyst" hires
- Budget expansion language in JDs

---

#### **Press Release / Earnings Call Mining**
- **Free**: Company investor relations
- **Spend Proxy**: Public companies occasionally disclose marketing spend

**Where to Look**:
- 10-K filings ("Selling, General & Administrative")
- Earnings call transcripts
- Marketing campaign launch announcements
- Agency appointment press releases

---

## PART 2: PROGRAMMATIC AD SPEND ESTIMATION

### The Challenge

Programmatic spend is distributed across multiple DSPs, SSPs, and ad exchanges. No single source sees everything.

### Method 1: Bid Stream Analysis (If You Have Access)

**What You Need**: Access to SSP bid stream data (as a publisher or via partnership)

**What Bid Streams Show**:
- Bid requests by advertiser domain
- CPM bids (not just clears)
- Volume of impressions attempted

**How to Estimate Spend**:
```
Estimated Daily Spend = 
  (Bid Requests × Win Rate × Avg CPM) / 1000

Example:
- 1M bid requests/day
- 5% win rate = 50K impressions
- $5 CPM average
- Daily spend = (50,000 × $5) / 1000 = $250/day
- Monthly = ~$7,500
```

**Sources**:
- **Prebid.js analytics** (if you're a publisher)
- **SSP partnerships** (The Trade Desk, Magnite, etc.)
- **Data clean rooms** (InfoSum, LiveRamp)

---

### Method 2: DSP Platform Intelligence

**If You're a DSP Partner/Client**:

Most DSPs provide **advertiser-level benchmarking** (anonymized):

**The Trade Desk**:
- Vertical spend benchmarks
- CPM trends by category
- Device mix data

**DV360**:
- Category spend insights (Google Ads data)
- Format performance benchmarks

**Amazon DSP**:
- Category spending indices
- Retail media benchmarks

**How to Use**:
1. Get vertical benchmarks from your DSP rep
2. Compare competitor's public presence to benchmarks
3. Estimate based on activity level

---

### Method 3: Publisher Direct Relationships

**If You Work With Publishers**:

Major publishers (news sites, connected TV apps) know who's buying their inventory:

**What Publishers Know**:
- Direct ad server data (DFP/Ad Manager)
- Programmatic guaranteed deals
- Private marketplace (PMP) participation

**How to Access**:
- Partnership conversations
- Publisher intelligence tools (GumGum, Oracle)
- Industry events (publishers talk)

---

### Method 4: Ad Intelligence Tool Aggregation

**Combine Multiple Sources**:

| Source | Coverage | Use For |
|--------|----------|---------|
| Pathmatics | Display, social | Primary estimate |
| SEMrush | Search | Add to total |
| SocialPeta | Social creative | Frequency/volume proxy |
| Facebook Ad Library | Meta properties | Validation |
| LinkedIn Ad Library | LinkedIn | B2B spend |

**Triangulation Formula**:
```
Estimated Total Digital Spend = 
  Pathmatics Display Estimate +
  SEMrush Search Estimate +
  SocialPeta Social Estimate +
  Manual FB/LinkedIn Validation
```

**Accuracy**: ±30-50% for total, better for relative comparison

---

### Method 5: Public Data Correlation

**For Public Companies**:

**Step 1**: Find total marketing spend in 10-K
```
Look for: "Selling, General & Administrative" or "Marketing & Advertising"
```

**Step 2**: Estimate digital % by vertical
| Vertical | Typical Digital % |
|----------|-------------------|
| E-commerce/DTC | 70-90% |
| CPG | 40-60% |
| Financial Services | 50-70% |
| Healthcare | 30-50% |
| B2B SaaS | 60-80% |

**Step 3**: Estimate programmatic % of digital
| Company Type | Programmatic % |
|--------------|----------------|
| Enterprise brand | 40-60% |
| DTC brand | 60-80% |
| B2B | 30-50% |

**Example Calculation**:
```
Company: Large CPG Brand
- Total marketing: $500M (from 10-K)
- Digital %: 50% = $250M
- Programmatic %: 50% = $125M estimated
```

---

## PART 3: FACEBOOK AD LIBRARY SCRAPING

### What You Can Scrape (Free)

**Available Data**:
- Active ads by advertiser
- Ad creative (images, video thumbnails, copy)
- Estimated audience size
- Platform (Facebook, Instagram, Messenger, Audience Network)
- Start date (when ad began running)
- "Amount Spent" range (for political/social issue ads: $0-$99, $100-$499, etc.)
- "Impressions" range
- Demographic targeting (location, age, gender if disclosed)

**Not Available**:
- Exact spend figures (for non-political ads)
- Real-time data (slight delay)
- Historical ads that are no longer active
- Performance metrics (CTR, conversion)

---

### Method 1: Manual Scraping (Free, Slow)

**Step-by-Step**:

1. **Go to**: https://www.facebook.com/ads/library

2. **Search**: Enter company name or keyword

3. **Filter**: 
   - Country
   - Ad status (active/all)
   - Platform

4. **Count Ads**:
   - Scroll through all active ads
   - Note ad volume (more ads = higher spend)

5. **Analyze Creative Rotation**:
   - Count unique creatives
   - More creative rotation = higher spend (testing)

6. **Check Active Duration**:
   - Long-running ads = proven performers = higher spend

7. **For Political/Social Ads**:
   - View "Amount Spent" and "Impressions" ranges
   - Calculate estimated CPM

**Manual Estimation Formula**:
```
Estimated Monthly Spend = 
  (Number of Active Ads × Avg Duration in Days × Estimated Daily Spend per Ad)

Estimated Daily Spend per Ad (rough ranges):
- 1-3 ads: $100-500/day
- 4-10 ads: $500-2K/day
- 11-25 ads: $2K-10K/day
- 25+ ads: $10K+/day
```

---

### Method 2: Automated Scraping (Python)

**⚠️ WARNING**: Automated scraping may violate Facebook's Terms of Service. Use responsibly and at your own risk.

**Unofficial Python Library**: `facebook-ad-library-scraper`

```bash
pip install facebook-ad-library-scraper
```

**Basic Script**:
```python
from facebook_ad_library_scraper import scraper

# Note: Requires Facebook Developer access token
# Get at: https://developers.facebook.com/tools/explorer

ACCESS_TOKEN = 'your_access_token'

ads = scraper.get_ads(
    access_token=ACCESS_TOKEN,
    ad_reached_countries=['US'],
    search_terms='your_brand_name',
    fields=['ad_creation_time', 'ad_creative_bodies', 'ad_delivery_start_time', 
            'ad_delivery_stop_time', 'currency', 'demographic_distribution',
            'impressions', 'spend', 'platforms']
)

for ad in ads:
    print(f"Ad started: {ad['ad_delivery_start_time']}")
    print(f"Platforms: {ad.get('platforms', [])}")
    if 'spend' in ad:
        print(f"Spend range: {ad['spend']}")
    if 'impressions' in ad:
        print(f"Impressions: {ad['impressions']}")
```

**Official API**: Facebook Marketing API

```python
import requests

ACCESS_TOKEN = 'your_access_token'
AD_LIBRARY_API_URL = 'https://graph.facebook.com/v18.0/ads_archive'

params = {
    'access_token': ACCESS_TOKEN,
    'ad_reached_countries': 'US',
    'search_terms': 'brand_name',
    'fields': 'ad_creation_time,ad_creative_bodies,spend,impressions,platforms'
}

response = requests.get(AD_LIBRARY_API_URL, params=params)
data = response.json()

for ad in data.get('data', []):
    print(ad)
```

**API Limitations**:
- Rate limits apply (varies by access level)
- Only active ads (unless archived)
- Limited fields for non-political ads
- Requires Facebook Developer account

---

### Method 3: Third-Party Scraping Tools

#### **AdEspresso** (by Hootsuite)
- **Cost**: $ (part of Hootsuite)
- **Feature**: Facebook ad monitoring
- **Best For**: Ongoing competitor tracking

#### **BigSpy**
- **Cost**: $ (freemium)
- **Coverage**: Facebook, Instagram, Twitter, Pinterest
- **Feature**: Ad database, creative search

#### **PowerAdSpy**
- **Cost**: $$ ($49-349/month)
- **Coverage**: Facebook, Google, Instagram, YouTube
- **Feature**: Ad intelligence, landing page tracking

---

### Method 4: Chrome Extensions (Semi-Automated)

#### **Turbo Ad Finder** (discontinued, alternatives exist)
- Replaced by: **Ad Library Helper** extensions

#### **Facebook Ad Library Helper**
- **Cost**: Free
- **Feature**: Enhanced browsing, download options

**How to Use**:
1. Install extension
2. Browse Facebook Ad Library
3. Export data to CSV
4. Analyze in spreadsheet

---

## ESTIMATION FORMULAS

### Formula 1: Ad Volume Proxy

```
Estimated Monthly Facebook Spend = 
  (Active Ad Count × Avg Days Running × Daily Spend Estimate)

Daily Spend Estimate by Ad Volume:
- 1-5 active ads: ~$200/day each = $1K/day total
- 6-15 active ads: ~$500/day each = $5K/day total
- 16-30 active ads: ~$1K/day each = $20K/day total
- 30+ active ads: ~$2K/day each = $60K+/day total

Monthly = Daily × 30
```

**Example**:
- Competitor has 12 active ads
- Average running 45 days
- Estimation: 12 × $500/day = $6K/day = ~$180K/month

---

### Formula 2: Creative Rotation Rate

```
High creative rotation = Higher spend (testing)

Rotation Rate = New Ads per Week / Total Active Ads

Spend Proxy:
- <0.5 (slow rotation): Established campaigns, steady spend
- 0.5-1.5 (moderate): Active optimization, growing spend
- >1.5 (fast rotation): Aggressive testing, high spend
```

---

### Formula 3: Audience Size Correlation

**From Ad Library**: Estimated audience size

```
Audience Size Spend Proxy:
- <10K: Likely retargeting, lower spend
- 10K-100K: Prospect testing, moderate spend
- 100K-1M: Scale prospecting, higher spend
- 1M+: Broad reach, very high spend
```

---

### Formula 4: Platform Distribution

```
Platform Mix Indicates Budget:
- Facebook only: Conservative, lower spend
- Facebook + Instagram: Standard, moderate spend
- All platforms (FB, IG, Messenger, Audience Network): Full funnel, high spend
```

---

## KWCA APPLICATION: Using Ad Spend Intel

### Use Case 1: Account Prioritization

**High Spend Signals = High Intent Need**:
- Companies spending $100K+/month have sophisticated audiences
- They're likely hitting platform limitations
- They have budget for data solutions

**Scoring Model**:
| Spend Level | kwca Priority | Outreach Approach |
|-------------|---------------|-------------------|
| $10K-50K/month | B | Educational |
| $50K-200K/month | A | Solution-focused |
| $200K-500K/month | A+ | Direct value prop |
| $500K+/month | A++ | Executive outreach |

---

### Use Case 2: Personalization

**Reference Their Spend in Outreach**:

```
"I noticed {{company}} is running 15+ active Facebook campaigns. 
Most brands at that scale are dealing with audience fatigue. 
Are you seeing CPMs climb as you scale?"
```

```
"{{company}} appears to be investing heavily in programmatic 
(Pathmatics estimates $200K+/month). Are you satisfied with 
the data quality for those campaigns?"
```

---

### Use Case 3: Timing & Trigger Identification

**Spend Increase = Buying Signal**:
- New CMO hired + spend up 50% = Change agent
- New product launch + heavy spend = Intent need
- Q4 ramp + spend surge = Seasonal opportunity

**Spend Decrease = Different Opportunity**:
- Spend down but still active = Efficiency focus (kwca value prop)
- Reduced creative rotation = Optimization mode

---

### Use Case 4: Competitive Positioning

**Show Prospect vs. Competitor Spend**:

```
"Based on public ad intelligence, {{competitor_1}} is spending 
~3x more than {{company}} on Facebook. That suggests they're 
capturing intent signals you're not. Want to see what keywords 
their audiences are searching for?"
```

---

## RECOMMENDED TOOL STACK FOR KWCA

### For DTC/Facebook-Heavy Prospects:

| Tool | Cost | Use |
|------|------|-----|
| Facebook Ad Library | Free | Daily monitoring |
| SocialPeta | $$ | Creative + spend trends |
| Pathmatics | $$$$ | Validation |
| Triple Whale (client) | N/A | Post-pilot validation |

### For Enterprise/Programmatic Prospects:

| Tool | Cost | Use |
|------|------|-----|
| Pathmatics | $$$$ | Primary source |
| SEMrush | $$ | Search validation |
| BuiltWith | $$ | Tech sophistication |
| Manual research | Free | Earnings calls, press |

### Budget-Conscious Option:

| Tool | Cost | Use |
|------|------|-----|
| Facebook Ad Library | Free | Core research |
| SEMrush (basic) | $ | Search trends |
| BuiltWith (basic) | $ | Tech stack |
| LinkedIn Sales Nav | $$ | Contact + company intel |

---

## DATA SOURCES SUMMARY

| Source | Type | Cost | Accuracy | Best For |
|--------|------|------|----------|----------|
| Pathmatics | Paid | $$$$$ | High | Enterprise programmatic |
| Sensor Tower | Paid | $$$$ | High | Mobile advertising |
| SocialPeta | Paid | $$ | Medium | Creative + social |
| SEMrush | Paid | $$ | Medium | Search + display |
| Facebook Ad Library | Free | $ | Low-Medium | Meta properties |
| BuiltWith | Paid | $$ | Low | Tech stack proxy |
| Job postings | Free | $ | Low | Growth signals |
| Earnings reports | Free | $ | Medium (public co) | Total marketing |
| Bid stream | Partnership | $$ | High | Direct access |

---

## ACCURACY EXPECTATIONS

### What You Can Reliably Determine:
✅ **Relative spend** (Company A spends more than B)  
✅ **Spend trends** (Increasing, decreasing, flat)  
✅ **Platform mix** (Heavy Facebook vs. programmatic)  
✅ **Creative volume** (Testing aggressively vs. steady state)  
✅ **Campaign timing** (New launches, seasonal patterns)  

### What You Cannot Reliably Determine:
❌ **Exact spend figures** (±30-50% is best case)  
❌ **ROAS/performance** (private data)  
❌ **Offline spend** (TV, print, radio)  
❌ **Strategy effectiveness** (what's working)  

---

*Generated: 2026-03-10*  
*Purpose: Ad spend intelligence for kwca account targeting*  
*Accuracy: Directional and comparative, not exact*
