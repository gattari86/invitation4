# Jane & Joe - Interactive 3D Card Flip Wedding Invitation

A stunning monochrome wedding invitation featuring an envelope opening animation followed by an interactive 3D card flip experience.

## Features

- 🎭 **Envelope Opening Animation**: Elegant 4-5 second entrance sequence
- 🔄 **3D Card Flip**: Click, tap, or swipe to flip the card and reveal event details
- 🎨 **Sophisticated Monochrome Palette**: Elegant grayscale design with metallic accents
- ✨ **Glassmorphism Effects**: Modern frosted glass aesthetic
- 📱 **Mobile-Friendly**: Touch gestures and responsive design
- ⌨️ **Accessible**: Keyboard navigation support (Enter/Space to flip)
- 💎 **Premium Design Resources**:
  - Heroicons (292 beautiful SVG icons)
  - Animate.css (entrance animations)
  - Google Fonts (Cormorant Garamond, Great Vibes, Montserrat)

## Color Palette

The template uses an elegant monochrome color scheme:

- **#161616** - Near Black (primary backgrounds)
- **#8A8A8A** - Medium Gray (borders, accents)
- **#A5A5A5** - Light Gray (text highlights)
- **#1C1C1C** - Dark Charcoal (secondary backgrounds)
- **#4C4646** - Warm Dark Gray (subtle warmth)

Plus metallic gradients:
- **Silver**: Linear gradient for elegant text effects
- **Chrome**: High-contrast gradient for primary headings

## Event Details

- **Date**: July 12, 2026
- **Venue**: Sandals Royal Caribbean, Montego Bay, Jamaica
- **Ceremony**: 4:00 PM - Beachfront Gazebo
- **Cocktail Hour**: 5:30 PM - Sunset Terrace
- **Reception**: 7:00 PM - Oceanview Pavilion
- **After Party**: 10:00 PM - Beach Bar

## How It Works

1. **Page Load**: Envelope animation plays automatically (4-5 seconds)
2. **Card Reveal**: After envelope opens, the 3D card appears
3. **Front Side**: Displays couple names and wedding date in metallic chrome text
4. **Back Side**: Shows complete event details with elegant icons
5. **Interaction**:
   - **Desktop**: Click the card to flip
   - **Mobile**: Tap or swipe the card
   - **Keyboard**: Press Enter or Space

## Local Development

Simply open `index.html` in your browser. No build process required!

## Deployment

### Deploy to Vercel

1. Push to GitHub
2. Import repository in Vercel
3. Deploy automatically

The `vercel.json` is pre-configured with the correct settings to serve all static assets.

## Project Structure

```
wedding-invitation-3d-flip/
├── assets/
│   ├── images/
│   │   ├── hero-bg.jpg
│   │   ├── attire.jpg
│   │   ├── welcome-background.jpg
│   │   ├── family/
│   │   │   ├── 1.jpg
│   │   │   ├── 2.jpg
│   │   │   └── 3.jpg
│   │   └── resort/
│   │       ├── 1.jpg
│   │       ├── 2.jpg
│   │       └── 3.jpg
│   └── audio/
│       └── background-music.mp3
├── index.html
├── vercel.json
├── .gitignore
└── README.md
```

## Design Resources Used

- **Icons**: Heroicons (292 hand-crafted SVG icons from Tailwind CSS creators)
- **Animations**: Animate.css (80+ cross-browser animations)
- **Fonts**: Google Fonts (Cormorant Garamond, Great Vibes, Montserrat)
- **3D Effects**: Native CSS 3D transforms (`perspective`, `rotateY`, `preserve-3d`)

## Technical Highlights

### 3D Card Flip Implementation

```css
.card-3d {
    transform-style: preserve-3d;
    transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.card-3d.flipped {
    transform: rotateY(180deg);
}

.card-face {
    backface-visibility: hidden;
}

.card-back {
    transform: rotateY(180deg);
}
```

### Metallic Text Effects

```css
.front-names {
    background: linear-gradient(135deg, #A5A5A5 0%, #FFFFFF 50%, #A5A5A5 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
```

### Glassmorphism

```css
.card-front {
    background: linear-gradient(135deg,
        rgba(22, 22, 22, 0.95) 0%,
        rgba(76, 70, 70, 0.95) 50%,
        rgba(28, 28, 28, 0.95) 100%
    );
    backdrop-filter: blur(20px);
}
```

## Mobile Optimization

- Touch gesture support (swipe to flip)
- Responsive font sizes and spacing
- Optimized card dimensions for small screens
- Reduced animation complexity on mobile devices
- Fast loading with optimized assets

## Accessibility Features

- Keyboard navigation (Enter/Space to flip card)
- Reduced motion support for users with motion sensitivity
- High contrast text and backgrounds
- Semantic HTML structure
- ARIA labels and roles

## Credits

Monochrome 3D card flip wedding invitation template
Design inspired by sophisticated editorial design and premium metallic finishes
Perfect for elegant, modern weddings with a minimalist aesthetic

---

**#JaneAndJoe2026** 💍✨
