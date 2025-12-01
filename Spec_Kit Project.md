# AI-Native Driven Development Book Website (Next.js + Spec-Kit Plus)
Full Step-by-Step Guide (Copy-Paste Ready)

## Step 1: System Ready Karo

```bash
# Python version check (3.12+ hona chahiye)
python --version

# Spec-Kit Plus install
pip install specifyplus

# Next.js project folder banao
mkdir ai-native-book && cd ai-native-book

# Spec-Kit Plus project init
specifyplus init ai-native-book

# AI tool select karo → Claude Code (recommended)
# Terminal → bash
```

## Step 2: Project Folder Mein Jao & Claude Launch

```bash
cd ai-native-book
claude
```

Ab tum Claude CLI ke andar ho – yahan se saare `/sp.` commands chalenge.

## Step 3: Constitution (Global Rules)

Run the following command:

```bash
/sp.constitution
```

**Project:** AI-Native Driven Development – Premium Book Website (Next.js 15 + Tailwind + MDX)

**Core Principles:**
- Zero external UI libraries except shadcn/ui & Tailwind
- Mobile-first, glassmorphism + gradient design
- MDX for all book content (easy future updates)
- Dark/Light mode toggle
- Lightning fast (<1.5s FCP)
- 100% accessible (ARIA + keyboard nav)

**Standards:**
- TypeScript strict mode
- All components reusable
- Chapter content in `/content/chapters/`
- Total bundle size < 150KB (without images)

**Constraints:**
- 4 pages only: Home, Book, About, Contact
- Book = 5 chapters × 2 topics each
- Deploy on Vercel (free)

## Step 4: Specification (Kya Banana Hai)

Run the following command:

```bash
/sp.specify AI-Native Book Website
```

**Intent:**
Create a premium Single source of truth book website AI-Native-Driven Development And explain 5 chapters of this topic.

**Pages:**
1. **Home** → Hero + Book preview + CTA
2. **Book** → Full scrollable book with chapter navigation + progress bar
3. **About** → Author bio + vision
4. **Contact** → Waitlist form (save to localStorage)

**Success Criteria:**
- Book has exactly 5 chapters, each with 2 topics
- Smooth scroll + chapter progress bar
- Mobile perfect + dark mode
- All content in MDX (easy to update)
- Deployed live link within 30 minutes
- Looks like $10k website

**Non-goals:**
- Backend, auth, payments, comments

## Step 5: Plan Phase

Run the following command:

```bash
/sp.plan
```

Create full Next.js 15 (App Router) + Tailwind + MDX architecture.

**Phases:**
1. Project setup + Tailwind + shadcn
2. Layout + Navigation + Theme provider
3. Home page (Hero + Chapter cards)
4. Book page (MDX loader + progress bar + TOC)
5. About + Contact pages
6. Content (5 chapters in MDX)
7. Polish + deploy

**Important decisions:**
- MDX vs plain React → **MDX** (easy content updates)
- App Router vs Pages Router → **App Router** (Next.js 15)
- localStorage vs backend → **localStorage** (MVP)

## Step 6: Tasks Phase (Auto generate atomic tasks)

Run the following command:

```bash
/sp.tasks
```

## Step 7: Implement Shuru!

Run the following command:

```bash
/sp.implement
```

---

**Thank You! Like and subscribe to my channels.**
