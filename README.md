# 🌊 Ocean Depths — Frontend Odyssey Submission

> *"A story told in five thousand fathoms"*

An immersive scroll-driven storytelling experience that takes users on a narrative journey from the sunlit ocean surface to the deepest trench on Earth — the Challenger Deep at 11,034m.

---

## ✅ Mandatory Requirements Checklist

| Requirement | Implementation |
|---|---|
| **5+ Story Sections** | Hero (The Call) · Introduction (Descent) · Exploration I (Twilight) · Exploration II (Midnight) · Insight (Abyss) · Conclusion (Hadal) |
| **2+ Scroll Effects** | Parallax hero layers + caustic rays · Scroll-triggered reveals on every element · Background color morphs smoothly across entire page |
| **3+ Interactions** | Creature card hover lift · Accordion toggles (Abyss) · Bioluminescent orb hover · Fact chip hover · Nav dot tooltips · Keyboard arrow navigation |
| **3+ Animations** | Custom wave loader · Fish school swimming · Caustic light ray sway · Bioluminescent pulse orbs · Hydrothermal vent smoke · Bubble particle system · Canvas particle system |
| **Responsive Design** | Mobile / Tablet / Desktop — fluid with `clamp()` + CSS Grid auto-fit |
| **Bonus: Accessibility** | ARIA labels · `prefers-reduced-motion` · Keyboard navigation · Focus styles |
| **Bonus: Performance** | Passive scroll listeners · `will-change` only where needed · Canvas particles toggle off when out of view · No external JS dependencies |

---

## 🗂️ Project Structure

```
ocean-depths/
├── index.html              ← Main HTML (all 6 chapters)
├── css/
│   ├── reset.css           ← Box-sizing, scrollbar, reduced-motion
│   ├── variables.css       ← Design tokens (colours, fonts, spacing)
│   ├── loader.css          ← Loading screen with animated waves
│   ├── ui.css              ← Cursor, depth meter, nav dots, bubbles
│   ├── sections.css        ← All chapter styles (hero → hadal)
│   ├── animations.css      ← Reveal system, keyframes, parallax helpers
│   └── responsive.css      ← Tablet + mobile breakpoints
├── js/
│   ├── loader.js           ← Progress bar simulation + hide on complete
│   ├── cursor.js           ← Smooth custom cursor with hover states
│   ├── bubbles.js          ← Dynamic bubble DOM generation
│   ├── scroll.js           ← Depth meter · BG colour · Reveals · Parallax
│   ├── accordion.js        ← Abyss creature toggle panels
│   └── particles.js        ← Canvas bioluminescent particles + hadal stars
└── README.md
```

---

## 🚀 Getting Started in VS Code

### Step 1 — Open the project
```bash
# Option A: Open folder in VS Code directly
code ocean-depths/

# Option B: File → Open Folder → select ocean-depths/
```

### Step 2 — Install Live Server extension
1. Press `Ctrl+Shift+X` (Extensions panel)
2. Search **"Live Server"** by Ritwick Dey
3. Click **Install**

### Step 3 — Run the project
- Right-click `index.html` in the Explorer panel
- Select **"Open with Live Server"**
- Browser opens at `http://127.0.0.1:5500`

> 💡 Every time you save a file, Live Server auto-refreshes the browser instantly.

### Step 4 — Recommended VS Code Extensions
| Extension | Why |
|---|---|
| **Live Server** | Auto-reload on save |
| **Prettier** | Auto-format HTML/CSS/JS |
| **Color Highlight** | Visualize CSS colors inline |
| **CSS Peek** | Click class names → jump to CSS |
| **GitLens** | Better Git history |

---

## 📦 GitHub Setup (Day 6)

```bash
# 1. Initialize git in the project folder
cd ocean-depths
git init
git add .
git commit -m "feat: Ocean Depths — Frontend Odyssey submission"

# 2. Create repo on github.com
#    → Click New Repository → Name: "ocean-depths-odyssey" → Public → Create

# 3. Link and push
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ocean-depths-odyssey.git
git push -u origin main
```

---

## 🌐 Vercel Deployment (5 minutes)

1. Go to **[vercel.com](https://vercel.com)** → Sign up with GitHub
2. Click **"Add New Project"**
3. **Import** `ocean-depths-odyssey` from your GitHub repos
4. Framework Preset: **Other** (static HTML — no build step)
5. Click **Deploy**
6. ✅ Live at: `https://ocean-depths-odyssey.vercel.app`

> Every `git push` auto-triggers a new deployment.

---

## 📝 Project Description (200–300 words)

**Ocean Depths** is an immersive, scroll-driven storytelling experience that guides users on a narrative journey from the sunlit ocean surface to the deepest point on Earth — the Challenger Deep at 11,034 metres. The experience is structured as a six-act story: Hero, Introduction, two Exploration chapters, an Insight act, and a Conclusion.

As users scroll, the world transforms. The background colour morphs seamlessly from tropical teal to absolute black, tracking the descent in real time. A depth meter on the right edge counts down in metres and kilometres. Parallax hero layers — caustic light rays, swimming fish schools, coral silhouettes — shift at different speeds to create genuine spatial depth.

Each chapter introduces new interactive elements: creature cards with hover lift-and-glow effects, bioluminescent orb animations that pulse with different colours representing the four types of deep-sea light, animated accordion panels revealing the strange inhabitants of the abyss, and a pressure visualiser that animates on scroll entry. A canvas-based particle system generates floating bioluminescent dots in the midnight zone and below.

The experience was built with zero external JavaScript dependencies — pure vanilla HTML, CSS, and JavaScript — for maximum performance. Smooth custom cursor, keyboard arrow key navigation, and ARIA labels ensure accessibility across devices and assistive technologies. A `prefers-reduced-motion` media query disables all animations for users who prefer it.

The goal: make the ocean feel alive, alive with mystery, and make users feel the weight of the water above them as they descend.

---

## 🏆 Judging Criteria Coverage

| Criteria | Weight | How this project covers it |
|---|---|---|
| Creativity & Storytelling | 30% | Six-act narrative arc with literary writing, quotes, and character vignettes |
| Visual Design | 25% | Playfair Display + DM Mono typography, evolving dark colour palette, layered visual depth |
| Animation & Interactivity | 20% | 10+ distinct animations; all interactions are meaningful and story-relevant |
| Responsiveness | 15% | Fully tested grid layouts, fluid `clamp()` sizing, mobile-specific overrides |
| Code Quality | 10% | Modular file structure, commented JS, CSS custom properties, semantic HTML |
| **Bonus** | + | Accessibility (ARIA, keyboard nav, reduced-motion), zero dependencies, canvas particles |
