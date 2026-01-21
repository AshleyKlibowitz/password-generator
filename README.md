# Secure Passphrase Generator: Length-Based Security Tool

## 📖 Project Overview

This repository documents the development of a **Secure Passphrase Generator** web application.
The goal of this project is to demonstrate front-end development capability combined with cybersecurity best practices. Unlike traditional password generators that rely solely on complexity (e.g., `xi8s7$t#6%`), this tool applies the core security principle found in the *CompTIA Security+ guide to network security fundamentals*: **"Long passwords are more secure than complex passwords"** (Ciampa, 2020). By combining randomized words with optional entropy boosters (special characters, numbers), the tool facilitates the creation of memorable yet mathematically resistant passphrases.

## ⚙️ Technical Highlights

This project displays technical proficiency across modern web development and algorithmic logic:

### Phase 1: Interactive Frontend (DOM & CSS)
* **Theming Engine:** Implemented a CSS variable-based architecture (`:root`) to handle seamless switching between **Light and Dark modes**, preserving user preference without page reloads.
* **Responsive Design:** Utilized flexbox and media queries to ensure the control interface adapts fluidly to mobile and desktop viewports.

### Phase 2: Logic & Security (JavaScript)
* **Entropy Injection:** Designed algorithms to splice random integers, special characters, and casing variations into word arrays at randomized indices, ensuring no predictable patterns.
* **Clipboard API Integration:** Built a robust "Copy to Clipboard" feature that utilizes the modern `navigator.clipboard` API with a fallback to `execCommand` for legacy browser support.

## 🔍 Security Logic (Key Principles)

The table below illustrates how specific user configurations translate into tangible security improvements based on course textbooks:

| Configuration | Input Example | Security Insight (Output) |
| :--- | :--- | :--- |
| **Word Combination** | `Select: 5 words` | **Brute Force Resistance:** Exponentially increases crack time by expanding length significantly. |
| **Separators** | `Separator: -` | **Usability:** Increases readability (memorable) without sacrificing character count. |
| **Entropy Injection** | `Random Numbers: 2` | **Pattern Disruption:** Prevents simple dictionary attacks by breaking pure word sequences. |
| **Capitalization** | `Random Caps: ON` | **Rule-Based Defense:** Counters cracking rules that assume standard sentence casing. |

### 📊 Application Interface
*A clean, user-friendly interface allowing for granular control over password generation parameters.*

<img width="1115" height="857" alt="Screenshot 2026-01-15 at 10 32 02 AM" src="https://github.com/user-attachments/assets/a891005e-a5f4-4abf-820d-b3257c676cc1" />

## ✨ Functional Features

### 1. Customization Pipeline
* **Variable Length:** Users can select between 4 to 7 words, directly influencing the "bit strength" of the resulting password.
* **Character Injection:** Granular controls to inject specific counts of numbers, letters, and special symbols to meet strict IT requirements.

### 2. User Experience (UX) Enhancements
* **Visual Feedback:** Interactive toggle states (`transition: 0.3s`) and hover effects for better usability.
* **Accessibility:** High-contrast text options in both light and dark modes to ensure readability.

## 🛠️ Technology Stack

* **Structure:** HTML5 (Semantic tags)
* **Styling:** CSS3 (CSS Variables, Flexbox, Transitions)
* **Logic:** JavaScript (ES6+, Array Manipulation, DOM Event Listeners)

## 🗄️ File Structure

The repository is organized to facilitate a review of the web application:

* `/passwordgenerator.html`: The main application structure, logic scripts, and word lists.
* `/styles.css`: The stylesheet containing the theming logic and responsive design rules.
* `README.md`: Project documentation and security justification.

## 🚀 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/password-generator.git](https://github.com/YourUsername/Password-Generator.git)
    ```

2.  **Launch the Application:**
    Simply open the `passwordgenerator.html` file in any modern web browser (Chrome, Firefox, Edge). No server or backend installation is required.

3.  **Generate a Password:**
    * Select your desired word count (Recommended: 5+).
    * Add "salt" (random numbers/specials) if required by your specific login portal.
    * Click **Generate Password** and use the **Copy to Clipboard** button.
