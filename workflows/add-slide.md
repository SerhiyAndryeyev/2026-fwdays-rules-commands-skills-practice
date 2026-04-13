# Add New Slide

This workflow guides the process of adding a new slide to the presentation based on the established `plan.md` specification.

## Step 1: Review Specification
Read the `plan.md` file to identify the next slide to be implemented, focusing on its Layout, Content, and Design constraints.

## Step 2: Implement Slide
Add the new slide to `slides.md`. Follow these rules during implementation:
- **Separation**: Start with `---`.
- **Layout**: Define the layout (e.g., `layout: center`).
- **Styling**: Use UnoCSS classes.
- **Interactivity**: Add `v-click` for progressive disclosure.

## Step 3: Verify View
Run the `/run-dev` workflow to preview changes locally and verify the design meets expectations.
