# Catering Website Feature Requirements Document

## 1. Purpose & Business Goals

### Primary Goals
- Drive direct catering orders through the restaurant’s website.
- Reduce reliance on third-party catering platforms (e.g., Easy Cater).
- Increase profitability by capturing higher-margin catering sales.
- Capture and retain customer data for long-term relationships.
- Boost sales on slow days (Mondays & Tuesdays).

### Key Business Insights
- Catering orders are ~2× more profitable than equivalent single orders.
- ~65% of catering orders are corporate.
- Corporate catering demand peaks on Mondays and Tuesdays.
- Third-party platforms take 30%+ commission and own customer data.

## 2. Core Catering Ordering System (Website)

### 2.1 Direct Online Catering Ordering
The website must support end-to-end catering orders without redirecting users off-site.

**Requirements**
- Dedicated catering ordering flow on the restaurant website.
- Orders placed directly with the restaurant.
- Customer accounts tied to catering orders.

### 2.2 Headcount / Per-Person Ordering
Catering orders should be selectable by number of people, not just item quantity.

**Requirements**
- Input for headcount (e.g., “Feeds 10–12 people”).
- Automatic quantity calculation based on headcount.
- Ability to adjust headcount dynamically.
- Clear per-person pricing visibility.

### 2.3 Catering Menu Configuration
Menus must be optimized specifically for catering use cases.

**Requirements**
- Catering-specific dishes and tray sizes.
- Large format items (e.g., large trays, bulk salads).
- Pre-configured catering packages.
- Ability to highlight popular corporate catering items.

### 2.4 Catering Delivery Integration
Delivery must be as easy as third-party platforms while remaining first-party.

**Requirements**
- Integration with third-party delivery networks.
- Delivery scheduling for future dates/times.
- Delivery options selectable within the website checkout.
- Delivery availability by location.

## 3. Loyalty & Incentive System

### 3.1 Catering Loyalty Program
A loyalty system specifically designed for corporate administrators and repeat catering buyers.

**Requirements**
- User accounts with login functionality.
- Loyalty points earned on catering orders.
- Points redeemable for free food.
- Loyalty rewards tied to ordering directly on the website.

### 3.2 Administrator Incentive Support
The system must support workflows that encourage office admins to order directly.

**Requirements**
- Ability to associate loyalty accounts with specific users/companies.
- Tracking repeat orders per account.
- Support for promotional credits or free items.
- Loyalty system positioned as a replacement for third-party incentives.

## 4. SEO & Catering Discovery

### 4.1 Catering-Focused SEO Architecture
The website must be structured to rank for catering-intent search queries.

**Requirements**
- Catering-specific landing pages.
- Dish-level SEO pages (e.g., “large tray of salad”).
- Location-based catering SEO (city / neighborhood targeting).
- Structured data optimized for catering searches.

### 4.2 Catering Product Pages
Each catering item should function as a discoverable search asset.

**Requirements**
- Individual indexable pages for catering dishes.
- SEO-friendly titles and descriptions.
- Clear catering intent language.
- Headcount and use-case visibility (meetings, offices, events).

## 5. Promotion & Operational Enablement (Website Support)

### 5.1 Corporate Ordering Enablement
The website must support a workflow that aligns with in-person promotion.

**Requirements**
- Simple ordering experience for repeat corporate buyers.
- Fast re-ordering from past orders.
- Account-based ordering (not guest-only).
- Clear messaging that encourages ordering through the website.

### 5.2 Support for Manager-Driven Promotion
While promotion is offline, the website must reinforce it.

**Requirements**
- Easy onboarding for new corporate users.
- Clear explanation of loyalty benefits.
- Website positioned as “preferred ordering channel”.
- Ability to handle increased catering volume smoothly.

## 6. Performance & Scalability

### 6.1 Multi-Location Support
The system must support restaurants with multiple locations.

**Requirements**
- Location-specific menus and availability.
- Catering orders routed to the correct location.
- Scalable architecture for multiple concepts or stores.

### 6.2 Reliability on High-Value Orders
Catering orders are large and time-sensitive.

**Requirements**
- High checkout reliability.
- Clear order confirmation and visibility.
- Accurate fulfillment data for staff.

## 7. Strategic Outcomes Supported by the Website
- Capture 100% of catering revenue instead of losing 30%+.
- Own corporate customer relationships and data.
- Make ordering easier than third-party platforms.
- Reward decision-makers directly.
- Drive catering volume on traditionally slow days.

## 8. User Types & Primary Use Cases

### 8.1 User Types
- Corporate office administrators ordering recurring meetings.
- Department managers ordering ad-hoc lunches.
- Event planners ordering large gatherings.
- Restaurant staff/ops fulfilling and coordinating delivery.

### 8.2 Primary Use Cases
- Schedule a catering order for a future date and time.
- Build an order by headcount with per-person pricing.
- Reorder a previous corporate order in a few clicks.
- Apply loyalty points or promotional credits at checkout.
- Route the order to the correct location with fulfillment notes.

## 9. End-to-End User Flow (First-Party)

1. **Discover catering** (SEO page, menu landing page, or “Catering” navigation).
2. **Select location** (or auto-detect) and verify delivery/pickup availability.
3. **Choose headcount** to auto-build a package or adjust items per person.
4. **Customize items** (dietary preferences, add-ons, upgrades).
5. **Schedule delivery** (date/time windows) or select pickup.
6. **Sign in / create account** to apply loyalty and save preferences.
7. **Review & pay** with taxes, fees, gratuity, and delivery costs visible.
8. **Receive confirmation** with clear receipt, ETA, and contact information.
9. **Manage order** (edits, status updates, delivery tracking, invoices).

## 10. Functional Requirements (Detailed)

### 10.1 Location & Availability
- Default to nearest location with manual override.
- Block ordering outside operational hours or lead-time windows.
- Holiday and blackout-date controls for catering.

### 10.2 Menu & Package Logic
- Item-level “feeds X people” metadata.
- Packages defined by headcount tiers (e.g., 10–12, 20–24).
- Rules for substitutions and dietary swaps.
- Admin-facing availability toggles per location.

### 10.3 Headcount Pricing Engine
- Per-person price ranges with minimum headcount rules.
- Auto-scale quantities by headcount with manual adjustments.
- Real-time price updates when headcount changes.

### 10.4 Checkout & Payment
- Multiple payment options: card, corporate card vault, invoice (optional).
- Tip/gratuity guidance for catering delivery.
- Purchase order fields for corporate accounts.
- Taxes/fees broken out by location.

### 10.5 Account & Loyalty
- Corporate account profiles with multiple users.
- Points balance visibility and redemption rules.
- Promotional credits with expiry and usage limits.
- Saved addresses, delivery instructions, and reorder favorites.

### 10.6 Order Management
- Order confirmation email + SMS with order details.
- Staff view with printable prep sheets and packaging notes.
- Status updates (received, in prep, out for delivery, delivered).
- Order change policy enforcement (cutoffs).

### 10.7 Delivery Integration
- Integration with third-party delivery networks or internal drivers.
- Delivery quote at checkout based on location and window.
- Real-time driver tracking link (where supported).

## 11. Content & SEO Requirements

### 11.1 Site Architecture
- `/catering` landing page with conversion-focused content.
- `/catering/menu` with headcount filtering and package highlights.
- `/catering/items/<slug>` for item-level SEO.
- `/catering/<city>` or `/catering/<neighborhood>` pages.

### 11.2 Metadata & Structured Data
- Schema.org for `Restaurant`, `FoodEstablishment`, and `Menu`.
- Item pages include headcount, occasion, and delivery keywords.
- Canonicals for duplicate items across locations.

## 12. Analytics & KPIs

### 12.1 Core KPIs
- Catering conversion rate (landing → checkout).
- Average order value (AOV) and headcount.
- Repeat rate by corporate account.
- Direct-order share vs third-party platforms.

### 12.2 Event Tracking
- Headcount changes and package selection.
- Reorder clicks and conversions.
- Loyalty redemption usage.
- Delivery option selection.

## 13. Operational Readiness

### 13.1 Staff Enablement
- Prep timelines and lead times per package.
- Auto-generated packing lists.
- Location routing for multi-store operations.

### 13.2 Reliability Controls
- Order validation checks (lead time, minimums).
- Fallback flows for delivery API outages.
- Clear customer support escalation path.

## 14. Technical & Data Model (High-Level)

### 14.1 Core Entities
- **Location**: hours, catering availability, menu overrides.
- **CateringItem**: headcount range, pricing, package flags.
- **Package**: includes multiple items, headcount tiers.
- **Order**: line items, headcount, delivery schedule, payments.
- **Account**: company profiles, users, points, credits.

### 14.2 Integrations
- Payment processor (tokenized cards, corporate billing).
- Delivery provider APIs.
- CRM/Email for follow-up and loyalty campaigns.

## 15. Rollout & Milestones (Suggested)

### Phase 1: MVP Direct Ordering
- Catering landing + menu pages.
- Headcount-based ordering and checkout.
- Basic account creation and order confirmation.

### Phase 2: Loyalty & Corporate Accounts
- Points accumulation and redemption.
- Corporate accounts with reorder workflows.

### Phase 3: Delivery & SEO Expansion
- Delivery network integrations.
- SEO expansion across locations and items.
