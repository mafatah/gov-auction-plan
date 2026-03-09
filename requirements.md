# Ministry of Finance — Government Auction Tender Requirements

**Tender #**: 2025/4494
**Client**: Ministry of Finance, State of Qatar
**Vendor**: Ebdaa Digital Technology (Mzad Qatar)
**Contract**: 5 years
**Source PDF**: `final finance tender-2-5.pdf` (34 pages, Zoho Sign signed 2026-01-25)
**Implementation Timeline**: 40 working days from contract signing

---

## 1. Project Overview

White-label government auction platform built on top of MzadQatar's existing infrastructure. Dedicated section within MzadQatar app/website for Ministry of Finance and authorized government entities to sell/lease government assets via electronic public auctions.

**Key Architecture**: Synchronization (Sync) between MzadQatar platform and a dedicated Ministry of Finance section — real-time data sync, independent operations, shared user base (1M+ users).

---

## 2. Platform Components

### 2.1 Mobile App (iOS + Android)
- Native apps (Objective-C for iOS, Kotlin for Android)
- Arabic + English bilingual
- Synchronized with MzadQatar app via dedicated government auction section
- Must work on phones and tablets

### 2.2 Website (Browser)
- Responsive design (desktop, mobile, tablet)
- Arabic + English bilingual
- SEO-optimized
- Full bidding capability via browser
- Synchronized with mobile app

### 2.3 Admin Dashboard (Control Panel)
- Dedicated to Ministry of Finance and authorized government entities
- Full auction lifecycle management

---

## 3. Registration & Authentication

| Requirement | Detail |
|------------|--------|
| Registration method | Phone number + OTP (SMS verification) |
| Required at signup | Name, bidder type (individual/company) |
| KYC (ID upload) | Only required after winning an auction |
| GCC participation | Bidders from GCC countries can participate (toggleable per item) |
| Multiple accounts | Strictly prohibited — all accounts + deposits confiscated |

---

## 4. Auction Features & Services

### 4.1 Core Auction Features
| # | Feature | Details |
|---|---------|---------|
| 1 | **Auto-Extension** | If bid placed in last 10 minutes, timer extends 10 min (configurable). No max duration. |
| 2 | **Multiple Payment for Deposit** | Credit card, bank transfer, cash (per central bank rules), Apple Pay, Google Pay |
| 3 | **Auto-Bidding** | User sets max bid amount; system bids automatically on their behalf up to that limit |
| 4 | **Deposit Refund** | Request refund via app; track status in-app |
| 5 | **GCC Bidders** | Toggleable per item — allow/disallow GCC country bidders |
| 6 | **Delivery Service** | Available inside/outside Qatar; bidder pays shipping costs |
| 7 | **Charity Linking** | Integration with charity organizations for unsold items (Qatar Charity, Red Crescent) |
| 8 | **Re-listing Unsold Items** | Can re-list unsold items at later dates with optional discount badge |
| 9 | **Bidder Transparency** | Show username, last 4 digits of phone, bidder country, bid amount |
| 10 | **Committee Access** | Ministry committee can view all bids with full phone numbers and amounts |
| 11 | **Government API Integration** | APIs for linking with Ministry of Interior (vehicle transfer), other govt systems |
| 12 | **Payment Gateway** | Electronic payment for deposits via app |
| 13 | **Vehicle Parking** | Long-term parking for 100+ vehicles (standard + premium) for inspection |
| 14 | **Inspection Center** | Mzad Qatar's own inspection center for detailed vehicle condition reports |

### 4.2 Auction Management Services (Provided by Ebdaa)
1. Professional photography (standard, video, 360° technology)
2. Content writing and technical details for items
3. Technical reports and condition assessment via inspection center
4. Washing/cleaning of items (vehicles, machinery)
5. Transport and delivery to winning bidder (no storage included)
6. Assistance with government registration procedures (vehicle title transfer)
7. Customer service available 24/7 throughout the week
8. Dedicated account manager for government entity communication
9. Asset valuation/appraisal when requested
10. Payment collection from bidders and receipt issuance
11. Reports and notifications to government entities
12. Electronic payment gateway activation

---

## 5. Auction Lifecycle (3 Phases)

### Phase 1 — Before Auction
- Government entity submits auction request via system to Ministry committee
- Committee approves and sends to Mzad Qatar team
- Team coordinates: photography, content writing, washing, technical reports
- Items arranged at inspection locations for bidder access
- Terms & conditions prepared per entity requirements
- Files/photos sent to Ministry committee for valuation review
- After committee valuation, auction launch request sent to Mzad Qatar

### Phase 2 — During Auction
- Electronic auction goes live
- Marketing campaigns launched (coordinated with marketing team)
- Operations team sets start price, minimum bid increment, deposit amount (percentage)
- Marketing oversees campaign performance across platforms
- Operations handles customer inquiries and complaints via dedicated number
- Account manager sends notifications to government entity and Ministry committee
- Emergency communication channel available

### Phase 3 — After Auction
- Operations coordinates item handover and payment collection
- Accounts team collects purchase amounts, issues receipts
- If winner doesn't collect within 48 hours, internal rules apply
- Operations organizes delivery after payment
- Marketing reviews results, analytics, and recommendations for future auctions

---

## 6. Bidder Terms & Conditions

1. Phone registration required to participate and view items
2. Deposit payment required before bidding (system blocks bidding without deposit)
3. Participation = inspection waiver (as-is condition accepted)
4. Items sold as-is; no claims after auction award
5. Winner must collect within 72 hours of payment (max 10 days with daily penalty)
6. Cash payments over 50,000 QAR prohibited (bank transfer required per central bank law)
7. Deposit confiscated if winner fails to pay within 48 hours of notification
8. Technical reports are non-binding; bidder responsible for inspection
9. Deposit refund available if bidder doesn't win any items
10. Bidder must wait for entity approval if bid doesn't reach valuation price
11. Winner must fill owner details form and upload personal ID (KYC)
12. All costs (registration fees, shipping, storage, title transfer) borne by bidder

---

## 7. Dispute Resolution & Price Review

### 7.1 Dispute Mechanism (per Plan #7)
1. Mzad Qatar investigates bidder claims
2. Coordinates with government entity to verify claims
3. Submits recommendation to Ministry committee for approval/rejection

**Acceptable dispute cases:**
- Delayed delivery from government entity beyond announced timeline
- Significant condition difference between pre-auction and post-auction state

**Not accepted:** disputes after bidder has taken delivery of items

### 7.2 Price Review Recommendation (per Plan #5)
- For items unsold/unleased after multiple auction attempts
- Committee can accept or reject review recommendations
- Internal process with pre-agreed terms
- Designed to increase chances of selling items

---

## 8. Admin Dashboard Features

### 8.1 Admin Control Panel
- Account and permission management (IAM)
- Category and classification management (create, edit, show, hide)
- Item management (add, edit, delete, hide auction items)
- Reports and analytics (participants, winners, performance)
- Government entity request tracking
- Financial tracking (balances, transactions)
- Asset valuation before auction listing
- User management (block users from bidding)

### 8.2 Additional Dashboard Screens (from design review)
- **Workflow/Pipeline**: Auction approval pipeline with statuses (Draft → Inspection → Photography → Deposit → Approval → Published → Live → Completed)
- **Live Bids Monitoring**: Real-time auction monitoring with WebSocket
- **Financial Tracking**: Deposits collected, refunds pending, late payments, revenue
- **Government Entity Performance**: Per-entity analytics and KPIs
- **Reports**: Monthly, quarterly, annual PDF reports
- **Compliance Monitoring**: Adherence tracking and operations oversight
- **Asset Valuation Screen**: Government asset appraisal management
- **Invoice/Receipt Generation**: Create and manage invoices and receipts
- **Dispute Management**: Handle disputes and complaints
- **Price Review Recommendations**: Analysis and recommendations workflow

---

## 9. Mobile App Features (End User)

### 9.1 Core Features
- Easy-to-use interface (designed for non-technical users)
- Browse available auctions with full details
- Bid on items for sale or lease
- Pay deposit via multiple payment methods
- Receive notifications (new auctions, outbid alerts, auction end, winning)
- Personal account for tracking bid history
- Favorites/watchlist
- Track bid status with full transparency
- View item description, current price, minimum increment, time remaining, T&C

### 9.2 Additional Features (from tender + design)
- **Auto-Bidding UI**: Set maximum bid amount
- **GCC Bidder Participation**: Register with GCC phone numbers
- **Share Auction Link**: Share via WhatsApp, Twitter, Facebook, copy link
- **Q&A Per Item**: Ask questions about specific auction items
- **Chat Channel**: Support chat per item (Intercom-style)
- **Terms & Conditions Page**: Dedicated T&C display with acceptance
- **FAQ Page**: Common questions and answers
- **Deposit Payment Flow**: Pay insurance before bidding
- **Deposit Refund Request**: Request and track refund status
- **KYC/Owner Form**: Upload ID and owner details after winning
- **Winner Payment Flow**: Complete purchase with multiple payment methods
- **Language Toggle**: Arabic/English switch
- **360° Image Viewer**: Interactive product visualization
- **Coming Auctions Bar**: Upcoming auction countdown display
- **Floating Help Button**: Intercom-style support access
- **Bidder Number Masking**: Show only last 3-4 digits (****XXX) with country flag

---

## 10. Website Features

### 10.1 Pages
- Home (hero, categories, active/coming auctions, how it works, stats, government entities)
- Auction Listing (filters, sorting, search)
- Auction Detail (images, specs, bid history, Q&A, share, terms, inspection location)
- Login (phone + OTP)
- Registration (phone, name, bidder type)
- User Account/Dashboard
- FAQ
- Deposit Refund Request
- Payment Methods
- Terms & Conditions
- About the Platform

### 10.2 Technical Requirements
- Responsive design (all devices)
- Arabic + English
- SEO optimized
- Full bidding via browser
- Synchronized with mobile app
- Ministry branding (logo, colors)

---

## 11. Technical & Security Requirements

### 11.1 Security
- OWASP best practices
- IAM (Identity and Access Management)
- Firewall protection
- Network monitoring for suspicious activity
- Data governance (prevent unauthorized access)
- Data encryption (at rest and in transit)
- Qatar Data Privacy Law compliance (Law No. 13 of 2016)
- Fraud detection for payment operations
- DLP (Data Loss Prevention)
- Periodic security certificates from third-party auditors

### 11.2 Infrastructure
- APIs for government system integration (Ministry of Interior for vehicle transfer)
- Cloud hosting: Google Cloud / Huawei Cloud
- Auto-backup for data protection and disaster recovery
- Scalable architecture
- MySQL database
- Native mobile development (iOS + Android)
- Programming languages: Angular, Node.js (and others)
- WebSocket for real-time bidirectional communication (live auctions)

---

## 12. Marketing (Provided by Ebdaa)

### Channels
- Instagram, TikTok, Facebook, Snapchat, X (Twitter)
- In-app promoted ads (banners, full-screen)
- Influencer marketing
- Direct marketing (SMS, push notifications)
- SEO optimization
- Email campaigns (per Law 13/2016)
- Traditional media (newspaper ads for auction announcements)
- Marketing automation (WebEngage)
- AI recommendation engines
- 360° product photography
- Customer experience videos (UGC)

### Reporting (Quarterly)
- UGC report, platform performance, ROAS, competitive analysis, optimization strategy

---

## 13. Support, Training & Maintenance

| Service | Frequency | Owner |
|---------|-----------|-------|
| Monthly performance & security check | Monthly (12/year) | Maintenance team |
| Systems & servers check | Monthly | Maintenance team |
| Maintenance per reports | Every 2 months (6/year) | Maintenance team |
| Security updates | As needed (immediate) | Dev team |
| Employee training | As needed | Project manager |
| Bug fixes | As needed per reports | Maintenance team |
| KPI-based improvements | Every 2 months | Dev team |
| User feedback collection | Periodic | Project manager |
| Feature additions/UI changes | As needed | Dev team |
| Modification requests | Via email/account manager | Project manager |
| Documentation & archiving | Continuous | Business dev team |
| Monthly performance reports | Monthly | Operations team |

### Emergency Response SLA
| Priority | Case | Response Time | Channel |
|----------|------|---------------|---------|
| P1 | Security breach | 15 min | Hotline / Account manager |
| P1 | System failure | 30 min | Hotline / Account manager |
| P1 | App performance failure | 30 min | Hotline / Account manager |
| P2 | Modification/improvement request | 1 hour (business hours) | Account manager |
| P2 | User reports | 2 hours | Customer service |
| P3 | Government entity communication | 1 hour | Account manager |
| P3 | IT incidents | 2 hours | Customer service + Account manager |
| P3 | Minor technical reports | 4 hours | Customer service / Email |

---

## 14. Timeline (from contract date, estimated 60 days)

| Phase | Task | Duration |
|-------|------|----------|
| Planning | Define objectives, requirements, schedule | 2 days |
| Design | Update app interface per brand guidelines | 5 days |
| Design | Create wireframes and website design | 7 days |
| Review | Design review and feedback | 3 days |
| Development | Customize app functions per new requirements | 15 days |
| Development | Compatibility testing (iOS + Android) | 5 days |
| Development | Website update (frontend + backend) | 20 days |
| QA | Comprehensive testing (app + website) | 10 days |
| Launch Prep | Final preparation and training | 10 days |
| Launch | Go-live and continuous monitoring | 5 days |

---

## 15. Pricing Model

| Type | Rate |
|------|------|
| **Sale auction** | 3% of total auction value (fixed percentage) |
| **Lease/rental auction** | 500 QAR per lease auction (fixed amount) |

---

## 16. Equipment & Software (Available)

### Hardware
- 3D Camera, Canon SLR Camera, Sony Alpha 7
- Samsung/Lenovo tablets (for field inspectors)
- 20+ laptops (various: Lenovo, HP, ASUS)
- iPhone 15 Pro Max (marketing team)
- HP LaserJet printer, Lenovo monitor

### Software/Services
Amazon, Cloudflare, CometChat, Figma, GoDaddy, Google Cloud / Huawei Cloud, Hubstaff, Jira, New Relic, ServerPilot, Sketch, Shutterstock, Twilio, Envato, Twitter/X, ChatGPT, Testimo, Apple Search Ads, Zoho (Accounting + CRM + Desk), WebEngage

---

## 17. Admin Actions on Live Auctions with Active Bids

This section defines the complete flow for every admin action that can happen while an auction has active bids. It maps what the tender and T&C already cover, and fills the gaps with the recommended implementation logic.

---

### 17.1 Cancel Auction with Active Bids (إلغاء المزاد)

**Tender/T&C coverage**: Section 7 of T&C states: *"Government entity reserves the right to cancel, postpone, or withdraw any item at any time before the award, without providing reasons and without bearing any liability. In case of cancellation, the deposit is fully refunded to all bidders."*

**Recommended flow**:

```
Admin clicks "إلغاء المزاد" on live auction
  │
  ├─ 1. System shows confirmation dialog:
  │     "This auction has [X] active bidders and [Y] bids. Are you sure?"
  │     → Admin must select cancellation reason from dropdown:
  │       - Government entity request
  │       - Committee decision
  │       - Technical issue
  │       - Legal/compliance issue
  │       - Item withdrawn by entity
  │     → Admin can add free-text notes
  │
  ├─ 2. Requires 2-factor confirmation:
  │     → If auction value > 100,000 QAR → requires committee member approval
  │     → If auction value ≤ 100,000 QAR → admin can cancel directly
  │
  ├─ 3. On confirm:
  │     a. WebSocket broadcasts "AUCTION_CANCELLED" to all connected clients
  │     b. Auction status changes to "Cancelled" (not deletable from records)
  │     c. All active auto-bids are deactivated
  │     d. Timer stops immediately
  │     e. No new bids accepted
  │
  ├─ 4. Deposit handling (automatic):
  │     a. All deposits marked for refund
  │     b. Refund processed within 3-5 business days (per T&C 3.2)
  │     c. Refund goes back to original payment method
  │
  ├─ 5. Notifications (immediate):
  │     a. Push notification to all bidders: "Auction [name] has been cancelled"
  │     b. SMS to all bidders who placed bids
  │     c. Email to government entity contact
  │     d. In-app notification with reason (generic, not internal reason)
  │
  └─ 6. Audit log:
        → Cancellation reason, admin name, timestamp, bid count at cancellation
        → All bid history preserved for compliance
```

---

### 17.2 Pause Live Auction (إيقاف مؤقت)

**Tender/T&C coverage**: Not explicitly defined in tender. Dashboard design shows "إيقاف مؤقت" button but no behavior specification.

**Recommended flow**:

```
Admin clicks "إيقاف مؤقت" on live auction
  │
  ├─ 1. System shows pause dialog:
  │     → Admin must select reason:
  │       - Technical investigation
  │       - Suspected fraud / bid manipulation
  │       - Government entity request
  │       - System maintenance
  │     → Estimated pause duration (optional)
  │
  ├─ 2. On confirm:
  │     a. Auction status → "Paused" (new status between Live and Completed)
  │     b. Countdown timer FREEZES at exact remaining time
  │     c. New bids BLOCKED (server rejects with "auction paused" error)
  │     d. Auto-bids FROZEN (not deactivated — will resume)
  │     e. WebSocket broadcasts "AUCTION_PAUSED" with remaining time snapshot
  │
  ├─ 3. User experience during pause:
  │     a. Auction page shows "⏸ Auction temporarily paused" banner
  │     b. Bid button disabled with "Auction paused" tooltip
  │     c. Timer shows frozen time with pause indicator
  │     d. Users can still view item details, bid history, Q&A
  │     e. Auto-extension rules suspended during pause
  │
  ├─ 4. Resume flow:
  │     → Admin clicks "استئناف" (Resume)
  │     → Timer resumes from exact frozen time
  │     → If remaining time < 30 minutes at resume → auto-extend by 30 min
  │       (to give bidders fair notice that auction is back)
  │     → WebSocket broadcasts "AUCTION_RESUMED" with new end time
  │     → Push notification to all bidders: "Auction [name] has resumed"
  │     → Auto-bids reactivated
  │
  ├─ 5. Auto-cancel on extended pause:
  │     → If paused for > 24 hours without resume → system flags for review
  │     → If paused for > 72 hours → auto-escalate to committee
  │
  └─ 6. Audit log:
        → Pause reason, duration, admin name, resume admin, timestamps
```

---

### 17.3 Extend Live Auction (تمديد المدة)

**Tender/T&C coverage**: Auto-extension is covered (T&C 4.2: bid in last minutes → 5 min extension). Manual extension by admin is shown in dashboard design but not defined in tender.

**Recommended flow**:

```
A. AUTOMATIC EXTENSION (already covered by tender):
  │
  ├─ Bid received within last X minutes (configurable, default 5 min per T&C)
  ├─ Timer extends by X minutes from the bid timestamp
  ├─ No maximum cap on number of extensions
  ├─ WebSocket broadcasts updated end time to all clients
  └─ Auto-bid triggers count as bids for extension purposes

B. MANUAL EXTENSION (admin action):
  │
  ├─ 1. Admin clicks "تمديد المدة"
  │     → Select extension duration: 1 hour / 6 hours / 12 hours / 24 hours / custom
  │     → Reason: Low activity / Government entity request / Marketing extension / Other
  │
  ├─ 2. On confirm:
  │     a. End time recalculated
  │     b. WebSocket broadcasts "AUCTION_EXTENDED" with new end time
  │     c. Auto-extension eligibility window resets to new end time
  │
  ├─ 3. Notifications:
  │     a. Push notification to all bidders and watchers
  │     b. Auction detail page shows "Extended" badge with new end time
  │
  └─ 4. Restrictions:
        → Cannot extend after auction has been awarded (completed)
        → Cannot extend a paused auction (must resume first)
        → Extension must be at least 1 hour (no micro-extensions)
        → Audit log records: old end time, new end time, reason, admin
```

---

### 17.4 Winner Forfeits / Doesn't Pay (الفائز لا يدفع)

**Tender/T&C coverage**: Tender 6 #7 says deposit confiscated after 48 hours. T&C 5 says 7 business days with 1% daily penalty. Neither specifies what happens to the auction item after forfeiture.

**Recommended flow**:

```
Auction ends → Winner #1 notified
  │
  ├─ Day 1-7: Payment window (7 business days per T&C 5)
  │     → Daily reminder notifications (push + SMS)
  │     → 1% daily penalty applied after Day 1
  │
  ├─ Day 7 (deadline passed, no payment):
  │     a. Winner #1's deposit CONFISCATED (per T&C 3.3)
  │     b. Winner #1 flagged in system ("forfeited auction")
  │     c. Winner #1 blocked from next 3 auctions (configurable)
  │
  ├─ SECOND BIDDER OFFER (not in tender — recommended addition):
  │     a. System automatically offers to Bidder #2 (second highest)
  │     b. Bidder #2 gets notification: "You have been offered [item] at your bid price [X]"
  │     c. Bidder #2 has 48 hours to accept or decline
  │     d. If Bidder #2 accepts → same payment/KYC flow as winner
  │     e. If Bidder #2 declines → offer cascades to Bidder #3
  │     f. Maximum cascade: top 3 bidders only
  │     g. Bidder's original deposit remains locked until they accept/decline
  │
  ├─ If all top 3 decline or no second bidder:
  │     a. Auction marked as "Unsold — Winner Forfeited"
  │     b. Item enters Price Review workflow (Section 7.2 of tender)
  │     c. Committee decides: re-list / lower price / charity / hold
  │
  └─ Financial handling:
        → Confiscated deposit split: Mzad Qatar operational costs + government entity
        → Revenue from forfeiture logged separately in financial reports
        → If second bidder wins at lower price → difference is a loss, not charged to anyone
```

---

### 17.5 Entity Rejects Highest Bid (Below Valuation)

**Tender/T&C coverage**: Tender 6 #10 says bidder must wait for entity approval if bid doesn't reach valuation. T&C 4.3 says entity can reject if below minimum. Price Review screen offers: extend duration, lower opening price, cancel and re-list, accept current price.

**Recommended flow**:

```
Auction ends → Highest bid = 95,000 QAR but valuation = 150,000 QAR
  │
  ├─ 1. Auction status → "Pending Entity Approval" (not "Completed")
  │     → Timer stopped, no new bids
  │     → All bidders notified: "Auction ended. Awaiting entity decision."
  │     → Deposits remain locked
  │
  ├─ 2. Entity / Committee reviews (via Price Review screen):
  │     → System shows: valuation, highest bid, gap %, bidder count, activity level
  │     → Options:
  │       a. ACCEPT current price → proceed to winner flow normally
  │       b. EXTEND auction → re-open with more time, all bids preserved
  │       c. LOWER opening price → cancel and re-list with lower valuation
  │       d. REJECT and re-list → full re-auction at later date
  │
  ├─ 3. If accepted:
  │     → Normal winner notification flow
  │     → Losing bidders' deposits released
  │
  ├─ 4. If extended:
  │     → Auction re-opens from current highest bid
  │     → All existing bids and auto-bids remain active
  │     → New extension period (e.g., 3 more days)
  │     → All bidders notified: "Auction extended for [duration]"
  │
  ├─ 5. If rejected and re-listed:
  │     → All deposits refunded
  │     → All bidders notified: "Auction will be re-listed"
  │     → Item goes back to "Draft" in pipeline
  │
  └─ 6. Decision deadline:
        → Entity must decide within 5 business days of auction end
        → If no decision in 5 days → system auto-escalates to committee
        → If no decision in 10 days → highest bid is auto-accepted
```

---

### 17.6 Auto-Bidding Conflicts

**Tender/T&C coverage**: Tender 4.1 #3 says system bids automatically up to user's max. FAQ says system bids by minimum increment. No tie-breaking logic specified.

**Recommended flow**:

```
Scenario: Bidder A sets auto-bid max = 200,000 QAR
          Bidder B sets auto-bid max = 200,000 QAR
          Current price = 150,000 QAR
          Minimum increment = 5,000 QAR

Flow:
  ├─ Normal auto-bid escalation:
  │     → Bidder A auto-bids 155,000
  │     → Bidder B auto-bids 160,000
  │     → Bidder A auto-bids 165,000
  │     → ... continues until one hits their max
  │
  ├─ Tie-breaking (both reach 200,000):
  │     → FIRST-TO-SET wins — whoever set 200,000 as their max first
  │     → Server timestamp of auto-bid creation determines priority
  │     → Losing auto-bidder notified: "Your max has been matched. Increase to continue."
  │
  ├─ Auto-bid + Manual bid conflict:
  │     → Manual bid always processed first in the same tick
  │     → Auto-bid responds on next tick (server-side queue)
  │
  └─ Notifications:
        → Each auto-bid trigger sends push notification to the bidder
        → "Auto-bid placed: [amount]. [X] remaining before your max."
        → When max reached: "Your auto-bid limit reached at [amount]. Bid manually to continue."
```

---

### 17.7 Simultaneous Bids (Race Condition)

**Tender/T&C coverage**: WebSocket mentioned (Section 11.2) but no race condition handling specified.

**Recommended flow**:

```
Two bids arrive at "same time":
  │
  ├─ Server-side queue (mandatory):
  │     → All bids enter a single-threaded FIFO queue per auction
  │     → Server assigns sequential bid_number (atomic increment)
  │     → Bid with lower bid_number wins the slot
  │
  ├─ Validation on each bid:
  │     → Must be > current highest + minimum increment AT TIME OF PROCESSING
  │     → If bid was valid when sent but invalid when processed (someone beat them):
  │       → Bid REJECTED with "Outbid" response
  │       → WebSocket sends updated price to the losing bidder instantly
  │       → No penalty — bidder can re-bid
  │
  ├─ Optimistic locking:
  │     → Client sends: { amount, expected_current_price }
  │     → Server checks expected_current_price matches actual
  │     → If mismatch → reject with current price, client refreshes and re-bids
  │
  └─ Transparency:
        → Each bid shows server-assigned timestamp (not client timestamp)
        → Bid history shows exact order of processing
        → Committee can audit full bid queue log
```

---

### 17.8 Edit Live Auction (تعديل)

**Tender/T&C coverage**: Dashboard design shows "تعديل" (Edit) button on live auction. Not defined what can be edited while live.

**Recommended flow**:

```
What CAN be edited during a live auction:
  ├─ Description text / item details (typo fixes)
  ├─ Add more photos or 360° images
  ├─ Q&A answers
  ├─ Inspection location / schedule
  ├─ T&C clarifications (append only, no removals)

What CANNOT be edited during a live auction:
  ├─ Starting price
  ├─ Minimum bid increment
  ├─ Deposit amount
  ├─ Auto-extension settings (must cancel and re-list)
  ├─ GCC participation toggle
  ├─ Item category / classification

On every edit:
  ├─ System logs: what changed, old value, new value, admin, timestamp
  ├─ If material change (description, photos): all bidders notified
  └─ Change visible in audit trail for committee review
```

---

### 17.9 Dispute: Auto-Extension Didn't Trigger

**Tender/T&C coverage**: Dispute screen (DSP-001) shows exactly this case: *"I object to the auction result because a bid was accepted in the last 30 seconds and the auction was not automatically extended as stated in the terms."*

**Recommended flow**:

```
Bidder files dispute claiming auto-extension failed
  │
  ├─ 1. System auto-generates evidence report:
  │     → Exact timestamp of last bid
  │     → Auction end time
  │     → Was bid within auto-extension window? (yes/no)
  │     → Did auto-extension trigger? (yes/no + server log)
  │     → WebSocket delivery confirmation logs
  │
  ├─ 2. If system confirms auto-extension DID fail (bug):
  │     → Committee options:
  │       a. Re-open auction from the disputed bid point
  │       b. Accept the last valid bid before the failure
  │       c. Full re-auction
  │     → All deposits remain locked until resolution
  │     → Mzad Qatar responsible for technical fix + report
  │
  ├─ 3. If system confirms auto-extension DID trigger correctly:
  │     → Show evidence to bidder (timestamps, logs)
  │     → Committee rejects dispute
  │     → Bidder can escalate to higher committee (T&C 9)
  │
  └─ 4. Resolution deadline: 7 business days from dispute filing
```

---

### Summary: Coverage Matrix

| # | Scenario | Tender | T&C (Design) | Dashboard UI | Full Flow Defined |
|---|----------|--------|-------------|-------------|-------------------|
| 1 | Cancel auction with active bids | Partial (lifecycle) | **Yes** (Section 7) | **Yes** (button) | **Section 17.1 above** |
| 2 | Pause live auction | No | No | **Yes** (button) | **Section 17.2 above** |
| 3 | Extend live auction (manual) | No | Auto only (4.2) | **Yes** (button) | **Section 17.3 above** |
| 4 | Winner doesn't pay | **Yes** (6 #7) | **Yes** (3.3, 5) | No | **Section 17.4 above** |
| 5 | Entity rejects bid (below valuation) | **Yes** (6 #10) | **Yes** (4.3) | **Yes** (Price Review) | **Section 17.5 above** |
| 6 | Auto-bid tie / conflicts | Partial (4.1 #3) | FAQ only | No | **Section 17.6 above** |
| 7 | Simultaneous bids (race condition) | No | No | No | **Section 17.7 above** |
| 8 | Edit while live | No | No | **Yes** (button) | **Section 17.8 above** |
| 9 | Auto-extension dispute | **Yes** (7.1) | **Yes** (9) | **Yes** (DSP-001) | **Section 17.9 above** |

---

## 18. Key Team Members

| Role | Name | Experience |
|------|------|-----------|
| Project Manager | Mostafa Mohamed | 1.5 years |
| Operations Manager | Ameed Atta | 13 years |
| Customer Service | Aya Zeitoun | 4 years |
| Operations Coordinator | Ibrahim Ali | 3 years |
| Technical Inspector | Abdulghafour Shajdani | 3 years |
| Marketing Director | Mei Mohamed | 10 years |
| Marketing Specialist | Nasser Aloush | 6 years |
| Photographer/Editor | Dibu Vilaban | 3 years |
| Design Director | Victoria Babakina | 8 years |
| Team Lead (Marketing) | Ahmed Ehab | 2 years |
| Marketing Specialist | Ali Mabkhouta | 5 years |
| Product Manager | Mohamed Dawood | 7 years |
| Auction Scheduler | Mazen Mohamed | 1 year |
| Finance Director | Abdulbasit Falabil | 11 years |
| Procurement/Accounting | Ticson Thomas | 10 years |
| HR Manager | Fazrath Rahmath | 9 years |
| Tech Director | Abdullah Sanallah | 14 years |
| Mobile Team Lead | Tejas Riyai | 12 years |
| Backend Team Lead | Tigran Mansourian | 12 years |
| iOS Developer | Arun Mahajan | 9 years |
| Backend Developer | Ronen Kholid Zahanian | 8 years |
| Data Analyst | Ahmed Hesham | 8 years |
| QA Lead | Ahmed Syed | 15 years |
| QA Specialist | Mazen Farghani | 7 years |
| QA Specialist | Mostafa Eid | 8 years |
