# 🎨 **CSS Cheatsheet** 🎨

---

## 🔹 **CSS Selectors (How to Target Elements?)**

| Selector             | Description                    | Example                             |
| -------------------- | ------------------------------ | ----------------------------------- |
| `*`                  | Selects all elements           | `* { color: red; }`                 |
| `element`            | Selects all elements of a type | `p { font-size: 16px; }`            |
| `.class`             | Selects elements with a class  | `.box { border: 1px solid black; }` |
| `#id`                | Selects elements with an ID    | `#header { background: blue; }`     |
| `element1, element2` | Selects multiple elements      | `h1, h2 { color: green; }`          |
| `element element`    | Selects nested elements        | `div p { color: blue; }`            |
| `element > element`  | Selects direct child           | `ul > li { color: red; }`           |
| `element + element`  | Selects adjacent sibling       | `h1 + p { font-style: italic; }`    |

✅ **Example:**

```css
.container .box {
  color: red;
}
```

👀 **Visual:**  
📦 **Container**  
&nbsp;&nbsp;📦 **Box** (Text will be red!)

---

## 🎨 **Colors & Backgrounds**

🔹 **Text Colors:**

```css
color: red; /* Named color */
color: #ff5733; /* Hex code */
color: rgb(255, 87, 51); /* RGB */
color: rgba(255, 87, 51, 0.5); /* Transparent */
```

🔹 **Background Styling:**

```css
background-color: yellow; /* Solid color */
background-image: url("image.jpg"); /* Background image */
background-size: cover; /* Cover entire container */
background-repeat: no-repeat; /* Prevent repeating */
background-position: center; /* Center image */
```

👀 **Visual:**  
🟦 `background-color: blue;`  
🟥 `background-color: red;`  
🟨 `background-color: yellow;`

---

## 🖋️ **Text & Font Styling**

```css
font-family: "Arial", sans-serif; /* Change font */
font-size: 20px; /* Size of text */
font-weight: bold; /* Bold text */
font-style: italic; /* Italic */
text-align: center; /* Center align */
text-decoration: underline; /* Underline */
text-transform: uppercase; /* Capitalize text */
letter-spacing: 2px; /* Adjust spacing between letters */
word-spacing: 5px; /* Adjust spacing between words */
line-height: 1.5; /* Adjust line height */
```

👀 **Visual Example:**

| **CSS Rule**                  | **Effect**              |
| ----------------------------- | ----------------------- |
| `text-transform: uppercase;`  | **HELLO WORLD**         |
| `letter-spacing: 3px;`        | **H E L L O W O R L D** |
| `text-decoration: underline;` | **Hello World**         |

---

## 📏 **Box Model (Spacing & Sizing)**

🔹 **Key Properties**

```css
width: 100px;
height: 200px;
margin: 10px; /* Space outside */
padding: 15px; /* Space inside */
border: 2px solid black; /* Outline */
border-radius: 10px; /* Rounded corners */
box-shadow: 5px 5px 10px gray; /* Shadow effect */
```

👀 **Box Model Diagram:**

```
margin
┌───────────────────┐  🔳 Border
│   Padding         │
│   ┌───────────┐   │
│   │  Content  │   │
│   └───────────┘   │
└───────────────────┘
```

✅ **Margin** (Outer spacing)  
✅ **Padding** (Inner spacing)  
✅ **Border** (Outline of the box)

---

## 🎭 **Display & Positioning**

🔹 **Common Display Types**

```css
display: block; /* Full width */
display: inline; /* Inline element */
display: flex; /* Flexbox */
display: grid; /* Grid layout */
```

🔹 **Positioning Elements**

```css
position: static; /* Default */
position: relative; /* Move relative to itself */
position: absolute; /* Move relative to parent */
position: fixed; /* Stay fixed while scrolling */
position: sticky; /* Sticks to viewport */
```

👀 **Visual Positioning Example:**

```
----------------------
|       Header       |
----------------------
| Sidebar | Content  |
| Sidebar | Content  |
----------------------
|       Footer       |
----------------------
```

Using **Flexbox or Grid** can help arrange layouts like this easily!

---

## 🖼️ **Flexbox (Responsive Layouts)**

🔹 **Flexbox Basics**

```css
display: flex; /* Enables flexbox */
flex-direction: row; /* Items in a row */
justify-content: center; /* Center horizontally */
justify-content: space-between; /* Distribute space */
align-items: center; /* Align items vertically */
flex-wrap: wrap; /* Wrap items */
```

👀 **Flexbox Visual Representation:**

```
| 🟥 🟦 🟨 |   justify-content: center;
|🟥 🟦 🟨  |   flex-direction: column;
| 🟥 🟦 🟨 |   align-items: center;
```

---

## 📊 **Grid Layout (Powerful Layouts)**

🔹 **Grid Basics**

```css
display: grid;
grid-template-columns: repeat(3, 1fr); /* 3 equal columns */
grid-template-rows: auto auto; /* Row heights */
grid-gap: 10px; /* Spacing */
align-items: center;
```

👀 **Grid Example:**

```
---------------------
| 🟥 | 🟦 | 🟨 |
---------------------
| 🟩 | 🟪 | 🟧 |
---------------------
```

Each box can be placed and resized easily using `grid-column` and `grid-row`!

---

## 🚀 **Animations & Transitions**

🔹 **Smooth Transitions**

```css
transition: all 0.5s ease-in-out; /* Smooth animations */
transform: rotate(45deg); /* Rotate effect */
transform: scale(1.2); /* Scale up */
```

🔹 **Keyframe Animations**

```css
@keyframes bounce {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: translateY(0);
  }
}
.animation-box {
  animation: bounce 1s infinite;
}
```

👀 **Example Animation:**
🔴⬆️⬇️🔴 (Bouncing effect!)

---

## 📱 **Responsive Design (Mobile Friendly!)**

```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

👀 **Effect:**  
✅ If the screen width is below 600px, the background turns gray! 🎉

---

### 🎉 **Final Thoughts**

- ✅ This cheatsheet covers **ALL** major CSS topics!
- ✅ Use **Flexbox & Grid** for layouts 📐
- ✅ **Animations & Transitions** make your website dynamic! 🎬
- ✅ **Media Queries** make your website mobile-friendly! 📱
