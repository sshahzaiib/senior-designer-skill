# Phase 4 Scored Checklist

Score every applicable item pass/fail against the actual rendered output. Web tasks score the 43 base items. SwiftUI tasks score all 55. Every item is validated 10/10 against the evidence base (see `evidence-base.md` §3 for per-item sources and scoring).

## Typography
- [ ] T1 Body 16-18px (web) / Dynamic Type styles (SwiftUI); nothing below 12px web / 11pt iOS; mobile web inputs ≥16px
- [ ] T2 Measure 45-75 characters
- [ ] T3 Line-height: body 1.3-1.5, headings 1.0-1.2 (web; system styles handle iOS)
- [ ] T4 All sizes from one modular scale / one text-style set
- [ ] T5 ≤2 typefaces, one role each, matched x-heights, none banned
- [ ] T6 ≤3 type sizes per screen; hierarchy = size + weight + color together
- [ ] T7 Caps tracked +5-12%, label-length only; lowercase body never tracked

## Color
- [ ] C1 Text ≥4.5:1 (large ≥3:1); non-text UI ≥3:1 — verified, not eyeballed
- [ ] C2 No meaning carried by color alone anywhere
- [ ] C3 One accent, rarest color on screen, primary actions only; ~3 color families; saturation small-area only
- [ ] C4 8-10 tinted neutrals from one hand-tuned scale (web) / semantic system hierarchy (SwiftUI)
- [ ] C5 No #000 body on white; dark mode: dark-gray surfaces, desaturated accents
- [ ] C6 Semantic tokens by function, conventional hues, icon/label paired

## Layout
- [ ] L1 Every spacing/size value from the scale (8px grid / point grid)
- [ ] L2 Within-group gaps visibly smaller than between-group gaps
- [ ] L3 Billboard test: each screen's purpose obvious in seconds
- [ ] L4 Everything grid-aligned; optical corrections applied
- [ ] L5 Touch targets ≥44pt/48dp
- [ ] L6 Primary actions largest and nearest; choice sets trimmed
- [ ] L7 Progressive disclosure ≤2 levels
- [ ] L8 Tables compare / lists browse / cards preview; peer content in equal cells
- [ ] L9 Tab bar 3-5 items (if mobile nav)
- [ ] L10 Same visual framework every screen; headings front-loaded

## Onboarding / States / Copy
- [ ] O1 Activation moment defined; shortest path built
- [ ] O2 No tutorial carousel; contextual guidance; skippable
- [ ] O3 Signup deferred where possible; minimal fields
- [ ] O4 No cold-launch permission requests; each tied to value
- [ ] O5 Checklists use endowed progress
- [ ] O6 Every empty state: what's missing + why + filling action
- [ ] O7 Loading tiers correct (<1s / 1-10s / >10s); skeletons content-shaped
- [ ] O8 Errors human, precise, constructive, unblaming, never premature; undo > confirm
- [ ] O9 Copy halved twice; verb+object buttons; no placeholder-as-label; one voice

## Process
- [ ] P1 Problem defined before solutions existed
- [ ] P2 4-6 real competitors analyzed by name
- [ ] P3 Goals and mental models stated, not feature lists
- [ ] P4 Heuristic self-audit (Nielsen's 10) run on the build
- [ ] P5 Zero lorem ipsum / placeholder imagery
- [ ] P6 Every major decision has rationale + 2 rejected alternatives on record

## Motion
- [ ] M1 Durations in range (web 200-500ms; SwiftUI springs at system-plausible values)
- [ ] M2 No linear easing (web) / no ease-curve movement where a spring belongs (SwiftUI)
- [ ] M3 Every animation communicates; none replay on frequent actions
- [ ] M4 Reduced-motion honored (prefers-reduced-motion / accessibilityReduceMotion)
- [ ] M5 Staggers ≤20ms; transitions spatially coherent; one focal point

## Anti-slop
- [ ] A1 No purple/indigo gradient identity
- [ ] A2 Typeface from brand reasoning, not the AI reflex set
- [ ] A3 No icon-tile card grid skeleton
- [ ] A4 No decorative glass/glow/gradient-text
- [ ] A5 Screenshot critique loop run: "could this belong to any generic template?" — if yes, redesign
- [ ] A6 Copy says specifically what the product does — zero buzzwords
- [ ] A7 Aesthetic traceable to the Phase 1 outside references
- [ ] A8 Banned list re-checked against final output
- [ ] A9 No vanilla library defaults visible
- [ ] A10 The missing layer added: real grouping, hierarchy, validation, states

## SwiftUI only (S-checklist)
- [ ] S1 All text via Dynamic Type styles or `.custom(relativeTo:)`; zero fixed font sizes
- [ ] S2 TabView 3-5 tabs, visible except in sheets; no hamburger anywhere
- [ ] S3 Push = hierarchy, sheet = self-contained task, never swapped; dirty-state Cancel confirms
- [ ] S4 Zero hardcoded hex in chrome: semantic colors + asset-catalog light/dark variants; Materials for layering; contrast verified in BOTH modes
- [ ] S5 SF Symbols matched to text style weight/scale; deliberate rendering mode
- [ ] S6 Full Dynamic Type range survives (AX5: text wraps, layout holds); VoiceOver labels complete and grouped
- [ ] S7 Springs only for movement; all animations interruptible with gesture velocity handoff
- [ ] S8 Hero/list-detail transitions use matchedGeometryEffect where elements persist
- [ ] S9 Haptics: system-meaning mapping only, prepare() called, used sparingly
- [ ] S10 Primary actions in thumb zone; sticky bottom action over header Submit
- [ ] S11 Preview matrix passed: SE-class + Pro-Max-class × light + dark × default + AX type
- [ ] S12 Native behaviors intact: edge-swipe back, rubber-band scroll, pull-to-refresh, swipe actions, context menus
