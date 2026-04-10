# Menu Card

A polished digital restaurant menu built as a single-page HTML app. The `menu-card` project lets restaurant owners customize menu items, branding, categories, themes, and sharing options from an admin panel — then display a beautiful public menu for guests.

## Features

- **Public menu interface** with hero section, category navigation, item cards, and detail-rich presentation
- **Admin panel** protected by a password to manage menu content and display settings
- **Menu item management**
  - Add, edit, delete items
  - Multiple price options per item
  - Item imagery and descriptions
  - Badge labels and searchable tags
  - Vegetarian / non-vegetarian / other item types
  - Out-of-stock item marking
- **Category management**
  - Parent and subcategory support
  - Drag-free category renaming and removal
  - Category-based admin filtering for easier menu maintenance
- **Branding customization**
  - Restaurant name and tagline
  - Hero title, subtitle, and image
  - Hours, phone, and address display
  - Browser tab title and favicon support
- **Theme switching**
  - Dark, light, neon, blush, and midnight visual themes
- **Share tools**
  - Optional WhatsApp share button with customizable message
  - Optional QR code generator and download button
- **Feature toggles**
  - Announcement banner
  - Table number input field
  - Social links in footer
  - Powered-by footer toggle
- **Location & external links**
  - Footer location strip with Google Maps directions button
  - Embedded Google Maps preview in footer
  - Delivery platform buttons (Swiggy, Zomato, Magicpin, Dunzo, Blinkit)
  - Dine-in/reservation app buttons (District, Dineout, EazyDiner, OpenTable)
  - Configurable button placement and style
- **Import / export**
  - Export the menu data as JSON
  - Import menu configuration from JSON
- **Local storage persistence** for menu data, theme, and admin config
- **Firebase Realtime Database sync** optional for live updates across devices

## Getting Started

### Opening the app

1. Open `index.html` directly in a browser.
2. The app is fully client-side and does not require a build tool or server.

### Admin access

- Click `Admin` in the top-right of the public menu.
- Default password: `admin123`
- After login, the admin panel opens with tabs for items, categories, branding, themes, links & location, and settings.

## Admin Panel Details

### Menu Items
- Add or edit item details, pricing options, image URL, tags, and availability.
- Change category assignment from any parent/subcategory selection.

### Categories
- Create parent categories and add child subcategories.
- Rename categories directly.
- Remove categories when they are no longer needed.

### Branding
- Customize your restaurant name, tagline, hero text, image, hours, phone, and address.
- Set the browser tab title and favicon URL for the public menu.

### Themes
- Switch between five predefined visual themes instantly.

### Links & Location
- Configure the footer location strip with Google Maps directions and optional embedded map preview.
- Add delivery platform buttons for Swiggy, Zomato, Magicpin, Dunzo, Blinkit, and custom URLs.
- Add dine-in/reservation apps such as District, Dineout, EazyDiner, OpenTable, or custom links.
- Choose whether order/reserve buttons appear in the footer, share bar, or both.

### Settings
- Optional Firebase config for real-time database syncing.
- Change the admin password.
- Toggle share, QR, banner, table input, social links, and footer branding features.
- Customize WhatsApp share text, QR code appearance, and announcement banner content.
- Export menu configuration as JSON or import a saved menu file.
- Reset all data to the default demo state.

## Firebase Sync

The app includes optional Firebase Realtime Database support.

1. In the `Settings` tab, paste your Firebase configuration fields.
2. Click `Connect Firebase`.
3. Menu data will sync live across connected clients.

> The app also contains a hardcoded Firebase configuration for demo usage if available.

## Customization Notes

- Hero titles support line breaks with `|`.
- WhatsApp share text supports placeholders:
  - `{url}` — current menu URL
  - `{name}` — restaurant name
  - `{table}` — table number if table input is enabled
- QR Code modal uses the current URL by default, or a custom URL if provided.

## Technical Details

- Single file app: `index.html`
- Uses `localStorage` for local persistence
- Uses `sessionStorage` for current menu filter and table number
- Includes Firebase compatibility libraries and QRCode.js
- Uses inline CSS and JavaScript for quick deployment

## Recommended Usage

- Deploy `index.html` to GitHub Pages, a static web host, or any web server.
- Use the admin panel to customize your menu before sharing the public URL.
- Use JSON export to back up your menu data or move it to another installation.

## License

This repository is provided as-is for customization and deployment.
