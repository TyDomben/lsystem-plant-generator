# 🌿 L-System Plant Generator

A beautiful, interactive web application for generating organic plant structures using Lindenmayer Systems (L-Systems). Watch mathematical rules create stunning natural patterns!

## ✨ Features

### L-System Implementation
- **Proper L-system parser** with support for:
  - `F` - Draw forward
  - `+` / `-` - Rotate right/left
  - `[` / `]` - Push/pop state (branching)
  - `A`, `B` - Additional variables for complex rules
- **Multiple iterations** (1-8 generations)
- **Stochastic variations** for organic randomness

### Plant Presets
6 beautiful pre-configured plant types:
1. **Fern** - Classic Barnsley fern with intricate fronds
2. **Binary Tree** - Symmetric fractal tree structure
3. **Algae** - Simple Lindenmayer's original growth pattern
4. **Bush** - Dense, shrub-like branching
5. **Flower** - Radial symmetry pattern
6. **Vine** - Climbing, trailing growth

### Interactive Controls
- **Angle Slider** (5-180°) - Control branching angles
- **Iterations Slider** (1-8) - Adjust growth depth/complexity
- **Length Slider** (2-30) - Modify segment lengths
- **Randomness Slider** (0-100) - Add natural variation
- **Tapered Branches** - Toggle realistic thickness variation
- **Growth Animation** - Watch plants grow step-by-step

### Visualization
- **2D Rendering** with p5.js
- **Green gradients** from light to dark (depth-based)
- **Smooth anti-aliased lines**
- **Multiple backgrounds**: White, Black, or Gradient
- **Efficient rendering** handles 1000+ line segments

### Export Options
- **PNG Download** - High-quality raster image
- **SVG Export** - Vector graphics for laser cutting/plotting
- **Share Links** - URL-encoded parameters to share configurations

### Educational Features
- **Live L-System Rules Display** - See axiom and production rules
- **Symbol Legend** - Understand the L-system grammar
- **Responsive Design** - Beautiful UI with Tailwind CSS

## 🚀 Quick Start

Simply open `index.html` in a modern web browser - no build process required!

```bash
# Clone and open
git clone <repository-url>
cd lsystem-plant-generator
open index.html  # macOS
# or
xdg-open index.html  # Linux
# or just double-click index.html on Windows
```

## 🎨 How to Use

1. **Choose a Preset** - Click any of the 6 plant buttons
2. **Adjust Parameters** - Use sliders to modify angle, iterations, length, and randomness
3. **Customize Appearance** - Toggle tapered branches and select background color
4. **Animate Growth** - Click "Play Growth" to watch the plant develop
5. **Export** - Download as PNG/SVG or copy a shareable link

## 🔬 Understanding L-Systems

L-Systems (Lindenmayer Systems) are parallel rewriting systems developed by Aristid Lindenmayer in 1968 to model plant growth. They work by:

1. Starting with an **axiom** (initial string)
2. Applying **production rules** repeatedly
3. Interpreting the final string as drawing commands

### Example: Binary Tree
```
Axiom: F
Rule: F → FF+[+F-F-F]-[-F+F+F]
Angle: 22.5°

Generation 0: F
Generation 1: FF+[+F-F-F]-[-F+F+F]
Generation 2: [Much longer string creating branching pattern]
```

## 🛠️ Technical Details

- **Framework**: Vanilla JavaScript with p5.js for rendering
- **Styling**: Tailwind CSS for responsive UI
- **Libraries**:
  - p5.js v1.7.0 (2D graphics)
  - Tailwind CSS (styling)
- **No build process** - Single HTML file with CDN resources
- **Browser compatibility** - Modern browsers (Chrome, Firefox, Safari, Edge)

## 📚 L-System Resources

- [Wikipedia: L-System](https://en.wikipedia.org/wiki/L-system)
- [The Algorithmic Beauty of Plants](http://algorithmicbotany.org/papers/#abop)
- [L-Systems in p5.js](https://p5js.org/examples/simulate-l-systems.html)

## 🎯 Future Enhancements

Potential additions:
- 3D rendering with WEBGL or Three.js
- More plant presets (trees, flowers, fractals)
- Custom rule editor
- Color customization
- Leaf/flower decorations at branch tips
- Multiple L-systems on one canvas

## 📄 License

Open source - feel free to use, modify, and share!

## 🌟 Examples

Try these configurations:

**Majestic Oak**
- Preset: Binary Tree
- Angle: 30°
- Iterations: 5
- Length: 8
- Randomness: 15
- Tapered: On

**Delicate Fern**
- Preset: Fern
- Angle: 25°
- Iterations: 5
- Length: 10
- Randomness: 5
- Tapered: On

**Abstract Flower**
- Preset: Flower
- Angle: 60°
- Iterations: 6
- Length: 12
- Randomness: 0
- Tapered: Off

---

Made with 🌱 and mathematical beauty
