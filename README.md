# Star Flight Simulator - Hyperdrive Edition

A spectacular, cinematic star flight visualization that takes you on a journey through deep space with Hollywood-quality hyperdrive effects.

## Features

- **15,000 Realistic Stars**: Massive starfield with varied colors (white, blue, orange, red) and sizes for depth
- **Smooth Flight Animation**: Experience continuous movement through deep space
- **Cinematic Hyperdrive**: Press 'H' to engage hyperdrive with stunning star-streaking effects
- **Realistic Physics**: Smooth acceleration and deceleration transitions
- **Immersive Camera**: Subtle camera movements for enhanced realism
- **Real-time HUD**: Velocity tracking, star count, and flight mode display

## Tech Stack

- **Three.js (r128)**: Industry-standard 3D graphics library for WebGL
- **WebGL**: Hardware-accelerated rendering for smooth 60fps performance
- **HTML5/CSS3/JavaScript**: Pure web technologies, no build process required

## Usage

### Running Locally

1. Clone the repository
2. Open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari)
3. No build process or dependencies required!

### Controls

- **H Key**: Toggle Hyperdrive mode
  - **Cruise Mode**: Leisurely flight at 2 units/frame
  - **Hyperdrive Mode**: Warp speed at 150 units/frame with star-streaking effects

### Visual Effects

- **Star Colors**: Realistic stellar classification
  - White: Main sequence stars (60%)
  - Blue: Hot stars (20%)
  - Orange: Cooler stars (15%)
  - Red: Red giants (5%)

- **Hyperdrive Effect**: 800 dynamic light streaks that extend and fade based on velocity
- **Additive Blending**: Stars glow and bloom for cinematic quality
- **Depth of Field**: Size attenuation for realistic distance perception

## Performance

- Optimized for 60fps on modern hardware
- 15,000+ particles rendered simultaneously
- Efficient geometry updates using buffer attributes
- Hardware-accelerated WebGL rendering

## Browser Compatibility

- Chrome/Edge (recommended)
- Firefox
- Safari
- Any modern browser with WebGL support

## Technical Details

- **Particle System**: BufferGeometry with custom attributes for color and size
- **Streak System**: Dynamic line geometry with real-time position updates
- **Animation Loop**: RequestAnimationFrame for smooth 60fps rendering
- **Spatial Wrapping**: Infinite flight experience with seamless star recycling

## Customization

Edit the constants in `index.html` to customize the experience:

```javascript
const STAR_COUNT = 15000;      // Number of stars
const SPACE_SIZE = 2000;       // Size of the space volume
const CRUISE_SPEED = 2;        // Normal flight speed
const HYPERDRIVE_SPEED = 150;  // Hyperdrive speed
```

## License

Open source - feel free to use and modify!

## Credits

Built with Three.js - https://threejs.org
