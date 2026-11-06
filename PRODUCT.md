# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static single-file HTML/CSS/JS, zero build, GitHub Pages deployment (consistent with all six existing family sites).

## Users

Primary: Chinese-speaking racket sports players (badminton + pickleball), age 30-50, who play 1-3 hours per session, often late evening. They experience post-play soreness, have or fear tendon issues (especially Achilles), and want to extend their athletic longevity — not optimize for competition.

Secondary: fitness-curious players researching recovery methods online, overwhelmed by conflicting advice (stretch! ice! massage! protein window!).

## Product Purpose

Tells players which recovery methods actually work (A-D evidence grades from RCT/systematic reviews), which are myths, and gives them an actionable 0-72h post-play timeline. Success = a player stops wasting time on stretching for DOMS and instead sleeps well, eats enough protein, and does progressive tendon loading. The emotional promise: "Your athletic lifespan is in your control."

## Positioning

The only recovery guide that shows its evidence grades honestly — not a listicle selling foam rollers. Each claim carries a citation (Cochrane, RCT, meta-analysis). Where evidence is weak, it says so. This "honest grading" approach is the mechanism competitors (marketing blogs, product-affiliate sites) cannot truthfully copy.

## Key Constraints

- Family design language: cream background (--cream #f7f3ea), paper cards (--paper #fffdf8), ink text (--ink #221e18), Songti serif headings, red single accent (--bing #bf3a26), bronze secondary (--zhong #a8722a). No dark sections, no gradient backgrounds, no more than one accent color per section.
- Chinese simplified, technical terms in English.
- Single-file HTML with inline CSS/JS, no external dependencies.
- PostHog telemetry (project: xiuyangshengxi), family shared sbf-uid.
- Content is evidence-graded, every claim sourced.

## Evidence Assets

- Web research agent: 14 recovery methods A-D graded, sourced from Cochrane/ACSM/ISSN/RCTs
- Gemini chat exports (6 files in /tmp/gemini-recovery-*): Achilles tendon protocols, HRV interpretation, strength training & aging fact-check, post-vacation pain self-diagnosis flow, foot callus care, medication timing for tendon pain
- These are curated personal research, not generic web content

## Accessibility

Chinese font stack (Songti SC / PingFang SC), mobile-first responsive. Text follows family baseline: 15.5px body, secondary/annotation text ≥11.5px at ≥4.5:1 contrast on cream (#6a6152 floor for small text; #8a8172 reserved for the kicker label per family canon).

## Voice

Direct, scientific but warm, occasionally witty. Numbers over adjectives. "The stretching you did after your game might have been useless" energy.
