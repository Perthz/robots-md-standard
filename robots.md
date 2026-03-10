# Agenti NZ - AI Agent Discovery & API Documentation

This file helps AI agents, crawlers, and tools discover and understand how to interact with Agenti NZ's digital services.

**Last Updated:** March 2026  
**Website:** https://agenti.nz  
**Organization:** Agenti NZ - We build AI operating system for business.

---

## 🤖 For AI Agents & Tools

### Primary Content API

**Endpoint:** `/api/trpc/content.markdown`  
**Method:** GET  
**Format:** JSON response with markdown content  
**Authentication:** None required (public)

**Response Structure:**
```json
{
  "content": "# Agenti NZ - AI Automation...",
  "format": "markdown",
  "version": "1.1",
  "lastUpdated": "2026-03-10T00:00:00.000Z"
}
```

**Use Cases:**
- AI agents fetching website content for analysis
- Content aggregators indexing business information
- LLM context enrichment for customer support bots
- Marketing automation tools gathering company details
- Research tools collecting information about services

**Example Usage:**
```bash
curl https://agenti.nz/api/trpc/content.markdown
```

---

## 📋 Available Content Sections

The markdown endpoint includes:

- **Overview:** Company mission and tagline ("We build AI operating system for business.")
- **Problem Statement:** Pain points for NZ SMEs (Drowning in admin)
- **Solution:** What agentic AI does and capabilities (Acts, Not Just Talks)
- **Services:** AI Discovery Audit, Custom Agent Build, Managed AI Retainer
- **Use Cases:** Tradie's Assistant, Smart Retailer, Admin Guardian, Hospo Helper, Property Pro, Wellness Co-Pilot, Consultant's Edge
- **Case Studies:** EVX (rental business), Smart Retailer (ecommerce)
- **Statistics:** Key metrics and impact numbers (40% time saved, 24/7 operations)
- **FAQ:** Common questions about costs, privacy, implementation
- **How It Works:** 3-step process (Discovery, Build, Launch)
- **Contact Information:** Email and website

---

## 🔗 Other API Endpoints

### Contact Form Submission
**Endpoint:** `/api/trpc/contact.submit`  
**Method:** POST  
**Authentication:** None required (public)

**Request Body:**
```json
{
  "name": "string",
  "email": "string",
  "company": "string (optional)",
  "message": "string"
}
```

**Response:**
```json
{
  "success": true
}
```

---

## 📄 Website Pages & Routes

| Route | Purpose | Content Type |
|-------|---------|--------------|
| `/` | Homepage | Landing page with hero, services, testimonials |
| `/blog` | Blog Index | List of articles and guides |
| `/case-studies/evx` | EVX Case Study | Detailed case study for EV rental business |
| `/case-studies/retail` | Retail Case Study | Detailed case study for ecommerce retail |
| `/contact` | Contact Form | Email contact form alternative to Calendly |
| `/openclaw/success` | Installation Success | Confirmation page for OpenClaw installation |

---

## 🔐 Data & Privacy

- **Data Handling:** Privacy Act 2020 compliant
- **Data Storage:** NZ-based servers
- **Data Sharing:** No data shared with third parties
- **API Rate Limiting:** None (public endpoints)
- **Caching:** Content updates reflected within 1 hour

---

## 📊 Content Metadata

**Organization Name:** Agenti NZ  
**Industry:** AI Automation & Business Process Automation  
**Location:** New Zealand  
**Primary Service:** Custom AI agent development for SMEs  
**Target Market:** NZ small and medium enterprises  
**Contact Email:** call@agenti.nz  
**Website:** https://agenti.nz

---

## 🎯 Key Business Information

### Services Offered
1. **AI Discovery Audit** - $499 (90-minute consultation)
2. **Custom Agent Build** - From $2,500 (bespoke automation)
3. **Managed AI Retainer** - $750/month (ongoing support)

### Key Statistics
- 50+ businesses automated
- 2,000+ hours saved annually
- $3,200 average monthly savings per client
- 40% average time saved on admin tasks
- 100% code ownership (no vendor lock-in)

### Implementation Timeline
- Simple automations: 2-3 weeks
- Standard projects: 4-8 weeks
- Complex systems: 8-10 weeks

---

## 🔄 Content Update Schedule

- **Markdown Content:** Updated weekly
- **Case Studies:** Updated as new projects complete
- **Statistics:** Updated monthly
- **FAQ:** Updated as new questions arise

---

## 🚀 Integration Guidelines for AI Agents

### Best Practices
1. **Cache the markdown content** - Refresh every 24 hours to reduce load
2. **Parse markdown sections** - Use headers to organize content
3. **Extract structured data** - Convert pricing and stats to JSON
4. **Respect rate limits** - Although none currently enforced, implement backoff
5. **Identify yourself** - Include User-Agent header with your tool name

### Example Integration (Python)
```python
import requests
import json

response = requests.get('https://agenti.nz/api/trpc/content.markdown')
data = response.json()
markdown_content = data['content']
print(markdown_content)
```

### Example Integration (JavaScript)
```javascript
fetch('https://agenti.nz/api/trpc/content.markdown')
  .then(res => res.json())
  .then(data => console.log(data.content))
  .catch(err => console.error(err));
```

---

## 📞 Support & Questions

For questions about this API or content:
- **Email:** call@agenti.nz
- **Website:** https://agenti.nz
- **Contact Form:** https://agenti.nz/contact

---

## 📜 License & Attribution

When using content from this API:
- **Attribution:** Please credit "Agenti NZ" when using content
- **Commercial Use:** Contact call@agenti.nz for licensing questions
- **Modification:** Do not modify content without permission

---

## 🔄 Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Feb 2026 | Initial release with markdown endpoint |
| 1.1 | Mar 2026 | Updated branding and expanded use cases |

---

**Note:** This robots.md file is designed to help AI agents discover and understand how to interact with Agenti NZ's services. It complements the standard robots.txt file for search engines.
