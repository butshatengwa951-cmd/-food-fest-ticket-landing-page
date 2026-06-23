# Cape Town Food Fest - Ticket Tier Landing Page

## Overview

Cape Town Food Fest is an annual outdoor food festival that brings together top chefs, street food vendors, artisans, and live musicians for a weekend of food, entertainment, and community celebration.

This project is a modern, interactive Vue 3 landing page designed to showcase the festival's ticket tiers: **Bronze**, **Silver**, and **Gold**. The page allows potential attendees to compare pricing, benefits, and ticket options before purchasing.

Built as the foundation for a future ticketing platform, the application includes simulated e-commerce interactions such as favourites tracking, featured tier promotion, and theme customization.

---

## Key Features

### Reusable Component Architecture

* Ticket tiers are rendered using reusable `TicketCard` components.
* Easy to extend with additional ticket types or event packages.

### Featured Tier Highlight

* Gold tier receives special visual treatment.
* Neon glow effects and a **"Most Popular"** badge help draw user attention.

### Interactive Favourites

* Users can favourite ticket tiers using a heart icon.
* Live favourite count updates instantly for each tier.

### Responsive Design

* Mobile-first layout.
* Ticket cards stack vertically on smaller screens.
* Three-column grid layout on larger desktop displays.

### Festival-Themed UI

* Dark mode styling inspired by concerts and festivals.
* Neon accent colours and immersive hero imagery.

### Theme Toggle

* Switch between dark and light themes.
* Smooth transitions for an enhanced user experience.

### Local Data Storage

* Ticket information is stored directly within the application.
* No backend or database required for the current version.

---

## Tech Stack

### Frontend

* Vue 3
* Composition API
* `<script setup>`

### Tooling

* Vite

### Styling

* CSS Variables
* Custom CSS Animations
* Responsive Grid Layouts

### Additional Notes

* No Vue Router
* No external UI frameworks or plugins
* Lightweight single-page architecture

---

## Installation & Setup

### Prerequisites

Ensure the following software is installed:

* Node.js v18 or higher
* npm or Yarn

Check your installation:

```bash
node -v
npm -v
```

---

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd cape-town-food-fest
```

---

## 2. Install Dependencies

```bash
npm install
```

Or with Yarn:

```bash
yarn install
```

---

## 3. Run the Development Server

Start the local development environment:

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:5173
```

---

## 4. Build for Production

Generate an optimized production build:

```bash
npm run build
```

Compiled files will be placed in the `dist/` directory.

---

## 5. Preview Production Build

Preview the production build locally:

```bash
npm run preview
```

---

## Project Structure

```text
src/
├── assets/
│   ├── base.css
│   │   └── CSS variables, theme settings, and resets
│   │
│   └── main.css
│       └── Hero section, grid layouts, and page styling
│
├── components/
│   └── TicketCard.vue
│       └── Reusable ticket tier component
│
├── App.vue
│   └── Main landing page and ticket tier data
│
└── main.js
    └── Application entry point
```

---

## Configuration Notes

### Ticket Data

All ticket information is currently stored locally within:

```text
src/App.vue
```

Modify the ticket array to:

* Add new ticket tiers
* Update pricing
* Change benefits and descriptions

### Theme Customization

Theme colours are managed through CSS variables located in:

```text
src/assets/base.css
```

You can easily customize:

* Background colours
* Accent colours
* Neon glow effects
* Typography styling

### Favourite System

The favourites feature is currently stored in application state only.

This means:

* Counts update instantly while using the app.
* Favourite selections reset when the page is refreshed.

---

## Future Enhancements

Potential improvements include:

* Integrating a backend API for live ticket data
* Connecting "Get Tickets" buttons to a checkout system
* Adding sorting by price or popularity
* Tier filtering and search functionality
* Persisting favourites using Local Storage
* User accounts and authentication
* Real-time ticket availability tracking
* Event schedule and performer integration

---

## Development Commands

### Start Development Server

```bash
npm run dev
```

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

---

## License

This project was created for educational and portfolio purposes as part of the Cape Town Food Fest marketing initiative.

**Built for the Cape Town Food Fest Marketing Team — June 2026.**

