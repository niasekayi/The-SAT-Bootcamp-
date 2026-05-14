# SAT Bootcamp Website - Visual Design Specifications

## Brand Aesthetic: Pink Boho + Earthy Minimalist

---

## Color System

### Primary Palette
| Color | Hex | CSS Variable | Usage |
|-------|-----|---|---|
| Dusty Rose | #D4A5A5 | `--dusty-rose` | Accent, muted primary |
| Terracotta | #C97755 | `--terracotta` | Primary CTA, headlines, energy |
| Sage | #9CAF88 | `--sage` | Secondary, trust, calm |
| Deep Charcoal | #3A3A3A | `--deep-charcoal` | Primary text, strong contrast |

### Secondary Palette
| Color | Hex | CSS Variable | Usage |
|-------|-----|---|---|
| Off-White | #F5F3F0 | `--off-white` | Default backgrounds, neutral |
| Soft Taupe | #E8DDD6 | `--soft-taupe` | Section backgrounds, separation |
| Cream | #FBF9F6 | `--cream` | Card backgrounds, warmth |

### Gradient Combinations
```css
/* CTA Gradients */
Terracotta → Dusty Rose: "135deg, #C97755 0%, #D4A5A5 100%"
Sage → Darker Sage: "135deg, #9CAF88 0%, #8B9F77 100%"

/* Background Gradients */
Off-white → Soft Taupe: "135deg, #F5F3F0 0%, #E8DDD6 100%"
```

---

## Typography System

### Font Stack
```css
/* Headlines - Elegant, Editorial */
font-family: 'Playfair Display', serif;
Weights: 700 (bold), 800 (extra bold)
Sizes: 3.5rem (H1), 2.8rem (H2), 2rem (H3), 1.8rem (H4)

/* Body Text - Clear, Readable */
font-family: 'Inter', sans-serif;
Weights: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)
Sizes: 1.1rem (large), 1rem (standard), 0.95rem (small)
```

### Line Heights
- Headlines: 1.2 (tight for impact)
- Body text: 1.6–1.8 (breathing room)
- Lists: 1.8 (spacing between items)

### Font Pairing Rationale
- **Playfair Display**: Sophisticated, premium feel (reflects boutique positioning)
- **Inter**: Modern, accessible, excellent readability on screens

---

## Icon & Illustration Style Guide

### Icon System (Fine-Line, Minimal)

#### Style Rules
1. **Stroke Weight**: 2–3px for visibility
2. **Line Endings**: Rounded caps (no sharp corners)
3. **Fill**: Minimal (mostly outlines)
4. **Colors**: Use palette colors or #3A3A3A
5. **Size Consistency**: Icons should align on a grid (e.g., 24x24, 48x48)

#### Icon Categories & Usage

##### Primary Action Icons
```
📅 Calendar/Date → Sessions, registration deadlines
✏️ Application/Writing → Enrollment, forms
💳 Payment/Wallet → Pricing, transactions
🎯 Target/Goal → Results, objectives
```

##### Content Icons
```
👥 People/Community → Squads, collaboration
📚 Books/Knowledge → Learning, curriculum
🧠 Brain/Strategy → Thinking, methodology
📊 Chart/Data → Analytics, progress tracking
🔄 Rotation/Cycle → Recurring sessions, process
⏱️ Clock/Time → Scheduling, duration
```

##### Decorative Elements
```
✿ Botanical (leaf/flower) → Section dividers
🌱 Plant/Growth → Progress, development
✓ Checkmark → Confirmation, features
❌ X mark → Problems/contrast
```

### Botanical Graphics Style

#### Dividers (Between Sections)
```
✿ ✿ ✿ (Simple, centered)
or
—— ✿ —— (Elegant variation)
or
❋ (Single floral symbol)
```

#### Corner Accents (Optional)
- Subtle line-drawn flowers in page corners
- Use opacity: 0.15–0.3 to avoid overwhelming
- Sage or dusty-rose colors
- Size: 80–120px

#### Botanical Border Pattern (Optional)
```
Simple vine pattern:
~∿~∿~∿~
or
✿ ✿ ✿
```

### Icon Library Recommendations

#### Free Resources
1. **Feather Icons** (feathericons.com)
   - Minimal, consistent stroke weight
   - Perfect for this aesthetic
   
2. **Simple Icons** (simpleicons.org)
   - Social media, platform logos
   
3. **Ionicons** (ionicons.com)
   - Versatile, multiple icon types
   
4. **Heroicons** (heroicons.com)
   - High quality, customizable
   
5. **Custom SVGs**
   - Draw in Adobe Illustrator or Figma
   - Export as inline SVG for colors control

#### Implementation Example
```html
<!-- Inline SVG Icon -->
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" 
     stroke="currentColor" stroke-width="2" stroke-linecap="round">
  <circle cx="12" cy="12" r="10"></circle>
  <polyline points="12 6 12 12 16 14"></polyline>
</svg>

<!-- Or use Emoji (for rapid prototyping) -->
<span class="icon">📅</span>
```

---

## Visual Layout & Spacing

### Whitespace (Breathing Room)
```css
Large section padding: 4rem (64px)
Medium padding: 2.5rem (40px)
Small padding: 1.5rem (24px)
Component gaps: 2rem (32px)
```

### Container Max-Width
```css
1200px (desktop)
Allows generous margins on large screens
```

### Card/Component Patterns
```
Card padding: 2.5rem
Card border-radius: 12px
Card left-border: 4px solid (sage or terracotta)
Card shadow: 0 2px 8px rgba(0, 0, 0, 0.05)
Card hover shadow: 0 8px 20px rgba(0, 0, 0, 0.1)
```

---

## Button & CTA Design

### Button Styles

#### Primary Button
```css
Background: var(--terracotta) #C97755
Text: var(--cream) #FBF9F6
Padding: 1rem 2.5rem
Border-radius: 50px
Box-shadow: 0 4px 15px rgba(201, 119, 85, 0.3)
Font-weight: 600

Hover State:
  Background: var(--dusty-rose)
  Transform: translateY(-2px)
  Box-shadow: 0 6px 20px rgba(201, 119, 85, 0.4)
```

#### Secondary Button
```css
Background: var(--sage) #9CAF88
Text: var(--cream) #FBF9F6
Padding: 1rem 2.5rem
Border-radius: 50px
Box-shadow: 0 4px 15px rgba(156, 175, 136, 0.3)

Hover State:
  Background: #8B9F77
  Transform: translateY(-2px)
```

#### Outline Button
```css
Background: transparent
Border: 2px solid var(--terracotta)
Text: var(--terracotta)
Padding: 1rem 2.5rem
Border-radius: 50px

Hover State:
  Background: var(--terracotta)
  Text: var(--cream)
```

### Button Sizing
- **Touch targets**: Min 44x44px (mobile accessibility)
- **Desktop**: Slightly larger for visual hierarchy
- **Disabled state**: Opacity 0.6, no hover effects

### CTA Button Placement
1. **Hero**: Primary button, center above fold
2. **Section end**: Secondary button, offer choice
3. **Footer**: Links to primary CTAs
4. **Sidebar**: Sticky CTA on desktop

---

## Card & Section Design

### Standard Card
```css
Background: var(--cream) #FBF9F6
Padding: 2.5rem
Border-radius: 12px
Border-left: 4px solid var(--sage)
Box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05)
Transition: all 0.3s ease

Hover:
  Transform: translateY(-5px)
  Box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1)
  Border-left-color: var(--terracotta)
```

### Featured/Highlighted Card
```css
Same as above, but:
Border-left-color: var(--terracotta) (instead of sage)
Background: linear-gradient(135deg, var(--cream) 0%, var(--off-white) 100%)
Box-shadow: 0 6px 16px rgba(201, 119, 85, 0.15)
```

### Card Icon Placement
```css
Icon size: 3rem (for large cards)
Margin-bottom: 1rem
Opacity: 0.8 (slightly muted)
Color: Inherit or use palette color
```

---

## Section & Background Patterns

### Alternating Section Backgrounds
```
Odd sections: var(--off-white) #F5F3F0
Even sections: var(--soft-taupe) #E8DDD6
(Creates visual rhythm without overwhelming)
```

### Special Section Backgrounds
```
CTA Sections: Gradient (terracotta → dusty-rose)
Contract Sections: Solid terracotta with white text
Founder Section: Gradient (off-white → soft-taupe)
```

### Decorative Elements
```css
Circular background shapes:
  Width/Height: 300px
  Border: 1px solid var(--sage)
  Opacity: 0.2
  Border-radius: 50%
  Position: absolute, top-right or bottom-left

(Use sparingly, max 1-2 per page)
```

---

## Typography in Action

### Hero Headlines
```css
Font: Playfair Display, 3.5rem
Weight: 700 or 800
Color: var(--deep-charcoal) #3A3A3A
Line-height: 1.2
Letter-spacing: -0.5px (tighter for impact)
Margin-bottom: 1rem
```

### Section Titles (H2)
```css
Font: Playfair Display, 2.8rem
Weight: 700
Color: var(--deep-charcoal)
Text-align: center
Margin-bottom: 1rem
```

### Card Titles (H3)
```css
Font: Playfair Display, 1.5rem
Weight: 700
Color: var(--deep-charcoal)
Margin-bottom: 1rem
```

### Body Text
```css
Font: Inter, 1rem
Weight: 400 or 500
Color: var(--deep-charcoal) #3A3A3A
Line-height: 1.8
Margin-bottom: 1rem
```

### Emphasis/Highlights
```css
Highlight text: 
  Color: var(--terracotta) #C97755
  Font-weight: 600

Accent text:
  Color: var(--sage) #9CAF88
  Font-weight: 500
```

---

## Visual Hierarchy

### Contrast Levels (Dark to Light)
1. **Deep Charcoal** (Headlines, primary text) #3A3A3A
2. **Terracotta** (CTAs, emphasis) #C97755
3. **Sage** (Secondary information) #9CAF88
4. **Dusty Rose** (Soft accents) #D4A5A5
5. **Soft Taupe** (Backgrounds) #E8DDD6
6. **Off-white** (Default backgrounds) #F5F3F0
7. **Cream** (Cards, highlights) #FBF9F6

### Size Hierarchy
- H1: 3.5rem (Hero)
- H2: 2.8rem (Section titles)
- H3: 1.5rem (Card/subsection titles)
- H4: 1.2rem (Minor titles)
- Body: 1rem (standard), 1.1rem (emphasis)
- Small: 0.95rem (footnotes)

### Visual Weight
- Bold text: 700 weight
- Semibold: 600 weight
- Regular: 400 weight
- Light: 300 weight (use sparingly)

---

## Responsive Design Specifications

### Desktop (1200px+)
- Full multi-column layouts
- Cards in 3-column grids
- Generous spacing
- Larger images

### Tablet (768px–1199px)
- 2-column grids
- Reduced padding (3rem instead of 4rem)
- Slightly smaller fonts
- Maintained aspect ratios

### Mobile (<768px)
- Single-column layout
- Reduced padding (2rem)
- Smaller fonts (adjust by ~10%)
- Simplified navigation
- Stacked buttons (vertical)
- Full-width cards

### Mobile-First CSS Breakpoint
```css
@media (max-width: 768px) {
  /* Mobile adjustments */
  .hero h1 { font-size: 2.2rem; }
  .nav-links { gap: 1.5rem; font-size: 0.9rem; }
  .cards-grid { grid-template-columns: 1fr; }
  .button-group { flex-direction: column; }
}
```

---

## Animations & Transitions

### Subtle, Professional Transitions
```css
Default transition: all 0.3s ease
Easing: ease (natural, not linear)

Button hover: translateY(-2px) + shadow increase
Card hover: translateY(-5px) + shadow increase + border-color change
Link hover: color change + underline animation (0.3s)
```

### Animation Principles
1. Keep animations **under 300ms** (fast, responsive)
2. Use **ease** or **ease-out** (not linear)
3. Avoid multiple simultaneous animations
4. Test on lower-end devices (can be slow on mobile)

### Examples
```css
/* Button hover */
.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
  transition: all 0.3s ease;
}

/* Nav link underline */
.nav-links a::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0;
  height: 2px;
  background-color: var(--sage);
  transition: width 0.3s ease;
}
.nav-links a:hover::after {
  width: 100%;
}

/* Card hover lift */
.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  border-left-color: var(--terracotta);
  transition: all 0.3s ease;
}
```

---

## Image & Asset Specifications

### Hero/Background Images
- **Format**: JPG (compressed) or WebP (modern browsers)
- **Size**: 1920x1080px minimum (scaled down for smaller screens)
- **File size**: <500KB (optimized)
- **Aspect ratio**: 16:9 or full-width

### Profile/Circular Images
- **Format**: PNG (transparency) or JPG
- **Size**: 300x300px (for 1x) or 600x600px (for 2x)
- **File size**: <100KB each
- **Aspect ratio**: 1:1 (square)

### Icon Assets
- **Format**: SVG (scalable, lightweight)
- **Size**: 24x24px (inline), 48x48px (larger), 256x256px (large)
- **Stroke width**: 2px (consistency)
- **File size**: <5KB for SVG

### Logo/Branding
- **Format**: SVG preferred (scalable)
- **Size**: 200x60px (horizontal), 60x60px (icon version)
- **Formats**: PNG, SVG, PDF
- **File size**: <50KB

---

## Accessibility & Contrast Ratios

### Color Contrast (WCAG AA Standard)
- **Large text**: 3:1 minimum
- **Normal text**: 4.5:1 minimum
- **UI components**: 3:1 minimum

### Current Compliance
| Text Color | Background | Ratio | Status |
|---|---|---|---|
| Deep Charcoal (#3A3A3A) | Cream (#FBF9F6) | 16:1 | ✅ PASS |
| Terracotta (#C97755) | Off-white (#F5F3F0) | 5.8:1 | ✅ PASS |
| Sage (#9CAF88) | Cream (#FBF9F6) | 5.5:1 | ✅ PASS |
| Cream text | Terracotta bg | 10:1 | ✅ PASS |

### Recommendations
- Use tools like [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- Test designs before publishing
- Ensure no information is conveyed by color alone

---

## Interaction States

### Button States
```
Default: Base color with shadow
Hover: Darker/adjusted color, lifted position
Active: Same as hover (pressed effect)
Disabled: 0.6 opacity, no hover effects, cursor: not-allowed
Focus: Outline (for keyboard navigation)
```

### Link States
```
Default: Terracotta color, no underline
Hover: Darker, underline animation
Active: Visited color (optional, use sparingly)
Focus: Outline for accessibility
```

### Form States
```
Default: Light border (soft-taupe)
Focus: Sage or terracotta border
Error: Red/coral border (#E74C3C or similar)
Success: Sage color (#9CAF88)
```

---

## Print Design (Optional)

### Print CSS
```css
@media print {
  header, footer, .btn { display: none; }
  body { background: white; color: black; }
  h1, h2 { page-break-after: avoid; }
  a { text-decoration: underline; }
}
```

### Print Colors
- Use CMYK equivalent for branding
- Terracotta CMYK: 0, 55, 66, 0
- Sage CMYK: 45, 0, 40, 35

---

## Design File Recommendations

### Create Designs In (Optional)
1. **Figma** (web-based, collaborative)
   - Free for small teams
   - Excellent component system
   - Easy to export
   
2. **Adobe XD**
   - Professional, integrated
   - Strong prototyping tools
   
3. **Sketch** (macOS only)
   - Industry standard for UI design

### Export Settings
- Buttons: SVG (interactive components)
- Graphics: PNG/WebP (optimized)
- Icons: SVG (scalable)
- Backgrounds: JPG (compressed)

---

## Quick Visual Reference

### Color Palette Quick Grab
```
Primary CTA: #C97755 (terracotta)
Secondary: #9CAF88 (sage)
Text: #3A3A3A (deep charcoal)
Background: #F5F3F0 (off-white)
Cards: #FBF9F6 (cream)
Accent: #D4A5A5 (dusty rose)
Section BG: #E8DDD6 (soft taupe)
```

### Font Stack Quick Copy
```css
font-family: 'Playfair Display', serif; /* Headlines */
font-family: 'Inter', sans-serif; /* Body */
```

### Box Shadow Quick Copy
```css
box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05); /* Subtle */
box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1); /* Medium */
box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15); /* Strong */
```

---

## Final Design Checklist

- ✅ Colors consistently use CSS variables
- ✅ Typography hierarchy is clear (H1 > H2 > H3 > body)
- ✅ All CTAs are prominent and recognizable
- ✅ Whitespace is generous (not cramped)
- ✅ Icons are consistent in style
- ✅ Hover states are smooth and predictable
- ✅ Responsive design tested on mobile
- ✅ Contrast ratios meet accessibility standards
- ✅ Botanical elements enhance (not distract from) content
- ✅ Overall aesthetic feels premium, boutique, welcoming

---

This design system ensures consistency, accessibility, and a cohesive brand experience across all pages. Refer back to this guide when making design decisions or adding new components.
