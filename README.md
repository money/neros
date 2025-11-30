# Grill Americano - Static Website Replica

A static replica of the Grill Americano restaurant website, built with HTML, Tailwind CSS, and vanilla JavaScript.

## Overview

This is a static website replicating the design and structure of https://grillamericano.com. The site features a clean, contemporary aesthetic suitable for a fine dining Italian steakhouse with locations in Melbourne and Sydney.

## Technology Stack

- **HTML5**: Semantic markup
- **Tailwind CSS**: Utility-first CSS framework (via CDN)
- **Vanilla JavaScript**: For interactive elements
- **Google Fonts**: Cormorant Garamond (serif) and Montserrat (sans-serif)

## Project Structure

```
nero/
├── index.html              # Homepage
├── melbourne.html          # Melbourne location page
├── sydney.html             # Sydney location page
├── contact.html            # Contact page
├── reservations.html       # Reservations page
├── menu.html               # Menu page
├── whats-on.html          # What's On page
├── events.html            # Private events page
├── gift-vouchers.html     # Gift vouchers page
├── css/
│   └── styles.css         # Custom CSS
├── js/
│   └── main.js           # JavaScript functionality
├── images/               # Image assets (to be added)
│   ├── logos/
│   ├── hero/
│   ├── food/
│   └── icons/
└── README.md
```

## Features

- **Fully Responsive**: Mobile-first design that works on all devices
- **Modern UI**: Clean, professional aesthetic with neutral color palette
- **Interactive Navigation**: Mobile hamburger menu with smooth transitions
- **Form Validation**: Client-side form validation (visual only, non-functional)
- **Smooth Animations**: Fade-in effects and smooth scrolling
- **SEO Optimized**: Proper meta tags and semantic HTML
- **Accessibility**: ARIA labels and keyboard navigation support

## Setup & Installation

### Quick Start

1. Clone or download this repository
2. Open `index.html` in your web browser

That's it! No build process or dependencies required.

### Local Development Server (Optional)

For a better development experience, you can use a local server:

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js:**
```bash
npx serve
```

Then visit `http://localhost:8000` in your browser.

## Pages

- **Homepage** (`index.html`): Main landing page with location overview
- **Melbourne** (`melbourne.html`): Melbourne location details
- **Sydney** (`sydney.html`): Sydney location details
- **Reservations** (`reservations.html`): Booking form
- **Menu** (`menu.html`): Restaurant menu
- **What's On** (`whats-on.html`): Events and special occasions
- **Events** (`events.html`): Private event inquiries
- **Contact** (`contact.html`): Contact information and form
- **Gift Vouchers** (`gift-vouchers.html`): Gift voucher information

## Customization

### Colors

The site uses a neutral color palette. To customize colors, edit `css/styles.css`.

### Fonts

Current fonts:
- **Serif**: Cormorant Garamond (headings, elegant elements)
- **Sans-serif**: Montserrat (body text, navigation)

To change fonts, update the Google Fonts link in each HTML file.

### Images

Images should be placed in the `images/` directory:
- `images/logos/` - Location logos
- `images/hero/` - Hero section backgrounds
- `images/food/` - Food photography
- `images/icons/` - UI icons

Update image paths in HTML files as needed.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Deployment

This static site can be deployed to:

### GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select branch and root folder

### Netlify
1. Drag and drop project folder to Netlify
2. Or connect GitHub repository for automatic deployments

### Vercel
1. Import project from Git repository
2. Deploy with zero configuration

### Traditional Web Hosting
Upload all files to your web server via FTP/SFTP.

## Features to Note

### Forms
All forms include client-side validation but are non-functional (no backend). To make forms functional:
- Integrate with a form service (Formspree, Netlify Forms, etc.)
- Set up a backend API endpoint
- Update form action attributes

### Mobile Menu
The mobile menu automatically toggles on small screens and closes when:
- User clicks outside the menu
- Window is resized to desktop size
- User selects a navigation item

### Animations
Scroll-based fade-in animations are implemented using Intersection Observer API for performance.

## Contact Information

**Melbourne**
- Address: 112 Flinders Lane, Melbourne VIC 3000
- Phone: 03 8616 8010
- Email: reservations@grillamericano.com

**Sydney**
- Address: No. 1 Chifley Square, Sydney
- Email: reservations@grillamericano.com

**Hours**: Open from 12pm, Monday to Sunday

## Credits

- Original website: https://grillamericano.com
- Brought to you by LUCAS Collective
- This is a static replica for demonstration purposes

## License

This is a replica project created for demonstration purposes. All original branding and content belong to Grill Americano and LUCAS Collective.
