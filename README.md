# Namma Laundry Reimagined

Act as a 20+ years experienced senior UI/UX designer and full-stack web developer.

This is an EXISTING GitHub project. Do NOT create a new project and do NOT restart the design.

GitHub repository:
https://github.com/Poomani21/namma-laundry-reimagined.git

The repository is public. Use the existing codebase and continue from the current implementation.

IMPORTANT

The previous build was paused because the build was unsuccessful.

Your first priority is to inspect the existing repository, understand what has already been completed, fix the current build/type errors, and then continue the remaining implementation.

Do NOT unnecessarily recreate, replace, or redesign existing completed components/data.

Already completed — KEEP AND REUSE

The existing project already has:

Namma Laundry logo/CDN asset

Favicon

Brand-aligned generated images

Existing design system in src/styles.css

Bottle Green + Gold + Ivory brand colours

Marcellus + DM Sans typography

Existing card/gold-rule/green-surface utilities

src/lib/site.ts

src/data/services.ts

src/data/pricing.ts

src/data/knowledge.ts

src/data/reviews.ts

Header

Footer

CtaBar

Existing service data

Existing pricing catalogue

Existing knowledge-centre content

Existing reviews

Preserve all of these unless a change is genuinely required to fix an error.

STEP 1 — FIX BUILD FIRST

Inspect the entire existing project and run the appropriate build/typecheck.

Fix the existing errors before adding unnecessary features.

Known current issues:

Some components reference route paths that do not exist yet.

CtaBar uses button variants:

gold

outlineLight

ghostLight

Add these variants properly to the existing src/components/ui/button.tsx rather than replacing the button component.

Do not use temporary hacks, any, ignored TypeScript errors, or disabled type checking.

The final project must build successfully with zero TypeScript/build errors.

STEP 2 — COMPLETE THE MISSING ROUTES

After the build foundation is fixed, create the missing routes using the existing architecture and data.

Required pages:

Home /

Services /services

Individual service /services/$slug

Pricing /pricing

Online Estimate /estimate

Knowledge Centre /knowledge

Individual article /knowledge/$slug

About /about

Reviews /reviews

Contact/Booking /contact

Use the existing service, pricing, knowledge and review data instead of duplicating content.

STEP 3 — HOME PAGE

Create a premium but simple local-business homepage.

The homepage should clearly communicate:

What Namma Laundry does → Why customers need it → Services → Pricing/Estimate → Why choose us → Reviews → Service areas → CTA

Highlight approximately 10 years of local experience.

Use the existing brand system and images.

Primary conversion actions:

Get Estimate

WhatsApp

Call

Book Order

Do not overload the homepage.

STEP 4 — SERVICES

Use the existing src/data/services.ts.

Create:

Services listing page

Show all major services in a clean, easy-to-scan layout.

Individual service pages

Each $slug page should dynamically use the existing service data.

Include where available:

Service title

Description

Benefits

Process

Pricing/estimate CTA

Recommended frequency

FAQs

Related services

WhatsApp / Call / Estimate CTA

These pages must also be suitable as Google Ads landing pages.

STEP 5 — PRICING

Use the existing src/data/pricing.ts.

Create a clean pricing page that is easy to understand on mobile.

Do not invent new prices.

Organize the existing pricing catalogue clearly by service/category.

Include a prominent:

Get Online Estimate

CTA.

Keep the pricing structure backend-ready so prices can later be connected to an admin/backend system.

STEP 6 — ONLINE ESTIMATE

Create an interactive estimate page using the existing pricing data.

Customer should be able to:

Select service/category

Select item

Select quantity

See estimated total

Review estimate

Continue to:

WhatsApp

Call

Book Order

Keep the estimator simple and mobile-friendly.

Do not create unnecessary authentication or backend functionality at this stage.

STEP 7 — KNOWLEDGE CENTRE

Use the existing src/data/knowledge.ts.

Create:

Knowledge Centre listing

Individual article pages using $slug

Make articles easy to read on mobile.

Include useful categories/topics such as:

Blanket care

Curtain cleaning

Carpet cleaning

Upholstery

Monsoon care

Pet households

Children/elderly households

Dust/allergen care

Fabric care

Washing vs dry cleaning vs specialised cleaning

Do not replace the existing researched content with generic AI filler.

STEP 8 — ABOUT / REVIEWS / CONTACT

About

Present Namma Laundry as an experienced, established and trustworthy local laundry-care provider.

Reviews

Use the existing review data.

Contact

Provide:

Phone

WhatsApp

Service areas

Contact/booking CTA

Clear enquiry flow

Use the existing information from src/lib/site.ts.

STEP 9 — SEO

Every major page should have proper:

Page title

Meta description

Canonical-friendly structure

Relevant heading hierarchy

Service-specific metadata

Knowledge article metadata

Remove any default Lovable titles/descriptions.

The root title and description must represent Namma Laundry, not Lovable.

STEP 10 — ROOT LAYOUT

Update __root.tsx.

Make sure:

Header is mounted correctly

Footer is mounted correctly

Mobile CTA bar is mounted correctly

Global layout works across every route

Do not duplicate Header/Footer inside every page unnecessarily.

STEP 11 — RESPONSIVE DESIGN

After all routes work, perform a responsive pass.

Test:

Desktop 1920px

Desktop 1440px

Tablet 768px

Mobile 390px

Especially check:

No horizontal overflow

Header/mobile menu

Buttons

Pricing tables/cards

Estimate form

Service cards

Images

Typography

Footer

Sticky mobile CTA

The mobile experience is extremely important because Google Ads traffic may primarily come from mobile.

DESIGN DIRECTION

Keep the existing Namma Laundry visual identity.

Brand:

Bottle Green + Gold + Ivory/White

Style:

Premium

Clean

Elegant

Trustworthy

Modern

Local

Simple

Professional

Do NOT turn this into a large corporate website.

Do NOT add excessive animations.

Do NOT introduce random colours.

Do NOT replace the existing design system.

IMPORTANT DEVELOPMENT RULES

Work with the existing repository.

Reuse existing components.

Reuse existing data.

Reuse existing design tokens.

Do not duplicate data.

Do not remove completed work.

Do not change the project's architecture unnecessarily.

Do not install unnecessary packages.

Do not use mock data when real existing data is available.

Do not hide or suppress TypeScript errors.

Do not leave TODO placeholders for required pages.

Do not stop after fixing only the first error.

FINAL REQUIREMENT

Before finishing:

Run typecheck/build.

Fix every build error.

Check every required route.

Check desktop and mobile responsiveness.

Confirm there is no horizontal overflow.

Confirm all navigation links work.

Confirm all service $slug pages work.

Confirm all knowledge $slug pages work.

Confirm the estimate calculation works.

Confirm Header/Footer/CtaBar work globally.

Confirm no Lovable default branding/text remains.

Leave the repository in a fully buildable, working state.

Do not stop at analysis. Implement the changes in the existing GitHub project and verify the final build successfully.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/bb42c1f6-b980-4122-b6e3-7ce624023001).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
