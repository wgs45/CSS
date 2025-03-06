# 🎨 CSS Syntax Cheatsheet

A complete **CSS reference** with explanations! 🖌️

---

## 📌 Basic CSS Syntax

```css
selector {
  property: value;
}
```

### 🔹 Explanation

- **`selector`** → Targets the element(s) (e.g., `p`, `.class`, `#id`).
- **`property`** → Defines what to change (e.g., `color`, `margin`).
- **`value`** → The setting applied to the property (e.g., `red`, `20px`).

Example:

```css
h1 {
  color: blue;
}
```

This makes all `<h1>` elements **blue**.

---

## 📌 CSS Selectors

### 1️⃣ Universal Selector

```css
* {
  margin: 0;
  padding: 0;
}
```

- Targets **all elements** on the page.
- Often used for **resetting default styles**.

### 2️⃣ Element Selector

```css
p {
  color: green;
}
```

- Styles **all `<p>` elements**.

### 3️⃣ Class Selector

```css
.box {
  background-color: yellow;
}
```

- Targets **any element** with `class="box"`.

### 4️⃣ ID Selector

```css
#header {
  font-size: 24px;
}
```

- Targets **only one element** with `id="header"`.
- ⚠️ IDs should be unique per page.

### 5️⃣ Grouping Selector

```css
h1,
h2,
h3 {
  font-family: Arial, sans-serif;
}
```

- Styles multiple elements at once.

### 6️⃣ Descendant Selector

```css
div p {
  color: red;
}
```

- Targets `<p>` elements **inside** `<div>`.

### 7️⃣ Child Selector

```css
div > p {
  font-weight: bold;
}
```

- Selects **direct child** `<p>` inside `<div>`.

### 8️⃣ Adjacent Sibling Selector

```css
h1 + p {
  color: gray;
}
```

- Styles `<p>` **immediately after** `<h1>`.

---

## 🎨 Colors & Backgrounds

```css
color: red; /* Sets text color */
background-color: lightblue; /* Sets element's background color */
background-image: url("image.jpg"); /* Adds an image background */
background-size: cover; /* Makes background image fit the element */
background-repeat: no-repeat; /* Prevents background from repeating */
background-position: center; /* Centers the background image */
```

### 🔹 Explanation

- `color` → Changes text color.
- `background-color` → Fills the element with a color.
- `background-image` → Sets an image as the background.
- `background-size` → Defines how the background image fits.
- `background-repeat` → Prevents tiling (repeating).
- `background-position` → Moves the background to a specific position.

---

## 🔠 Fonts & Text

```css
font-family: "Arial", sans-serif; /* Sets font */
font-size: 16px; /* Sets text size */
font-weight: bold; /* Defines text thickness */
text-align: center; /* Aligns text (left, center, right) */
text-decoration: underline; /* Adds underline, overline, or none */
line-height: 1.5; /* Adjusts space between lines */
letter-spacing: 2px; /* Increases spacing between letters */
```

### 🔹 Explanation

- `font-family` → Defines which font to use.
- `font-size` → Controls text size.
- `font-weight` → Changes thickness (bold, normal, lighter).
- `text-align` → Aligns text inside its container.
- `text-decoration` → Adds underlines or strikethroughs.
- `line-height` → Controls spacing between lines.
- `letter-spacing` → Adjusts spacing between letters.

---

## 📏 Box Model

```css
margin: 10px; /* Space outside the element */
padding: 15px; /* Space inside the element */
border: 2px solid black; /* Adds a border */
width: 200px; /* Sets element width */
height: 100px; /* Sets element height */
box-sizing: border-box; /* Includes padding & border in width/height */
```

### 🔹 Explanation

- `margin` → Creates space **outside** the element.
- `padding` → Creates space **inside** the element.
- `border` → Adds a border **around** the element.
- `width` & `height` → Controls the element's size.
- `box-sizing` → Ensures padding & borders don't change the total size.

---

## 📐 Positioning & Layout

```css
position: absolute; /* Moves element to a specific position */
position: relative; /* Moves relative to its normal position */
position: fixed; /* Stays fixed when scrolling */
position: sticky; /* Sticks at a position when scrolling */
display: flex; /* Enables flexbox layout */
display: grid; /* Enables grid layout */
z-index: 10; /* Controls which element appears on top */
```

### 🔹 Explanation

- `position` → Defines how an element is placed.
- `display` → Controls how elements are shown (flex, grid, block, inline).
- `z-index` → Determines which element appears **on top**.

---

## 🔄 Flexbox

```css
display: flex; /* Enables flexbox */
flex-direction: row; /* Aligns children in a row */
justify-content: center; /* Aligns items horizontally */
align-items: center; /* Aligns items vertically */
flex-wrap: wrap; /* Allows items to wrap */
```

### 🔹 Explanation

- `display: flex` → Turns an element into a **flex container**.
- `flex-direction` → Defines how items are placed (row/column).
- `justify-content` → Aligns items **horizontally** (left, center, space-between).
- `align-items` → Aligns items **vertically** (top, center, bottom).
- `flex-wrap` → Allows items to move to the next line.

---

## 🔳 Grid

```css
display: grid; /* Enables grid */
grid-template-columns: 1fr 2fr; /* Defines column sizes */
grid-template-rows: auto auto; /* Defines row sizes */
gap: 10px; /* Adds space between grid items */
```

### 🔹 Explanation

- `display: grid` → Turns an element into a **grid container**.
- `grid-template-columns` → Defines column sizes (`fr` = fraction).
- `grid-template-rows` → Defines row sizes.
- `gap` → Adds space **between** grid items.

---

## 🎭 Transitions & Animations

```css
transition: all 0.3s ease-in-out; /* Smooth changes */
animation: slide 2s infinite; /* Runs an animation */
```

### 🔹 Explanation

- `transition` → Animates **small** changes (color, size, opacity).
- `animation` → Defines **keyframe animations** for movement.

Example:

```css
@keyframes slide {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100px);
  }
}
```

- Moves the element **100px to the right** repeatedly.

---

## 🔥 Responsive Design

```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

### 🔹 Explanation

- `@media` → Applies styles **only** if screen width is **600px or smaller**.
- Used for **mobile-friendly design**.

---

🎨 **Complete CSS reference with explanations** 🚀
