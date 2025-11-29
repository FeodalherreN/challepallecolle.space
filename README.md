# Chantal Palm - Palms Collections

A minimalist portfolio website for contemporary artist Chantal Palm, showcasing her graffiti-style paintings with a sophisticated aesthetic.

## Tech Stack

- **Astro** v5.0+ - Static site generator
- **Tailwind CSS** v4.0+ - Utility-first CSS framework (using new Vite plugin)
- **TypeScript** - Type safety

## Project Structure

```
/
├── public/
│   └── logos/
│       └── logo-rad.png          # Main logo
├── src/
│   ├── layouts/
│   │   └── Layout.astro          # Base layout with SEO
│   ├── pages/
│   │   ├── index.astro           # Home page (landing)
│   │   ├── store.astro           # Available collection gallery
│   │   ├── coming-soon.astro     # Upcoming pieces (blurred)
│   │   └── contact.astro         # Contact information
│   └── env.d.ts
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

## Setup

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Add your logo:**
   - Place `logo-rad.png` in `public/logos/`

3. **Add collection images:**
   - Create `public/collection/` directory
   - Add painting images for store and coming-soon pages
   - Update the arrays in `store.astro` and `coming-soon.astro` with your actual images

4. **Run development server:**
   ```bash
   npm run dev
   ```

5. **Build for production:**
   ```bash
   npm run build
   ```

## Adding Collection Items

### Store (Available Pieces)

Edit `src/pages/store.astro`:

```javascript
const availableCollection = [
  {
    id: 1,
    title: "Your Painting Title",
    image: "/collection/painting-1.jpg",
    price: "Available" // or actual price
  },
  // Add more items...
];
```

### Coming Soon (Upcoming Pieces)

Edit `src/pages/coming-soon.astro`:

```javascript
const upcomingCollection = [
  {
    id: 1,
    title: "Upcoming Piece Title",
    image: "/collection/upcoming-1.jpg"
  },
  // Add more items...
];
```

## Customization

### Contact Information

Update email and other details in `src/pages/contact.astro`

### SEO & Meta Tags

All pages have proper SEO setup. Update site-wide description in `src/layouts/Layout.astro`

### Styling

- Global styles in `src/layouts/Layout.astro`
- Tailwind config in `tailwind.config.mjs`
- Custom CSS in individual `.astro` files

## Features

✨ **Minimalist Design** - Clean, distraction-free interface
📱 **Fully Responsive** - Mobile and desktop optimized
🎨 **Gallery Views** - Elegant grid layouts for collections
😶‍🌫️ **Blur Effect** - Coming soon items have blur overlay
🔍 **SEO Optimized** - Meta tags, Open Graph, proper semantics
⚡ **Fast Performance** - Static site generation with Astro
🎯 **Accessible** - Semantic HTML and ARIA labels

## Author

Built by Markus Olsson for Chantal Palm / Palms Collections

## License

All rights reserved - Chantal Palm © 2023
