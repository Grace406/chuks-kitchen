# Chuks Kitchen 🍛

## Project Overview
Chuks Kitchen is a responsive frontend web project for a Nigerian food ordering platform. It consists of three pages: an Onboarding/Welcome page, a Sign In page, and a Home page. The project was built by translating Figma UI designs into clean, structured HTML and CSS code.

The platform represents a food ordering service that brings authentic Nigerian home cooking to customers, allowing them to browse meals, sign in to their accounts, and place orders.

## Tech Stack
- **HTML5** — for page structure and semantic markup
- **CSS3** — for styling, layout and responsiveness
- **Google Fonts** — Inter, Roboto, Jost, Poppins and Island Moments for typography
- **Flexbox & CSS Grid** — for layout management
- **CSS Media Queries** — for responsive design (mobile-first approach, desktop breakpoint at min-width: 1024px)

No frameworks or JavaScript libraries were used. The decision to use vanilla HTML and CSS was intentional to keep the project lightweight and demonstrate core frontend fundamentals.

## Project Structure
```
chuks-kitchen/
├── Onboarding_design/
│   ├── assets/          # Images and icons for onboarding page
│   ├── onboarding.html  # Welcome/onboarding page
│   └── onboarding.css   # Styles for onboarding page
│
├── Sign-in_design/
│   ├── assets/          # Images and icons for sign in page
│   ├── sign-in.html     # Sign in page
│   └── sign-in.css      # Styles for sign in page
│
└── Home_design/
    ├── assets/          # Images and icons for home page
    ├── home.html        # Home page
    └── home.css         # Styles for home page
```

## Design Interpretation
The Figma designs were translated into code using the following approach:

- **Mobile-first** — all base styles were written for mobile screens first, then desktop styles were added using `@media (min-width: 1024px)`
- **Onboarding Page** — the design shows a two-column layout on desktop with the hero image on the left and content on the right. On mobile it stacks vertically with a full-width hero image and scrollable content below
- **Sign In Page** — on desktop the page shows a two-column card with a hero image and orange overlay on the left and the login form on the right. On mobile only the form is shown, the hero image is hidden
- **Home Page** — the desktop layout features a full-width hero, a 3x2 grid for both Popular Categories and Chef's Specials sections. On mobile these display as single-column stacked cards. Three extra cards in each section are hidden on mobile and revealed on desktop using a `desktop-only` CSS class

**Assumptions made due to missing design details:**
- Footer was hidden on mobile and only shown on desktop as the Figma mobile designs did not include it
- The `desktop-only` category and specials cards use placeholder images since the Figma design only specified the desktop layout

## How to Run
1. Clone or download the repository at https://github.com/Grace406/chuks-kitchen
2. Open any of the following files in your browser:
   - `Onboarding_design/onboarding.html`
   - `Sign-in_design/sign-in.html`
   - `Home_design/home.html`

No installations or dependencies required. All pages work directly in any modern browser.

## Live Preview
- 👋 Onboarding Page: https://marvelous-alfajores-4d6ab9.netlify.app/onboarding.html
- 🔐 Sign In Page: [add link here]
- 🏠 Home Page: https://inquisitive-biscuit-af97db.netlify.app

## Limitations & Improvements
Given more time, the following improvements would be made:

- **Page linking** — connect all 3 pages together so buttons like "Get Started", "Continue" and "Login" navigate between pages
- **JavaScript interactivity** — add form validation on the sign in page, a working search bar on the home page and a functional cart system
- **More pages** — build out the Explore, My Orders and Account pages referenced in the navigation
- **Animations** — add subtle transitions and hover effects to buttons and cards for a more polished feel
- **Accessibility** — improve ARIA labels, keyboard navigation and color contrast across all pages
- **Performance** — optimize images for faster load times
