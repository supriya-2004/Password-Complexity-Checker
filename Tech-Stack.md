# Technologies Used

This document provides a structured breakdown of the main components and functions used in the Password Strength Checker project.

---

## 📄 HTML – Main Elements & Their Functions

- **`<div class="container">`**  
  → Main wrapper that contains the entire password checker UI.

- **`<input type="password" id="YourPassword">`**  
  → Input field for users to type their password.

- **`<div class="show">`**  
  → Toggle button that switches between “Show” and “Hide” for the password.

- **`<div class="strengthMeter">`**  
  → Visual meter bar that reflects the strength of the entered password.

---

## 🎨 CSS – Main Classes & Their Roles

- **`.container`**  
  → Styles the form container including layout, background, padding, and box shadow.

- **`.inputArea input`**  
  → Styles the password input field with colors, borders, and focus effects.

- **`.strengthMeter::before`**  
  → Creates an animated inner bar that adjusts width and color based on password strength.

- **`.container.weak / .moderate / .strong`**  
  → Defines different visual themes and labels based on password strength.

- **`.show` and `.show.hide`**  
  → Styles the toggle button and switches content between “Show” and “Hide”.

---

## ⚙️ JavaScript – Main Functions & Logic

- **`Strength(password)` function**  
  → Calculates the strength of the password based on criteria like length, uppercase letters, numbers, and patterns.

- **`keyup` event listener**  
  → Every time a key is released, the strength is recalculated and the visual feedback is updated accordingly by changing container classes.

- **`show.onclick` event handler**  
  → When the toggle is clicked, it switches the input type between `password` and `text`, changing visibility of the entered password.
