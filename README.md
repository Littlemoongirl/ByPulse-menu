# ByPulse-menu
# ByPulse Screen Menu

An animated, full-screen display page for the in-store screens at **ByPulse**, Dubai's first AI-operated juice bar at TheBlock, One Central.

It shows the ByPulse branding and a large QR code. Customers scan the code to order through Suzy.

## Files

| File | What it is |
|------|------------|
| `index.html` | The page (all styles and animations are inside this file) |
| `logo.png` | ByPulse logo in Lime, transparent background |
| `qr.png` | QR code that opens the ByPulse ordering page |

All three files must stay in the same folder, with these exact names.

## Features

- Built for display screens: fits one screen with no scrolling, and needs no clicking
- Works on both portrait (vertical) and landscape (horizontal) screens
- Intro animation where juice fills the screen, then the page reveals
- Animated "Menu." heading, a heartbeat line, and a gently beating logo
- Rotating typed lines and two slow scrolling banners, using copy from the ByPulse deck
- Large QR code in a spinning brand-colour frame
- Brand colours (Lime `#A1FF92`, Citrus, Raspberry, Plum, Ink `#121212`) and fonts (Fredoka + DM Sans)
- Reloads itself every 30 minutes, so any update shows on the screens automatically
- Respects the "reduce motion" setting on devices that have it turned on

## How to use it on a screen

1. Open the live link in the screen's browser.
2. Press **F11** for full screen.

## How to update

All of these are in `index.html` (open it in VS Code):

- **Typed lines:** search for `const lines`
- **Banner words:** search for `fill('trackA'` and `fill('trackB'`
- **Typing speed:** search for `}, 20);`. A smaller number types faster.
- **Banner speed:** search for `animation: scroll 90s`. A bigger number moves slower.
- **QR code:** replace `qr.png` with a new image that has the same file name.

After editing, upload the changed file to this repository. The screens pick up the change within 30 minutes.

## Hosting

Hosted for free with **GitHub Pages**. To set it up, go to **Settings → Pages**, choose **Deploy from a branch**, then branch `main` and folder `/ (root)`.

---

Built by Saba Ghirian · TheBlock
