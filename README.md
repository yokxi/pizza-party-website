# 🍕 Pizza Party Website

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Modern and dynamic website for managing the Pizzeria.
The site includes a menu and event management system based on **Google Sheets**, allowing for real-time updates without modifying the code.

**[🌐 View the website online](https://yokxi.github.io/pizza-party-website/)**

---

## 🍕 Manager's Guide

The website automatically reads data from a Google Excel file. To change prices, pizzas, or events, simply modify that file.

### 1. How to Edit the Pizza Menu
Open the **"Menu Pizze"** tab (bottom left of the sheet).
Fill in the columns following this exact order:

| Column | What to Write | Example |
| :--- | :--- | :--- |
| **A: Nome** | The name of the pizza | `Margherita` |
| **B: Descrizione** | Ingredients | `Tomato, mozzarella, basil` |
| **C: Prezzo** | The price (number only or with comma) | `6,50` |
| **D: Specialita** | Write **"si"** to add a colored badge | `si` (or leave empty) |

> **Note:** Changes will appear on the site after a few minutes. Try reloading the page if you don't see them immediately.

### 2. How to Manage Private Events
Open the **"Menu Eventi"** tab (at the bottom).
Here you can create custom menus for parties or corporate dinners.

| Column | What to Write | Example |
| :--- | :--- | :--- |
| **A: Evento** | Event name (same for all rows of that event) | `Marco's Birthday` |
| **B: Data** | Date of the party | `12/05/2025` |
| **C: Nome Pizza** | Pizza chosen for this event | `Diavola` |
| **D: Descrizione** | Ingredients (or special notes) | `No onions` |
| **E: Prezzo** | Agreed price (or empty) | `8,00` |

**Practical Example:**
If there are 3 pizzas for an event, you must fill in **3 rows**, repeating the event name in the first column for all three.

---

## 📂 File Structure
- `index.html`: Home page with Hero, About Us, Menu Teaser.
- `menu.html`: Complete Menu page (loaded from Google Sheets).
- `eventi.html`: Page dedicated to guests of private events.
- `style.css`: Unique stylesheet for the entire site.
- `script.js`: Mobile menu management and scroll animations.

## 🚀 Site Management
The site is configured to run autonomously.
To update content visible to customers (prices, new pizzas, special events), **exclusively use the Google Sheet**. There is no need to modify any code files.

---
&copy; 2025 Pizza Party Project
