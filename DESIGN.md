# Design System Document: MIRJUN S.A.

## 1. Overview & Creative North Star: "The Architectural Monolith"
Construction is the art of balancing immense weight with precision engineering. This design system departs from generic "corporate" templates to embrace a **Creative North Star** we call **"The Architectural Monolith."** 

The aesthetic is characterized by structural stability, expansive negative space, and intentional asymmetry. We move away from the "boxed-in" web by using the `primary` #6A2B86 (Morado Mirjun) as a structural anchor—like a steel beam—against the `surface` #fbf9f8. By utilizing high-contrast typography scales and overlapping tonal layers, we create a digital experience that feels as solid and premium as a MIRJUN S.A. build.

---

## 2. Colors & Tonal Depth
We do not use color merely for decoration; we use it to define volume.

### The Palette (Core Tokens)
- **Brand Primary:** `#6A2B86` (Morado Mirjun) - Used for primary actions and structural highlights.
- **Surface (Background):** `#fbf9f8` - A sophisticated off-white that feels more premium than a clinical hex-white.
- **On-Surface (Text):** `#1b1c1c` - Our "Gris Carbón" equivalent, optimized for digital legibility.

### The "No-Line" Rule
**Explicit Instruction:** Prohibit the use of 1px solid borders for sectioning. 
Construction is about slabs and volumes. Boundaries must be defined solely through background color shifts. To separate a testimonial section from a hero section, transition from `surface` to `surface-container-low`. 

### Surface Hierarchy & Nesting
Treat the UI as a series of stacked physical materials.
*   **Level 0 (Base):** `surface` (#fbf9f8)
*   **Level 1 (Sectioning):** `surface-container-low` (#f6f3f2)
*   **Level 2 (Cards/Modules):** `surface-container-lowest` (#ffffff) - This creates a subtle "lift" against the off-white base without needing a shadow.

### The Glass & Gradient Rule
To prevent a "flat" look, use **Glassmorphism** for floating navigation bars or overlays. Use `surface` with an 80% opacity and a `backdrop-blur` of 12px. For high-impact CTAs, use a subtle linear gradient from `primary` (#510e6d) to `primary_container` (#6a2b86) at a 135-degree angle to add "visual soul."

---

## 3. Typography: Editorial Authority
We use **Manrope** for its geometric stability and modern construction feel.

*   **Display (lg/md/sm):** Used for hero statements. Utilize `display-lg` (3.5rem) with tight letter-spacing (-0.02em) to create a "heavy" architectural presence.
*   **Headline (lg/md/sm):** Reserved for section starts. Always in `on_surface` (#1b1c1c).
*   **Title (lg/md/sm):** For card headers and subsection leads. Use `SemiBold` weights.
*   **Body (lg/md):** For project descriptions. Always use `body-lg` (1rem) for better readability on construction-heavy data.
*   **Label (md/sm):** All-caps, tracked out (+0.05em) for technical metadata or small accents.

---

## 4. Elevation & Depth: Tonal Layering
In this system, depth is "baked-in," not "pasted-on."

*   **The Layering Principle:** Avoid shadows. If a card needs to stand out, place a `surface-container-lowest` (#ffffff) card on a `surface-container` (#f0eded) background. This "Tonal Lift" is the hallmark of high-end design.
*   **Ambient Shadows:** If a floating element (like a Modal) is required, use an extra-diffused shadow: `box-shadow: 0 20px 40px rgba(27, 28, 28, 0.06)`. The shadow color must be a tint of the `on_surface` color, never pure black.
*   **The "Ghost Border" Fallback:** If a divider is essential for accessibility, use the `outline_variant` token at **15% opacity**. High-contrast lines are strictly forbidden.

---

## 5. Components

### Buttons (The Structural Unit)
*   **Primary:** Solid `primary` (#6A2B86) with `on_primary` (#ffffff) text. Roundness: `sm` (4px/0.25rem). 
*   **Secondary:** `primary_container` (#6a2b86) background with a "Glass" hover state. 
*   **Tertiary:** No background. Text-only with a subtle `primary` underline on hover.

### Cards & Content Modules
*   **Constraint:** Never use divider lines inside cards. 
*   **Spacial Separation:** Use the Spacing Scale (specifically `8` / 2rem) to separate a header from body text. Use `surface-container-highest` for small "tag" backgrounds within the card.

### Input Fields
*   **Style:** Minimalist. No full-box borders. Use a `surface-container-high` background with a 2px `primary` bottom-border that activates on focus.
*   **Labeling:** `label-md` typography should sit 4px above the input field.

### Signature Component: The "Project Stat" Chip
A high-contrast module using `primary_fixed` (#f8d8ff) background and `on_primary_fixed` (#320047) text to highlight construction metrics (e.g., "150+ Projects Completed") with `title-lg` typography.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** embrace asymmetry. Align a headline to the left and a body paragraph to the right to create "Architectural Tension."
*   **Do** use the `24` (6rem) spacing token for vertical section padding to let the content breathe.
*   **Do** use `surface_tint` (#82439e) for very subtle icon backgrounds or accent decorations.

### Don't:
*   **Don't** use a 1px solid #333 border. It breaks the "Monolith" feel and looks dated.
*   **Don't** use standard "drop shadows" on cards. Rely on background color shifts (`surface` vs `surface-container`).
*   **Don't** crowd the layout. If a section feels busy, double the padding. MIRJUN S.A. represents premium quality; quality needs space.
*   **Don't** use fully rounded (pill) buttons. Stick to the `0.25rem` (4px) radius to maintain the "solid" construction aesthetic.