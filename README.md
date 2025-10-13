[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/_4ZwDETh)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=21020005)
# Mastering CSS Layouts: Flexbox vs. Grid Learning Activity

## Overview

This learning activity will guide students through creating the same page layout using both Flexbox and CSS Grid. By implementing identical layouts with different techniques, students will develop a deep understanding of when and how to use each approach effectively.

## Learning Objectives

- Understand the fundamental concepts of both Flexbox and CSS Grid
- Recognize the strengths and limitations of each layout system
- Develop practical skills in implementing responsive layouts
- Build critical thinking about which layout system to choose for different scenarios

## Prerequisites

- Basic knowledge of HTML and CSS
- Understanding of CSS selectors and properties
- Familiarity with browser developer tools

---

## Level 1: Basic Layout (Beginner)

### Challenge

Create a simple webpage with a header, main content area, and footer using both Flexbox and Grid.

### Requirements

**Layout Structure:**
- Header (full width, fixed height)
- Main content (full width, expands to fill available space)
- Footer (full width, fixed height)

**Implementation Tasks:**
1. First create this layout using Flexbox
2. Then recreate the same layout using CSS Grid
3. Make both versions responsive (stack on mobile)

### Expected Output (Both Versions)

```
+---------------------+
|       Header        |
+---------------------+
|                     |
|    Main Content     |
|                     |
+---------------------+
|       Footer        |
+---------------------+
```

### Key Concepts to Apply

**Flexbox:**
- `display: flex`
- `flex-direction: column`
- `flex-grow`

**Grid:**
- `display: grid`
- `grid-template-rows`
- `grid-template-areas` (optional for this level)

---

## Level 2: Multi-Column Layout (Intermediate)

### Challenge

Create a webpage with a header, navigation, main content with sidebar, and footer using both Flexbox and Grid.

### Requirements

**Layout Structure:**
- Header (full width)
- Navigation menu (full width)
- Main content area (70% width) with sidebar (30% width)
- Footer (full width)

**Implementation Tasks:**
1. Create this layout using nested Flexbox containers
2. Recreate the same layout using CSS Grid
3. Implement responsive design:
   - Desktop: Layout as described above
   - Mobile: All sections stack vertically

### Expected Output (Both Versions)

```
+---------------------+
|       Header        |
+---------------------+
|        Nav          |
+---------------------+
|          |          |
|  Main    | Sidebar  |
|  Content |          |
|          |          |
+---------------------+
|       Footer        |
+---------------------+
```

### Key Concepts to Apply

**Flexbox:**
- Nested flex containers
- `flex-wrap`
- `flex-basis` vs. width

**Grid:**
- `grid-template-columns: 7fr 3fr`
- Basic media queries
- `grid-template-areas`

---

## Level 3: Complex Layout (Advanced)

### Challenge

Create a full webpage layout matching the example provided in the previous artifact (header, navigation, main content, left sidebar, right sidebar, and footer) using both Flexbox and Grid.

### Requirements

**Layout Structure:**
- Header (full width)
- Navigation menu (full width)
- Left sidebar (20% width)
- Main content (60% width)
- Right sidebar (20% width)
- Footer (full width)

**Implementation Tasks:**
1. Create this layout using nested Flexbox containers
2. Recreate the same layout using CSS Grid with named areas
3. Implement a comprehensive responsive strategy:
   - Desktop: Full layout as described
   - Tablet: Left and right sidebars become equal width columns below the main content
   - Mobile: All sections stack vertically

### Expected Output (Both Versions)

```
+---------------------+
|       Header        |
+---------------------+
|        Nav          |
+---------------------+
|     |       |       |
| Left|       | Right |
| Side| Main  | Side  |
| bar |       | bar   |
|     |       |       |
+---------------------+
|       Footer        |
+---------------------+
```

### Key Concepts to Apply

**Flexbox:**
- Complex nested flex containers
- Order manipulation for responsive layouts
- Advanced alignment techniques

**Grid:**
- Named grid areas
- Complex media queries
- `grid-column` and `grid-row` properties

---

## Level 4: Holy Grail Layout with Challenges (Expert)

### Challenge

Create the classic "Holy Grail" layout with additional interactive components and layout variations.

### Requirements

**Base Layout Structure:**
- Header with logo and user menu
- Navigation with horizontal menu items
- Left sidebar (fixed width)
- Main content (flexible)
- Right sidebar (fixed width)
- Footer with multiple sections

**Additional Requirements:**
- Header remains fixed at the top when scrolling
- Main content has card-based layout that reflows based on available space
- Sidebars can collapse/expand on user interaction
- Footer contains a 3-column grid of links

**Implementation Tasks:**
1. Create the layout using advanced Flexbox techniques
2. Recreate using CSS Grid with subgrids (where supported)
3. Implement all interactive features with minimal JavaScript
4. Support four responsive breakpoints with different layouts

### Key Concepts to Apply

**Flexbox:**
- Combining `flex-grow`, `flex-shrink`, and `flex-basis`
- Using `align-self` and `justify-content`
- Flexbox alignment with `margin: auto`

**Grid:**
- Overlapping grid areas
- CSS Grid alignment properties
- Complex auto-placement rules
- Subgrid (where supported)

**Shared Concepts:**
- Custom properties for layout dimensions
- `clamp()` for responsive sizing
- Container queries (where supported)

---

## Submission Requirements (All Levels)

For each level, students should submit:

1. HTML file with semantic markup
2. Two separate CSS files:
   - `flexbox-style.css`
   - `grid-style.css`
3. A brief reflection document (300-500 words) comparing their experience with both layout systems:
   - Which was easier to implement?
   - Which required less code?
   - Which was more intuitive?
   - In what scenarios would they prefer one over the other?

## Assessment Criteria

- **Functionality:** Both layouts should look identical and behave as specified
- **Code Quality:** Clean, well-commented, and logically organized code
- **Responsiveness:** Layouts adapt appropriately to different screen sizes
- **Optimization:** Efficient CSS with minimal redundancy
- **Analysis:** Thoughtful comparison between Flexbox and Grid implementations

---

## Learning Resources

### Flexbox Resources
- MDN Flexbox documentation: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox
- Flexbox Froggy (game): https://flexboxfroggy.com/
- CSS-Tricks Flexbox Guide: https://css-tricks.com/snippets/css/a-guide-to-flexbox/

### CSS Grid Resources
- MDN Grid documentation: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids
- Grid Garden (game): https://cssgridgarden.com/
- CSS-Tricks Grid Guide: https://css-tricks.com/snippets/css/complete-guide-grid/

### Comparison Resources
- "When to Use Flexbox and When to Use Grid" by Rachel Andrew
- Browser Developer Tools (Grid and Flexbox inspectors)

---

## Extension Activities

1. **Performance Comparison:** Use browser developer tools to measure rendering performance of both layouts
2. **Accessibility Audit:** Evaluate the accessibility of both implementations
3. **Animation Challenge:** Add smooth transitions when layouts change for responsive breakpoints
