# 🎨 Zylo Design System (UI/UX)
> **Premium. Glassmorphic. Minimalist.**

This document defines the visual language of **Zylo**. All modifications to the frontend must follow these guidelines to ensure the app remains a high-end alternative to standard players.

---

## 💎 The Rhombus Brand
The **Zylo** logo is a sharp, geometric Rhombus. 
* **Primary Icon:** A "Z" centered within a rhombus frame.
* **Philosophy:** Avoid "YouTube Red." The rhombus represents stability and a departure from the traditional rectangular play button.

## 🌙 Color Palette
We avoid flat blacks and pure reds. We use "Oasis Midnight" for depth.

| Element | Hex Code | Usage |
| :--- | :--- | :--- |
| **Background** | `#0B0E14` | Main application background. |
| **Surface** | `rgba(255, 255, 255, 0.05)` | Glassmorphic cards/panels. |
| **Primary Accent** | `#7C4DFF` | "Zylo Purple" - Buttons and active states. |
| **Secondary Accent** | `#00E5FF` | "Electric Cyan" - Progress bars and highlights. |
| **Text (Primary)** | `#E0E0E0` | High readability off-white. |

## 🧪 Glassmorphism Effects
To achieve the premium look, panels should use background blurs rather than solid colors.
* **Blur Strength:** `blur(12px)`
* **Border:** `1px solid rgba(255, 255, 255, 0.1)`
* **Shadow:** Soft, diffused shadows only. No hard edges.

## 🔡 Typography
We use modern, sans-serif fonts that feel tech-forward.
* **Primary Font:** `Inter` or `Geist Sans` (for that clean, developer-focused look).
* **Headings:** Bold weight with increased letter spacing (`tracking-tight`).

## 🚫 The "Invisible Player" Rule
When a video is playing:
1. **No Logos:** The Zylo and YouTube logos must be 100% hidden.
2. **Auto-Hide UI:** Controls should fade out completely after 2 seconds of inactivity.
3. **Clean Scrubbing:** The progress bar should be thin and only expand when hovered over.

---

### "Design is not just what it looks like; it's how it feels to use."
**Developed by Pavan Tej** | *Oasis Centers India*