# ApeFest 2025 UFO Redemption Experience 🛸

A premium, UFO-themed landing page for ApeFest 2025 redemption codes featuring smooth animations, tractor beam effects, and an exclusive experience for BAYC attendees.

## Features

- **Interactive UFO**: Click to activate the transmission
- **Power-Up Effects**: Multi-layered purple glow when activated
- **Tractor Beam**: Yellow-green gradient beam with floating particles
- **Code Levitation**: Redemption code floats up through the beam
- **Copy to Clipboard**: One-click code copying with visual feedback
- **Mobile Responsive**: Optimized for all screen sizes
- **100 Twinkling Stars**: Dynamic starfield background
- **Smooth Animations**: Premium CSS animations throughout

## Quick Start

Simply open `index.html` in any modern web browser. Your images are already integrated from the `assets/` folder!

## Project Structure

```
apefest redemption/
├── index.html              # Main landing page (references assets folder)
├── assets/                 # Image assets folder
│   ├── ape-ufo.png        # Your UFO image
│   ├── apefest-background.png  # Your background image
│   └── HOW_TO_ADD_UFO_IMAGE.txt
└── README.md              # This file
```

## Customization

### Change Redemption Code or URL

Edit the `CONFIG` object in the JavaScript section of `index.html`:

```javascript
const CONFIG = {
    redemptionCode: 'APES-2025-UFO',    // Change your code here
    redeemUrl: 'https://op.xyz/your-badge-link',  // Update redeem link
    numberOfStars: 100                   // Adjust star count
};
```

### Use Background Image

To use your custom background image instead of the gradient, update the CSS in `index.html`:

Replace:
```css
background: linear-gradient(180deg, #0a0e27 0%, #1a1a3e 50%, #0f0f1e 100%);
```

With:
```css
background: url('./assets/apefest-background.png') center/cover no-repeat;
```

## How It Works

1. **User clicks the UFO** anywhere on the image
2. **UFO powers up** with enhanced glow effects (0.5s)
3. **Tractor beam activates** from bottom with particles (0.5s)
4. **Status text updates** from "INITIATING TRANSMISSION..." to "TRANSMISSION RECEIVED"
5. **Code levitates** up through the beam over 2 seconds
6. **Buttons appear** for copying and redeeming the code

## Animation Timing

- UFO power-up: 0.5s
- Beam activation: 0.5s (starts after UFO power-up)
- Code levitation: 2s (starts with beam)
- Buttons fade-in: 1s (starts 2s after beam activation)

## Mobile Responsiveness

- **Desktop**: 400x400px UFO, side-by-side buttons
- **Mobile** (≤600px): 300x300px UFO, stacked buttons
- Optimized touch targets and spacing

## Design Specs

- **Background**: Deep space gradient or custom image
- **UFO Size**: 400x400px (300x300px on mobile)
- **Theme Color**: Purple (#c084fc)
- **Beam Color**: Yellow-green (rgba(190, 242, 100))
- **Font**: Courier New (monospace)
- **Animations**: 60fps CSS transitions and keyframes

## Browser Support

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Technical Details

- **File Type**: Single-page HTML with inline CSS and JavaScript
- **Dependencies**: None (completely self-contained)
- **Image Format**: PNG files referenced from assets folder
- **Copy Function**: Uses navigator.clipboard API

## Tips

- For best performance, optimize images before adding them to the assets folder
- The page works offline once loaded
- All animations are hardware-accelerated for smooth performance
- The UFO image should ideally have a transparent background

---

**Built for ApeFest 2025** 🦍✨

*Premium tech-forward UFO redemption experience for BAYC community*
