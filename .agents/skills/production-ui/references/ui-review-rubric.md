# UI Review Rubric

Use this rubric before shipping a production UI HTML page.

## Hierarchy

- Can a user name the page, current status, and next action within 3 seconds?
- Is there only one dominant primary action per action area?
- Are risk and compliance details above low-priority content?

## Visual System

- Are colors, spacing, radius, typography, and shadows coming from tokens?
- Are page-specific CSS rules limited to layout and content-specific refinements?
- Does the page avoid decorative gradients, excessive shadow, and unexplained ornament?

## Component Reuse

- Are repeated controls using component classes?
- Did new repeated UI become a reusable component or pattern?
- Are table, empty, loading, and error states standardized?

## Icons

- Are icons sourced from `src/assets/icons/`?
- Are icons rendered through `Icon.html` patterns or `.icon-*` classes?
- Do status icons match semantic color and include text?
- Are important actions still labeled with text instead of icon-only controls?

## Business States

- Are default, loading, empty, error, success, failed, reviewing, pending, and blocked states represented when applicable?
- Do abnormal states explain what happened, why, next action, and account/money effect?
- Are disabled actions paired with a reason?

## Responsive QA

- Check at 375px, 768px, 1024px, and 1440px.
- Tables must remain usable through horizontal scroll or responsive list treatment.
- Button text must not wrap poorly or overflow.
- Sticky mobile actions must not hide content.

## Accessibility

- Status is communicated with text, not color alone.
- Focus states are visible.
- Form fields have labels.
- Contrast is readable on all surfaces.
