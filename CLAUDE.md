# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a content marketing project for a mobile modular buildings business, containing professionally written website content, design guidelines, and business strategy documentation. The goal is to create a high-converting B2B website targeting customers who rent, buy, and lease mobile modular buildings.

## Repository Structure

### Core Documentation
- `DESIGN_CONTENT_GUIDELINES.md` - Comprehensive design system, color schemes (#1B365D navy, #4A90B8 steel blue), typography (Inter/Roboto), layout principles, and component specifications
- `mobile_modular_site_plan.md` - Website architecture, navigation structure, SEO strategy, and business planning
- `DesignScreenshots.docx` - Visual design references and mockups

### Content Organization
- **Homepage**: `homepage.md` - Main landing page content
- **Solutions Pages** (6 files): Content for specific building types (office, classrooms, restrooms, restaurants, healthcare, security)
- **Industry Pages** (6 files): Targeted content for education, construction, healthcare, government, retail, and emergency response sectors  
- **Company Pages** (4 files): About us, process, quality standards, and locations
- **Resource Pages** (4 files): Product gallery, case studies, planning tools, and FAQ
- **Contact**: `contact.md` - Contact information and forms

## Design System

### Colors
- Primary: Deep Navy Blue (#1B365D) for headers, navigation, primary buttons
- Secondary: Steel Blue (#4A90B8) for secondary buttons, highlights, links
- Background: Clean White (#FFFFFF)
- Accent: Success Green (#10B981), Warning Orange (#F59E0B)

### Typography
- Primary: Inter or Roboto (sans-serif) for headers and body
- Secondary: Roboto Slab (serif) for accent headers and testimonials
- Minimum body text: 16-18px for readability

### Layout
- Container width: 1200px maximum
- Grid system: 12-column responsive grid
- Margins/padding: 20px mobile, 40px tablet, 60px desktop

## Content Strategy

### Target Keywords
- Primary: "mobile modular buildings", "portable classrooms", "modular office buildings"
- Industry-specific: Healthcare facilities, construction site offices, emergency response buildings
- Geographic: Targets continental United States

### SEO Requirements
- Content depth: 2,000-3,500 words per page
- Local SEO targeting for service areas
- Schema markup for business, products, and reviews
- Page load time target: under 3 seconds

## Business Context

### Target Market
- B2B customers in education, construction, healthcare, government, retail, and emergency response
- Decision makers requiring rental, purchase, or lease options
- Geographic focus: Continental United States

### Conversion Goals
- Quote request forms on every page
- Phone call conversions
- Email lead capture
- Trust-building through case studies and testimonials

## Implementation Notes

This content is ready for implementation using:
- Static site generators (Gatsby, Next.js, Hugo)
- CMS platforms (WordPress, Contentful, Strapi)
- Custom web development with modern frameworks

All content is professionally written, SEO-optimized, and includes strategic placement of calls-to-action and conversion elements.

## Website Implementation - amanmodular-website

The content has been implemented as a modern Next.js 15 application with comprehensive page structure and navigation.

### Development Commands

```bash
cd amanmodular-website
npm run dev     # Start development server (localhost:3000)
npm run build   # Create production build
npm run lint    # Check code quality
npm start       # Start production server
```

### Technology Stack

- **Framework**: Next.js 15.0.3 with App Router
- **React**: Version 19.0.0 for latest features
- **Styling**: Tailwind CSS with custom design system
- **Animation**: Framer Motion for smooth transitions
- **Icons**: Lucide React for consistent iconography
- **TypeScript**: Full type safety throughout the application
- **Components**: Modular, reusable React components

### Complete Page Structure

#### Solutions Pages (/solutions/*)
- `/solutions` - Main solutions landing page
- `/solutions/office-buildings` - Professional office spaces
- `/solutions/portable-classrooms` - Educational facilities
- `/solutions/restroom-facilities` - Sanitation solutions
- `/solutions/restaurant-food-service` - Food service buildings
- `/solutions/healthcare-facilities` - Medical-grade facilities (to be created)
- `/solutions/security-buildings` - Security checkpoints (to be created)

#### Industries Pages (/industries/*)
- `/industries` - Industries overview (to be created)
- `/industries/education` - Educational sector solutions
- `/industries/construction` - Construction industry (to be created)
- `/industries/healthcare` - Healthcare sector (to be created)
- `/industries/government` - Government solutions (to be created)
- `/industries/retail-commercial` - Retail & commercial (to be created)
- `/industries/emergency-response` - Emergency services (to be created)

#### Locations Pages (/locations/*)
- `/locations` - All locations overview (to be created)
- `/locations/california` - California state coverage
- `/locations/texas` - Texas coverage (to be created)
- `/locations/florida` - Florida coverage (to be created)
- `/locations/new-york` - New York coverage (to be created)
- `/locations/illinois` - Illinois coverage (to be created)
- `/locations/all` - Complete location directory (to be created)

#### Resources Pages (/resources/*)
- `/resources` - Resources overview (to be created)
- `/resources/product-gallery` - Product showcase (to be created)
- `/resources/case-studies` - Customer success stories
- `/resources/planning-tools` - Planning resources (to be created)
- `/resources/faq` - Frequently asked questions (to be created)

#### Company Pages (/company/*)
- `/company` - Company overview (to be created)
- `/company/about-us` - Company history and mission
- `/company/our-process` - Our methodology (to be created)
- `/company/quality-standards` - Quality assurance (to be created)

#### Core Pages
- `/` - Homepage with full feature set
- `/quote` - Interactive quote request form
- `/contact` - Multi-method contact page

### Design System Implementation

- **Colors**: Navy Blue (#1B365D), Steel Blue (#4A90B8), gradients
- **Typography**: Inter primary, Roboto Slab secondary
- **Components**: PageLayout, PageHeader, reusable UI components
- **Animations**: Framer Motion for scroll reveals, hover effects
- **Responsive**: Mobile-first design with Tailwind breakpoints

### Key Features

- **Navigation**: Restructured with Locations as separate menu
- **Page Templates**: Consistent layout patterns across all pages
- **Interactive Elements**: Hover effects, animations, smooth transitions
- **Content Management Ready**: Structured for CMS integration
- **SEO Optimized**: Metadata, semantic HTML, performance optimized

### CMS Integration Preparation

All pages are structured with:
- Standardized data models in `/src/data/demo-data.ts`
- Reusable page components for consistent layouts
- TypeScript interfaces ready for database integration
- Dynamic content areas marked for CMS connection
- Image optimization prepared for CDN integration