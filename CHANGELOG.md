# Changelog

Notable changes to the WorkShip design files and this repository.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Design versions refer to the [Figma file](https://www.figma.com/design/CRmPtlj1NyeqXDfQQQRSwM/Workship---Wireframes).

## [2.0.0] - 2026-11-01 (design v2 + repository)

The full audit is in [docs/design-review.md](docs/design-review.md). In Figma, every v2 frame is `v2 / <name>`, 26,000px to the right of its untouched v1 original. The same log is also in the in-file *v2 · Read me & changelog* frame.

### Added: design foundations (Figma)
- `WorkShip v2 / Tokens` variable collection: 25 color variables (canvas, surfaces, borders, text, brand, success, warning, danger and info with subtle variants), 7 spacing and 4 radius variables, each scoped
- 9 Poppins text styles: `v2/Display`, `H1`, `H2`, `H3`, `Body`, `Body Small`, `Label`, `Caption`, `Button`
- Components: `Badge/Status` (6 tones), `Badge/Verified`, `Stage Tracker` (4 stages), `Segmented Control/Role`, `Stepper/Verification` (3 steps)
- v2 instances relinked to v2 copies of the existing components (375 instances), so v2 can change without touching v1

### Changed: system-wide (all 118 v2 nodes)
- Colors bound to variables: ~1,900 text layers and ~360 fills
- Brand pink limited to primary actions and active states. Statuses use semantic colors (e.g. "Assessment Pending" is warning, "Verified" is success, "Unverified" is danger)
- Brand fill `#F91E5A` → `#E2114D` so white button text passes WCAG AA. Pink text on dark uses the new `color/brand/text` `#FF5C8A`
- Gray text (`#7A7A7A`–`#C0C0C0`) → `color/text/secondary` `#B4B4BE`
- 165 pink-bordered inputs → neutral border with an input background
- ~310 pink glow shadows → soft neutral elevation, with 1px subtle borders on cards
- Fractional font sizes rounded; ~440 text layers mapped to v2 text styles
- Typos fixed: "Seach", "Succesfully", "San Fracisco", "Hi William Scott ,", double spaces, " % match", and the "Jon Listing Success" layer name
- Nav label "Career Compass" → "More" wherever the nav bar disagreed

### Changed: screens
- **Landing (3):** role cards get explicit CTAs; the question reads "How will you use WorkShip?"
- **Sign-up (7):** switch replaced by `Segmented Control/Role`; sign-in link at 14px and underlined; Google button made neutral; headline line breaks fixed
- **Profile creation (8):** "Step 1 of 2" progress header; hint under the disabled *Complete Profile* button
- **Home (8):** "Welcome back, William" header replaces the marketing copy; 40px search field with placeholder; Filters as a secondary button; `Badge/Verified` on featured jobs
- **Applications (2):** `Badge/Status` and `Stage Tracker` on each card; list height fits three full cards
- **Saved jobs (2) and search (1):** copied application statuses replaced with Verified + location/type; Quick Apply on saved jobs; result count on search
- **Company/logo data:** company names now match their logos (10 fixes)
- **Candidate verification (15):** `Stepper/Verification` (Academic → Experience → Certifications), dimmed under modals
- **Job hunter profile (3):** "Sign Out" → "Edit profile"; "Verify" → "Verify now →"
- **Career Compass:** offer count in success green; ghosted and rejected counts muted; placeholder tiles become "Assessments" and "+ Add a metric"
- **Wingman AI (15):** LLM usage/integrations panel → *Suggested prompts*; follow-up email uses the William Scott persona (11 fixes)
- **Analytics:** line chart over categories → labeled horizontal bar chart; stacked benchmark → grouped bars with a legend; plain chart titles
- **Company and recruiter profiles (3):** photos of real people and offices → brand banners with the company logo; "TechVision Inc." copy fixed
- **Recruiter (19 buttons):** destructive "Close" → primary "Review applicants" plus an overflow (⋯) for closing; job-posted modal → "View listing" with next-step copy
- **Job detail (2):** match donut labelled "profile match"

### Repository
- `docs/design-review.md`: prioritized audit with a before/after table and what was deferred
- `assets/v2/`: exported v2 screens plus before/after pairs
- README, `docs/screens.md` and `docs/design-system.md` updated for v2

## [1.1.0] - 2026-11-01 (repository)

### Added
- Full case-study README: problem, solution, objectives, audiences, key flows, team and role, next steps
- `docs/research.md`: target audiences, user needs, pain points, personas, empathy maps, storyboards, method rationale
- `docs/competitive-analysis.md`: feature and UX comparison vs LinkedIn, Indeed and Workday, plus positioning matrix
- `docs/use-cases.md`: Quick Apply, Post a Job, Profile Verification and Wingman AI follow-up, with alternate flows
- `docs/screens.md`: Figma file map and walkthrough of sign-up, onboarding and home
- `docs/design-system.md`: color, type, iconography, components, layout grid
- `assets/`: screens and research visuals exported from the presentation
- Links to the Figma prototype and file

### Changed
- Moved the PDFs into `docs/pdf/` with descriptive names:
  - `WorkShip.pdf` → `docs/pdf/WorkShip-Research-Report.pdf`
  - `WorkShip Presentation.pdf` → `docs/pdf/WorkShip-Final-Presentation.pdf`
- Moqups link (first-iteration wireframes) moved into the Team section of the README

## [1.0.0] - 2025-02-27

### Added
- Research report and final presentation PDFs
- README with a link to the high-fidelity wireframes in Moqups
