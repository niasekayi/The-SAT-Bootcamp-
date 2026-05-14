# SAT Bootcamp Website - Sitemap & Design Direction

## Website Structure

```
SAT Bootcamp (Root)
├── index.html (Home Page)
├── program.html (The Program)
├── schedule.html (Schedule & Dates)
├── apply.html (Apply & Pricing)
└── assets/
    ├── css/
    │   └── styles.css (Main stylesheet)
    └── images/
        └── (placeholder for botanical graphics, logos, icons)
```

---

## Page Hierarchy & Navigation

### Primary Navigation (Header)
- **Logo**: SAT Bootcamp (links to home)
- **Menu Items**: 
  - Home
  - The Program
  - Schedule
  - Apply

All pages include this consistent header for seamless navigation.

---

## Detailed Page Breakdown

### 1. **Home Page** (index.html)
**Purpose**: Hook & Convert  
**Key Sections**:
- Hero with value proposition
- Problem/Solution cards (3 failures of traditional prep)
- Our Solution (6 differentiators)
- Founder bio with mission statement
- Final CTA: "Sign Up for Strategy Reveal"

**Copy Tone**: Conversational, confident, results-focused  
**Visuals**: Fine-line icons for each card (X for failure, clock for time, dollar sign for cost)  
**CTA**: Primary button to Info Meeting Form

---

### 2. **The Program Page** (program.html)
**Purpose**: Deep Dive & Education  
**Key Sections**:
- Boutique Model explanation
- 5 Squads breakdown
- 3 Curriculum Pillars
- Weekly Rhythm
- The "Doer" Contract (three-way commitment)
- FAQs

**Copy Tone**: Educational, transparent, empowering  
**Visuals**: Squad icons, pillar graphics, timeline visuals  
**Color Coding**: Use sage for pillars, terracotta for contract sections

---

### 3. **Schedule Page** (schedule.html)
**Purpose**: Logistics & Clarity  
**Key Sections**:
- 3 Sessions overview (timeline cards)
- Weekly schedule table
- Squad meeting times
- Registration deadlines (bolded May 20 for Session 1)
- Next steps CTA

**Copy Tone**: Clear, organized, deadline-focused  
**Visuals**: Color-coded session cards, schedule table with time slots  
**Visual Direction**: Use striped backgrounds or light borders to differentiate sections

---

### 4. **Apply Page** (apply.html)
**Purpose**: Conversion & Enrollment  
**Key Sections**:
- Pricing cards (3 options: Session 1, Full Summer, Session 3)
- 3 Steps to Join
- Requirements breakdown
- FAQs
- Final CTA section

**Copy Tone**: Action-oriented, clear, reassuring  
**Visuals**: Featured pricing card (Full Summer) with highlighted border  
**Button Strategy**: 
  - Primary button: "Enroll Now" (links to Application Form)
  - Secondary buttons: "Sign Up for Strategy Reveal"

---

## Color Palette & Design Direction

### Core Colors
```
--dusty-rose:        #D4A5A5 (Accent, warm)
--terracotta:        #C97755 (Primary CTA, headlines)
--sage:              #9CAF88 (Secondary, trust)
--off-white:         #F5F3F0 (Main background)
--deep-charcoal:     #3A3A3A (Text, dark)
--soft-taupe:        #E8DDD6 (Section backgrounds)
--cream:             #FBF9F6 (Cards, softer background)
```

### Design Aesthetic: Pink Boho + Earthy
- **Typography**: Playfair Display (serif) for headlines = elegance; Inter (sans-serif) for body = clarity
- **Spacing**: Generous padding, breathing room between sections
- **Borders**: Subtle left-border accents on cards (4px solid sage/terracotta)
- **Shadows**: Soft, minimal shadows (0 2px 8px rgba(0,0,0,0.05))
- **Radius**: Rounded corners (10-12px) for soft, boutique feel

---

## Icon Recommendations (Fine-Line Style)

### Hero Section
- 📚 (Books) - Knowledge
- 👥 (People) - Community/Squads
- 🎯 (Target) - Results

### Program Page
- 📚 Knowledge Base Building
- 🤝 Collaborative Problem-Solving
- 🎯 Strategic Mastery
- 👥 Squad structure
- 📊 Data-driven

### Schedule Page
- 📅 Calendar/dates
- 🕐 Clock for noon start
- 🔄 Rotation/cycle

### Apply Page
- 💳 Payment
- 📝 Application
- ✓ Checkmarks for features

### Botanical Graphics
- Dividers: "✿ ✿ ✿" (leaf motifs between sections)
- Accent: Small line-drawn flowers in page corners
- Borders: Subtle floral patterns on section dividers (optional in CSS)

---

## Visual Direction by Section

### Header
- Sticky header with subtle shadow
- Logo in terracotta
- Nav links with underline animation on hover
- Background: cream (#FBF9F6)

### Hero Sections
- Large serif headline (Playfair Display, 3.5rem)
- Subheader in terracotta
- Centered layout with max-width container
- Optional: Subtle circular background shape (opacity: 0.2, sage)

### Cards
- Consistent left-border accent (4px)
- Soft shadow on hover
- Icon at top (large, 3rem, ~0.8 opacity)
- Title in serif (h3)
- Description in body text

### Section Backgrounds
- Alternating off-white and soft-taupe for visual rhythm
- Cream backgrounds for cards
- Gradient backgrounds for CTAs (e.g., terracotta to dusty-rose)

### Buttons
- **Primary**: Terracotta background, cream text, rounded (50px border-radius)
- **Secondary**: Sage background, cream text, rounded
- **Outline**: Transparent, terracotta border, terracotta text
- **Hover state**: Slight lift (translateY -2px), shadow increase

### Tables
- Header: sage background, cream text
- Alternating row backgrounds (off-white, soft-taupe)
- Hover state: light highlight

### Pricing Cards
- Featured card: Terracotta border-top (vs. sage for standard)
- Gradient background on featured card
- Checkmark indicators for features

---

## Responsive Design Breakpoints

- **Desktop**: 1200px max-width
- **Tablet**: 768px breakpoints (adjust font sizes, stack sections)
- **Mobile**: Single-column layout, nav adjustments, larger touch targets

---

## CTA Strategy & Link Targets

### Info Meeting Form Link
```
https://docs.google.com/forms/d/e/1FAIpQLScLRryzbgHCas5e8FGF_DjHe6bkrKm01z4n2JVBh6kXZiDFnA/viewform?usp=header
```
- Used on: Home, Program, Schedule pages
- Button text: "📅 Sign Up for Strategy Reveal"
- Target: _blank

### Application Form Link
```
https://docs.google.com/forms/d/e/1FAIpQLScLRryzbgHCas5e8FGF_DjHe6bkrKm01z4n2JVBh6kXZiDFnA/viewform?usp=header
```
- Used on: Apply page (primary), all pages as secondary
- Button text: "✏️ Official Application" or "Enroll Now"
- Target: _blank

### Internal Navigation
- Logo always links to index.html
- All nav links use relative paths (program.html, schedule.html, apply.html)

---

## Micro-Copy & Tone Guidelines

### Headlines
- Direct, benefit-focused ("Master the Digital SAT Logic")
- Use power words: Boutique, Near-Peer, Strategy, Results

### Subheadings
- Supporting statement, specific differentiation
- Example: "High-level strategy taught by a Howard University CS & Math student"

### Body Copy
- Conversational but professional
- Short paragraphs (2-3 sentences max)
- Active voice, present tense where possible
- Use bold for emphasis on key commitments/numbers

### CTAs
- Urgent but not pushy ("Ready to join?" vs "SIGN UP NOW!!!")
- Emoji where appropriate (📅, ✏️, 🎓)
- Clear action verb

---

## Layout Pattern: 20/10/20 Rule Applied to Web

While the 20/10/20 rule is for sessions, the website mirrors this pacing:
1. **Kickoff** (Hero): Hook with value prop + problem
2. **Content Depth**: Detailed sections (Program, Squad structure)
3. **Action**: Clear call-to-action buttons
4. **Trust-Building**: Founder bio, testimonials space (future)
5. **Close**: Final CTA with urgency (deadlines, limited spots)

---

## Future Enhancement Opportunities

1. **Testimonials Section**: Add on Home/Program pages (student success stories, score improvements)
2. **Video Hero**: Nia introducing the program (10-15 sec)
3. **Blog/Resources**: SAT tips, strategy articles (SEO benefit)
4. **Dynamic Quiz**: "Which Squad Are You?" → personalized recommendation
5. **Calendar Integration**: Embedded Google Calendar showing session times
6. **Interactive Pricing**: Slider to select sessions, real-time pricing update
7. **Live Chat**: Real-time support during peak hours

---

## Performance & Accessibility

- Semantic HTML5 structure
- Alt text for all images/icons
- Keyboard navigation support
- Color contrast ratios meet WCAG AA standards
- Mobile-first responsive design
- Fast load times (CSS is inline, minimal external dependencies)
- Google Fonts for typography (preconnect headers included)

---

## File Structure Summary

```
website/
├── index.html               (Home - 500+ lines)
├── program.html             (Program - 450+ lines)
├── schedule.html            (Schedule - 400+ lines)
├── apply.html               (Apply - 500+ lines)
├── assets/
│   ├── css/
│   │   └── styles.css       (Comprehensive stylesheet - 600+ lines)
│   └── images/
│       └── (ready for botanical graphics, logos)
└── README.md or SITEMAP.md  (This document)
```

---

## Key Messaging Framework

| Page | Primary Message | Secondary Message | CTA |
|------|-----------------|-------------------|-----|
| **Home** | "Stop grinding. Start understanding." | Boutique near-peer model | Strategy Reveal |
| **Program** | "Squads, not classes. Logic, not tricks." | Transparent 3-way contract | Application |
| **Schedule** | "Mon-Wed, noon start. 3 strategic sessions." | Clear registration deadlines | Enroll |
| **Apply** | "$300/session. Choose your path." | Simple 3-step enrollment | Application |

---

## Brand Voice & Personality

✨ **Confident**: We know our method works  
🎯 **Direct**: No corporate fluff, just results  
🤝 **Collaborative**: Emphasize squads & community  
📚 **Educational**: Transparency about process  
🌿 **Warm**: Bohemian aesthetic = welcoming, not corporate  

---

This sitemap and design direction ensures:
- **Cohesive UX**: Consistent navigation, visual language, messaging
- **Clear User Journey**: Home → Learn → Schedule → Apply
- **Conversion Optimization**: Multiple CTAs, urgency signals, trust-building
- **Brand Identity**: Pink Boho + Earthy aesthetic reflected throughout
- **Scalability**: Easy to add features (testimonials, blog, integrations)
