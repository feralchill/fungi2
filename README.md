# The Fungi Consultant Website

This is the rebuilt Astro version of The Fungi Consultant website, originally built in Carrd.

## Project Structure

```
/
├── src/
│   ├── components/
│   │   ├── MessageBar.astro    # Rotating message banner at top
│   │   ├── Navigation.astro    # Main navigation menu
│   │   ├── Banner.astro        # Green banner with logo
│   │   └── BottomTab.astro     # Social media tab at bottom
│   ├── layouts/
│   │   └── Layout.astro        # Main layout template
│   └── pages/
│       ├── index.astro         # Homepage
│       ├── about.astro         # About/Services page
│       ├── mushrooms.astro     # Functional Mushrooms page
│       ├── media.astro         # Media page
│       ├── events.astro        # Events page
│       ├── testimonials.astro  # Testimonials page
│       └── booking.astro       # Booking page
```

## Features

- Fixed rotating message bar at the top
- Responsive hamburger navigation menu
- Animated logo banner
- Interactive expandable panels on About page
- Bottom social media tab with scroll integration
- Fully responsive design
- No horizontal scrolling

## Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment to Netlify

### Option 1: Connect Git Repository

1. Push this code to a GitHub repository
2. Go to [Netlify](https://app.netlify.com/)
3. Click "Add new site" → "Import an existing project"
4. Connect your GitHub account and select your repository
5. Build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

### Option 2: Drag and Drop

1. Build the site locally:
   ```bash
   npm run build
   ```
2. Go to [Netlify Drop](https://app.netlify.com/drop)
3. Drag the `dist` folder onto the page

### Option 3: Netlify CLI

1. Install Netlify CLI:
   ```bash
   npm install -g netlify-cli
   ```
2. Build the site:
   ```bash
   npm run build
   ```
3. Deploy:
   ```bash
   netlify deploy --prod --dir=dist
   ```

## Color Palette

- Background: #EFEFED
- Banner: #B6C2A0
- Nav: #4e625c
- Text: #52515c
- Accent Purple: #9A89A4
- Dark: #2C2930

## Fonts

- Abril Fatface (headings, brand name)
- Literata (body text)
- Almendra Display (footer links)

## Assets

All images and videos are hosted on GitHub at:
`https://raw.githubusercontent.com/feralchill/fungi/main/`

## Notes

- The homepage video uses the video1.mov file from the GitHub repo
- Navigation automatically updates "Home" link based on current page
- Bottom tab integrates into footer when scrolled to bottom
- All pages are mobile-responsive
