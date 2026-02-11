---
customer: "Dovista (Mockfjord)"
date: 2026-02-05
project_type: AI Visual Discovery | AI Guided Selling | Hybrid
status: active
tags:
  - scoping-notes
  - windows-doors
  - b2c
  - nordic
  - ai-discovery
---

# Dovista - Scoping Notes

## Calls

| Date | Meeting Type | Threekit Reps | Customer Reps |
|------|--------------|---------------|---------------|
| Dec 2025 | First Call | Stephane Ollier (SE), Patrice Arnera (Head of Services EMEA/Innovation) | Fredrik Hjort (DCJ Team), Frank Schad (Commercial Digitalization/E-commerce) |
| Jan 13, 2026 | Weekly Update | Stephane Ollier | Fredrik Hjort |
| Jan 16, 2026 | Scoping Session | Stephane Ollier | Fredrik Hjort |
| Jan 26, 2026 | Demo Feedback | Stephane Ollier, Patrice Arnera | Fredrik Hjort |

## Reference Links

- **Company Website**: mockfjard.se (Mockfjord brand)
- **Parent Company**: Dovista (dovista.com)
- **Existing Configurator**: On Mockfjord site - built specifically for Svenska Fönster, described as "old CPQ interface"
- **Image Gallery**: mockfjard.se (BRF section, inspiration images)
- **Partner**: Torit (technical integration partner)

## Important Dates

| Milestone | Date | Notes |
|-----------|------|-------|
| Internal Demo | Feb 23, 2026 | Big internal management meeting - need MVP/POC ready |
| Demo Ready | Feb 20, 2026 | Fredrik needs to test before presenting |
| New Website Launch | Early April 2026 | Mockfjord site relaunch |
| Nordbygg Tradeshow | Spring 2026 | Major Nordic building industry event - potential showcase |

## Customer Vision

Dovista wants to become a digitally-led organization with harmonized tools across all 14 brands in 25 European markets. The immediate focus is a pilot with Mockfjord (Swedish D2C brand) to prove AI-guided selling capabilities before rolling out across the group.

> [!quote] Customer Quote
> "This is a survival product for us... people are starting to understand that we can move this pretty fast, that they see this."
> — Fredrik Hjort

> [!quote] Customer Quote
> "What we really want is to have a really, really high quality product delivery here... this is a game changer here compared to what we have today. Most of the times we can't show them anything about their house."
> — Fredrik Hjort

## Problem Statement

1. **Poor customer discovery experience**: Existing configurator requires expert knowledge - "you have to be an expert" to use it. Too complex for end consumers.

2. **No visualization capability**: Customers cannot see how windows would look on their actual homes. "Today, a quote from us is just text."

3. **Limited customer intelligence**: No data flows back from ERP to marketing. "All information gets sent to the ERP system and we don't get any information back... we're just going a long ways away from understanding where do the leads come from, what makes them convert."

4. **Siloed brand operations**: 14 brands working independently with inconsistent digital experiences.

5. **High conversion costs**: "Window Tinder" experiment required heavy marketing spend. KPI = Conversion & Conversion Costs.

## Metrics

Key metrics to be improved:
- **Conversion rate** - Primary KPI
- **Conversion cost** - Reduce marketing spend per converted lead
- **Lead quality** - Capture insights about customer preferences
- **Time to quote** - Speed up the customer journey
- **Customer engagement** - Increase time on site, reduce bounce

## Personas

**Primary Users (B2C):**
- **Homeowner - Window Shopper**: Browsing, not ready to commit. Wants inspiration without uploading personal images. "They're just window shopping... they don't feel secure about uploading."
- **Homeowner - Active Buyer**: Has a project in mind, willing to upload house images, wants to see specific products on their home
- **Homeowner - Renovation Project**: Planning larger renovation, needs multiple windows, may be changing house color

**Secondary Users (B2B):**
- **Property Manager**: Managing building portfolios (e.g., Vasakronan - 50M EUR project). Needs quotes for multi-story buildings
- **BRF (Housing Cooperative) Representatives**: Making decisions for residential buildings

**Internal Users:**
- **Sales Representatives**: Visit customers at their homes, need mobile tools
- **Carpenters/Installers**: Different approach than end consumers

## User Journey / Selling Process

**Current State:**
```mermaid
flowchart LR
    A[Visit Website] --> B[Complex CPQ Interface]
    B --> C[Requires Expert Knowledge]
    C --> D[Text-Only Quote]
    D --> E[Manual Follow-up]
    E --> F[Lost Customer Data]
```

**Envisioned Future State:**
```mermaid
flowchart LR
    A[Enter Experience] --> B{Choose Path}
    B -->|Inspiration| C[Style Discovery]
    B -->|Ready to Buy| D[Upload Home Image]
    C --> E[AI Recommendations]
    D --> F[AI Window Detection]
    F --> G[Configure & Visualize]
    E --> G
    G --> H[Visual Quote with Image]
    H --> I[Lead to HubSpot]
    I --> J[Sales Intelligence]
```

## Outputs

Desired user takeaways from the experience:
- **Visual quote document** with configured windows shown on customer's actual home
- **Product recommendations** based on house style, preferences, and location
- **Before/after visualization** showing new windows on their home
- **Specification summary** with dimensions, materials, colors
- **Lead intelligence** for sales follow-up (preferences, style, budget indicators)

---

## Agent Body of Knowledge (AI)

### Structured Product Data
- **Source**: Product catalog, likely SAP S4/HANA (Christian Christensen mentioned S4 migration in progress)
- **Format**: TBD - Need confirmation
- **Scope**: Mockfjord window products (Ultima line mentioned), Svenska Fönster products
- **3D Assets**: "We have everything set up in 3D... our product images are all 3D images"

### Descriptive Content & Media
- **Product imagery**: 3D rendered product images available
- **Marketing content**: Case studies on website, inspiration galleries
- **Technical specs**: Installation guides, energy ratings, Swan eco-certification
- **House styles**: Mix of traditional Swedish (1800s), 1970s-80s brutalist, Mexeltegel brick homes

### Knowledge Base
- **Installation requirements**: Varies by facade type (wood vs brick vs Mexeltegel)
- **Regional preferences**: Sweden likes white/painted wood, Norway likes natural wood
- **Environmental certifications**: Swan logo certification (highest environmental standard in Scandinavia)

### Sales Process & Logic
- **Discovery questions**: House type, opening type, color preference, energy needs, sound insulation
- **Recommendation logic**: Based on house style, climate zone, budget, aesthetic preferences
- **Pricing factors**: Material, size, glazing type, installation complexity (brick vs wood facade)

## Discovery Inputs (AI)

| Input | Purpose | Maps To |
|-------|---------|---------|
| House style (traditional, modern, 70s-80s, contemporary) | Match window aesthetic | Product style family |
| Upload home image | Detect windows, analyze style | AI recommendation, visualization |
| Color preference (black, white, wood, painted) | Filter products | Frame color options |
| Energy requirements | Filter by insulation | Glazing type (double/triple) |
| Opening type preference | Determine function | Opening mechanism |
| Inside/outside color preference | Customization | Interior/exterior finish |
| Location (coastal, urban, rural) | Climate considerations | Weather resistance specs |
| Budget indicator | Guide recommendations | Price tier |

## Input/Output Criteria (AI)

**Scenario 1 - Mexeltegel Brick House:**
- **Input**: Upload image of white brick 1970s house, black window preference
- **Expected Output**: Recommend Ultima windows in black, show visualization, suggest matching trim

**Scenario 2 - Traditional Red Cottage:**
- **Input**: Traditional house style, green or white window preference
- **Expected Output**: Classic profile windows with traditional latches, show on uploaded image

**Scenario 3 - Multi-Story Building:**
- **Input**: Upload BRF building image, property manager persona
- **Expected Output**: Detect all windows (4-44+), provide bulk configuration, generate project quote

## Lead Intelligence (AI)

Enhanced lead data to capture:
- Style preferences (colors, profiles selected/viewed)
- House type and age indication
- Project scope (single window vs whole house)
- Price sensitivity (based on options selected)
- Timeline urgency
- Contact method preference
- Geographic/climate zone

> [!quote] Customer Quote
> "What we found out... there's a lot of visual discovery, how you want the end product to look like, but in a lot of areas it's not just how it looks like, it's also the weather, the heat, the wind, the humidity—all these type of things. So we also build that into our AI."
> — Patrice Arnera

---

## Visualization Requirements

**Image Upload & Analysis:**
- Upload exterior home images
- AI detects windows automatically (handles 4-44+ windows per building)
- Analyze house style for recommendations
- Handle multi-story buildings and residential homes

**Rendering Capabilities:**
- Place configured windows on uploaded home image
- Maintain perspective and lighting
- Support facade color changes (red house to black house, etc.)
- Show interior and exterior views
- Generate close-up detail views

**Quality Expectations:**
- Photo-realistic output expected long-term
- Current wireframe acceptable for demo
- Reference: Louis Vuitton, Dior quality examples shown

> [!quote] Customer Quote
> "The most important thing for me here is that we can show something that are close to what we have... this part is more impressive."
> — Fredrik Hjort

## Integration

| System | Type | Integration Need |
|--------|------|------------------|
| HubSpot | CRM | Lead capture, session intelligence, insights export |
| SAP S4/HANA | ERP | Product data source (future), order processing |
| Torit | Technical Partner | Configuration/pricing engine integration |
| Website | Embed | Mockfjord.se new site (April 2026 launch) |

## Internationalization

**Languages Required:**
- Swedish (primary for Mockfjord)
- Norwegian (Natre brand expansion)
- Danish (future)
- English (UK brands: Velfac, Rationel, Sidey, Devol, Dobie Plus)
- German, French, Swiss (future - "2027 for Southern regions")

**Regional Considerations:**
- House style recognition must adapt to local architecture
- Color preferences vary by country (Norway: natural wood, Sweden: painted white)
- Certification requirements differ by market

## Other Requirements

- **Security**: GDPR compliance for image uploads and lead data
- **Performance**: Mobile-friendly for sales reps visiting homes
- **Scalability**: Pilot with Mockfjord, expand to 14 brands across 25 markets

## Roles & Responsibilities

| Name | Role | Responsibility |
|------|------|----------------|
| Fredrik Hjort | DCJ Team (Digital Commercial Journey) | Product owner, Mockfjord pilot lead, harmonization across brands |
| Frank Schad | Commercial Digitalization & E-commerce Director | Strategic direction, budget approval, German e-commerce |
| Morton Denzrydborg | Manager of Business Development (Denmark) | Internal champion, business case |
| David (Torit) | Technical Partner | Integration, configuration engine |
| Christian Christensen | IT | ERP/SAP - currently blocked by S4 migration |

## Competitive Landscape

- No comparable AI-powered window visualization tool in Swedish market
- Traditional competitors: Tribekas, Caparka (France)
- Differentiation opportunity: "There is nothing out there right now that's easy available... that are providing anything like this in Sweden"

## Budget & Commercial Notes

- Initial pilot for Mockfjord brand
- Potential for B2B cross-sell to Torit users (building/property managers)
- Expansion to other brands would bring additional budget
- Vasakronan project: 50M EUR window replacement project as reference

## Other Notes

- Strategic expansion plan: Adding installation services across Europe (UK first)
- Nordbygg tradeshow in Spring 2026 - potential showcase opportunity
- Dovista acquiring installation companies to get closer to end customers
- 3D assets already exist for Svenska Fönster products - can leverage for rendering
- Fredrik training Adobe Firefly on window images for content generation

## Outstanding Questions

> [!warning] Follow-up Required
> - [ ] Confirm product data source and format (SAP S4, PIM, other?)
> - [ ] Get access to 3D asset library for product rendering
> - [ ] Clarify Torit integration scope and technical requirements
> - [ ] Confirm HubSpot instance details and integration specifications
> - [ ] Determine pricing data availability and structure
> - [ ] Identify specific Ultima product line attributes and options
> - [ ] Confirm mobile requirements for sales rep usage
> - [ ] Discuss multi-brand architecture for future rollout
