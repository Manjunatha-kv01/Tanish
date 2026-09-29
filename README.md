<<<<<<< HEAD
# ✨ Naming Ceremony Invitation ✨

An interactive, responsive digital invitation single-page web application designed for the **Baby Naming Ceremony** of **Chaitra & Chethan**.

---

## 🌟 Key Features

* **💌 Envelope & Splash Screen Reveal**:
  * Elegant dark blue & gold themed envelope landing screen.
  * Real-time canvas chroma keying / checkerboard removal engine for animated baby video with a graceful animated star & halo canvas fallback.
  * Smooth opening animation revealing the invitation.
* **⏳ 3D Flip Card Countdown Timer**:
  * Real-time countdown tracking days, hours, minutes, and seconds to the ceremony (**October 25, 2026 at 11:10 AM**).
  * 3D perspective card fold animation.
* **🎵 Background Soundtrack with Floating Controls**:
  * Auto-starts upon opening the envelope (`gulabi.mp3`).
  * Floating audio toggle button with mute/unmute visual states (🔊 / 🔇).
* **🌸 Falling Flower Petals Particle Effect**:
  * Procedurally generated falling blossoms (`🌸`, `🌺`, `🌼`, `✿`, `🌷`) across the screen with randomized trajectories and timings.
* **📑 Sticky Tabbed Navigation**:
  1. **Schedule**: Detailed order of events and ceremony timeline.
  2. **Venue**: Kalyana Mantapa details, photo, and direct Google Maps navigation button.
  3. **Gallery**: Responsive grid showcasing ceremony photos with interactive full-screen **Lightbox** supporting keyboard navigation (`←`, `→`, `Escape`).
  4. **RSVP & Blessings**: Interactive guest form with character counter and EmailJS integration.

---

## 📁 Project Structure

```text
wedding-invitation-main/
├── .vscode/
│   └── settings.json          # Live Server port configuration (Port 5501)
├── GGGG.png                   # Ceremony card graphic
├── G.png                      # Supplementary illustration asset
├── guru.jpg                   # Venue image (Sri Swarna Gowri Kalyana Mantapa)
├── gulabi.mp3                 # Background soundtrack
├── index.html                 # Complete SPA (HTML5, CSS3, JavaScript)
├── ma.jpg                     # Hero section background cover photo
├── ma0.jpg                    # Gallery image 1
├── ma1.jpeg                   # Gallery image 2
├── ma2.jpeg                   # Gallery image 3
├── ma3.jpg                    # Gallery image 4
├── ma4.jpg                    # Gallery image 5
└── README.md                  # Project documentation
```

---

## 🚀 Quick Start / Local Development

No build tools or Node.js required! You can run the application directly in any modern browser:

### Option 1: VS Code Live Server (Recommended)
1. Open the project folder in **Visual Studio Code**.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click [`index.html`](index.html) and select **"Open with Live Server"** (or click "Go Live" in the status bar at port `5501`).

### Option 2: Python Simple HTTP Server
Open your terminal in the project root directory and run:
```bash
python3 -m http.server 5501
```
Then visit `http://localhost:5501` in your browser.

---

## ⚙️ Customization Guide

### 1. Configure RSVP / EmailJS Integration
To receive RSVP messages and blessings directly in your inbox:
1. Create a free account at [EmailJS](https://www.emailjs.com/).
2. Create an **Email Service** (e.g. Gmail) and an **Email Template** with variables: `{{from_name}}`, `{{message}}`, `{{ceremony}}`, `{{guest_name}}`, `{{submitted_at}}`.
3. Open [`index.html`](index.html) and update lines 673–675 with your credentials:
   ```javascript
   const EMAILJS_PUBLIC_KEY = "YOUR_EMAILJS_PUBLIC_KEY";
   const EMAILJS_SERVICE_ID = "YOUR_SERVICE_ID";
   const EMAILJS_TEMPLATE_ID = "YOUR_TEMPLATE_ID";
   ```
*(Note: If left unconfigured, the form runs in demonstration mode and gracefully logs a helpful notice in the browser console while showing the guest a success confirmation).*

### 2. Update Ceremony Date & Time
To adjust the countdown timer target, edit line 789 in [`index.html`](index.html):
```javascript
const EVENT_DATE = new Date('2026-10-25T11:10:00+05:30');
```

### 3. Update Gallery Images
To add or modify photos displayed in the gallery tab and lightbox, update the `GALLERY_IMAGES` array in [`index.html`](index.html):
```javascript
const GALLERY_IMAGES = [
    { src: 'ma0.jpg',  caption: 'Our Story — Chapter One'   },
    { src: 'ma1.jpeg', caption: 'Our Story — Chapter Two'   },
    { src: 'ma2.jpeg', caption: 'Family Moment Three'       },
    { src: 'ma3.jpg',  caption: 'Our Story — Chapter Four'  },
    { src: 'ma4.jpg',  caption: 'Our Story — Chapter Five'  },
];
```

### 4. Update Venue & Location Link
To update the venue address or Google Maps destination, edit the venue tab section in [`index.html`](index.html):
```html
<a href="https://your-google-maps-link" target="_blank" rel="noopener noreferrer" class="map-btn">
    Open Google Maps
</a>
```

---

## 💻 Tech Stack

* **HTML5**: Semantic document layout and media elements (`<audio>`, `<video>`, `<canvas>`).
* **CSS3**: Custom CSS variables, Glassmorphism backdrop filters, 3D perspective transforms, CSS Grid & Flexbox, responsive `@media` breakpoints.
* **JavaScript (ES6+)**: `IntersectionObserver`, `requestAnimationFrame`, Canvas 2D image data manipulation, HTML Audio API, and asynchronous Fetch/EmailJS APIs.
* **Typography**: Google Fonts ([Cinzel](https://fonts.google.com/specimen/Cinzel), [Montserrat](https://fonts.google.com/specimen/Montserrat), [Great Vibes](https://fonts.google.com/specimen/Great+Vibes)).

---

## 👤 Author & Credits

* **Author**: Adarsh VD / Manjunath KV
* **Event**: Baby Naming Ceremony — Chaitra & Chethan
=======
# Tanish
my world
>>>>>>> 768a7e76c5c4fe8e67af1dbe66e10d11fb5f8e02
