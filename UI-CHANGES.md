UI-CHANGES for SkillSprint

This file lists small Figma-style UI fixes and polish steps you can apply.

1. Global tokens

   - Add a CSS variables file (e.g., `src/stylesheets/tokens.css`) with primary color, spacing, and font scales.

2. Header / Navbar

   - Add a compact header with logo text `SkillSprint` and a responsive hamburger menu.
   - Ensure auth buttons (Login/Register) show on mobile as icons.

3. Auth cards

   - Center login/register cards vertically with max-width 420px.
   - Use consistent input spacing and antd form layout.

4. Exam cards

   - Use consistent card heights and show a footer with `Start Exam` and `Preview` actions.

5. Accessibility

   - Ensure buttons have aria-labels and contrast ratios meet WCAG AA.

6. Responsive
   - Fix grid breakpoints: small (1 col), medium (2 cols), large (4 cols).

Notes: These are small, low-risk changes. I can produce exact code patches for any of the items above on request.
