# Kyru Documentation
## Distribution & Formatting Guide

**Internal Reference for Customer Success, Sales, and Support Teams**

---

## File Overview

This documentation repository contains four user guides designed to help restaurant owners implement multi-location management. Each guide serves a specific audience and use case.

### Quick Start Guide (English & Spanish)
- **Audience:** Restaurant owners new to multi-location features
- **Length:** 2-3 pages
- **Time to read:** 10-15 minutes
- **Purpose:** Get started quickly with the basics
- **When to send:** During onboarding, after account setup
- **Formats:** MD, PDF, DOCX, HTML

### Comprehensive Guide (English & Spanish)
- **Audience:** Managers, GMs, consultants implementing multi-location systems
- **Length:** 5-10 pages
- **Time to read:** 30-45 minutes
- **Purpose:** Deep dive into strategies and best practices
- **When to send:** After customer confirms they want to use multi-location features
- **Formats:** MD, PDF, DOCX, HTML

### Distribution & Formatting Guide (English only)
- **Audience:** Internal Kyru team (CSM, sales, support)
- **Purpose:** Reference for how to share and customize documentation
- **When to use:** When preparing materials for customers

---

## Email Distribution Template

### For New Onboarded Customers (Multi-Location)

**Subject:** Get Started with Kyru Multi-Location Management — Quick Start Guide

**Body:**

```
Hi [Name],

Welcome to Kyru! Congratulations on setting up your multi-location account.

To help you get started quickly, I've attached our Quick Start Guide for Multi-Location Management. This 2-3 page guide will walk you through:

1. Accessing your Multi-Location Dashboard
2. Understanding key metrics (Food Cost %, Labor Cost %, Prime Cost %)
3. Using Recipe Comparison to find cost optimization opportunities
4. Using Vendor Pricing Analysis to consolidate suppliers and save money

I recommend spending 15 minutes with this guide this week. It will save you thousands in the long run.

Once you're comfortable with the basics, I have a more comprehensive guide available if you'd like to dig deeper into strategies and best practices.

Let me know if you have any questions!

Best regards,
[Your Name]
Kyru Customer Success
```

### For Customers Ready for Advanced Features

**Subject:** Advanced Strategies for Multi-Location Restaurant Management

**Body:**

```
Hi [Name],

I wanted to follow up on your progress with the Multi-Location Dashboard. Great work getting your locations set up!

Now that you've had a chance to explore the basics, I'd like to share our Comprehensive Guide. This guide covers:

- Detailed metric interpretation and industry benchmarks
- Deep-dive strategies for recipe optimization
- Vendor consolidation tactics that can save $50K+/year
- Best practices from successful multi-location operators
- Advanced topics like seasonal adjustments and trend analysis

This is the resource our most successful customers use to drive operational improvements and savings.

I'm happy to do a brief walkthrough if you'd like to discuss how these strategies apply to your business.

Best regards,
[Your Name]
Kyru Customer Success
```

---

## In-App Embedding

### Help Menu Integration

**Location in app:** Help icon (bottom right, or top menu)

**Structure:**
```
Help Center
├── Getting Started
│   ├── Multi-Location Dashboard (link to Quick Start)
│   ├── Recipe Comparison (section of Quick Start)
│   └── Vendor Pricing (section of Quick Start)
├── Advanced Topics
│   ├── Best Practices (link to Comprehensive Guide)
│   ├── Seasonal Adjustments (section of Comprehensive)
│   └── Trend Analysis (section of Comprehensive)
├── Troubleshooting (link to FAQ in Comprehensive Guide)
└── Contact Support
```

**Implementation:**
- Store guides as HTML files in `/app/help/`
- Embed in iframe or render directly
- Make searchable (so "recipe cost" finds the Recipe Comparison section)
- Add table of contents with jump links

### Content URLs

- `/help/quick-start-en` → Quick Start Guide EN (HTML)
- `/help/quick-start-es` → Quick Start Guide ES (HTML)
- `/help/comprehensive-en` → Comprehensive Guide EN (HTML)
- `/help/comprehensive-es` → Comprehensive Guide ES (HTML)

---

## Website Integration

### Knowledge Base Structure

**URL structure:** `help.kyru.com/multi-location/[section]`

```
help.kyru.com/
├── multi-location/
│   ├── getting-started (Quick Start content)
│   ├── dashboard
│   ├── recipe-comparison
│   ├── vendor-pricing
│   ├── best-practices (Comprehensive content)
│   ├── advanced-topics
│   ├── troubleshooting
│   └── glossary
├── single-location/ (other guides)
└── api/ (developer docs)
```

### SEO Optimization

- Title tags: "Kyru Multi-Location Management: [Section]"
- Meta descriptions: 150-160 characters summarizing section
- H1: Section title
- Internal links: Link between related sections (e.g., "Learn more about Prime Cost" links to comprehensive glossary)
- Schema markup: Use FAQ schema for Troubleshooting sections

### Mobile Optimization

- Responsive design (guides are already mobile-friendly in HTML format)
- Sidebar navigation collapses on mobile
- Print-friendly CSS for PDF export
- Estimated read time displayed (e.g., "15 min read")

---

## Customization Tips

### White-Label Approach

For partners or resellers who want to rebrand guides:

**What to customize:**
1. Logo: Replace Kyru logo with your logo (top left of PDF/HTML)
2. Branding: Change "Kyru" to "Your Company Name" in headers
3. Contact info: Replace "Kyru Support" with your support contact
4. Colors: Update teal (#3EBF8A) and dark (#1A1A1A) to your brand colors
5. Examples: Replace generic "Location A/B/C" with customer's actual location names

**What NOT to customize:**
- Core content (strategies, metrics, best practices)
- Metric thresholds (green/yellow/red ranges)
- Financial examples (ROI calculations)

**Tool:** Use DOCX format for easiest customization (edit in Word, replace logo, save as PDF)

### Adding Customer Success Stories

**Optional section to add:**

"Success Story: [Customer Name]"
- Their multi-location setup (2 locations, type of restaurant)
- Problem they faced ("Food costs were 32% and 35% across locations")
- Action they took ("Switched vendor C from Supplier X to Supplier Y")
- Result ("Saved $2,400/year, food cost now 28% at both locations")

**How to add:** Insert as new page in DOCX, or add section in HTML

---

## Version Control

### Update Process

When features change or new versions are released:

1. **Identify changes** — Which features changed? Which sections need updates?
2. **Update guides** — Edit the Markdown files with new content
3. **Regenerate formats** — Convert updated Markdown to PDF, DOCX, HTML
4. **Version number** — Update footer: "Version 1.1 | Updated June 2026"
5. **Changelog** — Maintain a CHANGELOG.md documenting what changed

### Changelog Example

```
## [1.1] - June 2026
### Added
- Best Practices Replication feature (Phase 3)
- Prime Cost Dashboard section
- Case study: 3-location operator saves $54K/year

### Updated
- Multi-Location Dashboard section (new UI screenshots)
- Recipe Comparison workflow (simplified 4-step process)

### Fixed
- Corrected labor cost % examples (was 24%, now 25%)
```

### Archive Old Versions

- Keep previous versions available (some customers may reference them)
- Label clearly: "Version 1.0 (Archived)"
- Redirect current version to latest

---

## Translation Notes

### Spanish Translation Philosophy

The Spanish guides (Quick_Start_Guide_ES.md, Comprehensive_Guide_ES.md) are authentic Spanish translations, not machine-translated. Key principles:

1. **Preserve meaning over literal translation** — "Prime Cost" stays as "Costo Primo" (accurate financial term)
2. **Use regional Spanish** — Neutral Spanish that works across Latin America and Spain
3. **Restaurant terminology** — Use standard restaurant industry terms in Spanish (e.g., "costo de alimentos" not "precio de comida")
4. **Examples are consistent** — Same scenarios (Margarita, Chicken) used in EN and ES for parity

### Key Terms (EN → ES Translation)

| English | Spanish | Notes |
|---------|---------|-------|
| Food Cost % | Costo de Alimentos % | Or "Costo de Comida" but "Alimentos" is more formal |
| Labor Cost % | Costo de Mano de Obra % | "Mano de obra" is standard payroll term |
| Prime Cost % | Costo Primo % | Direct translation, used in restaurant industry |
| Inventory Accuracy | Precisión de Inventario | Or "Exactitud del Inventario" |
| Vendor | Proveedor | Standard term |
| Recipe | Receta | Standard term |
| SKU | SKU | (Same in Spanish, not translated) |
| Consolidation | Consolidación | Or "Integración de proveedores" |

---

## Distribution Checklist

**When onboarding a new multi-location customer:**

- [ ] Create account with multiple locations
- [ ] Send Quick Start Guide (English or Spanish, based on preference)
- [ ] Send link to online help center (/help/quick-start-en)
- [ ] Schedule follow-up call in 1 week to discuss implementation
- [ ] After call, send Comprehensive Guide if customer wants advanced strategies
- [ ] Add customer to quarterly "Success Stories" email with best practices

**Monthly CSM touchpoint:**

- [ ] Check if customer is using multi-location features (dashboard, comparisons)
- [ ] If not using, resend Quick Start + offer walkthrough
- [ ] If using, ask about specific challenges and share relevant sections of Comprehensive Guide

---

## Support Resources

### Common Questions (For Support Team)

**Q: Where do I find the guides?**
A: Guides are in the `/docs/` folder:
- `quick-start/` → Quick Start guides (EN/ES)
- `comprehensive/` → Comprehensive guides (EN/ES)
- `distribution/` → This guide

**Q: Can I customize the guides for white-labeling?**
A: Yes. Use DOCX format for easiest editing. See "Customization Tips" section.

**Q: How often are guides updated?**
A: When features change (major updates 2-3x/year, minor corrections ongoing). Check version number in footer.

**Q: Which guide should I send to a customer?**
A: Quick Start first (gets them oriented in 15 min). Then Comprehensive after they've explored (30-45 min for deep strategies).

---

**Last Updated:** May 26, 2026
**Version:** 1.0
**Audience:** Internal Kyru Team (CSM, Sales, Support)
