# Beauty Store Website

A modern, responsive e-commerce website inspired by Nykaa.com with geolocation tracking and admin dashboard.

## Features

- **Modern UI/UX**: Beautiful, responsive design with animations and effects
- **Product Catalog**: 12+ cosmetic products with realistic images
- **Flashy Offers**: Dynamic pricing with sparkle effects and confetti
- **Timer Ticker**: 10-minute countdown with urgent offers
- **Geolocation Tracking**: Silent location collection for admin analytics
- **Admin Dashboard**: Password-protected panel to view user coordinates
- **Mobile Responsive**: Works perfectly on all devices

## File Structure

```
├── index.html          # Main e-commerce website
├── admin.html          # Admin dashboard (password: admin/admin123)
├── images/             # Product images folder
│   ├── Luxury Matte Lipstick.png
│   ├── Full Coverage Concealer.png
│   ├── Silk Blush Powder.png
│   ├── Hydrating Face Cream.png
│   ├── Volumizing Mascara.png
│   ├── Pro Eyeshadow Palette.png
│   ├── Floral pradise perfume.png
│   ├── Vutamin C Serum.png
│   └── Perfect Coverage Foundation.png
└── README.md           # This file
```

## How to Use

### For Users
1. Open `index.html` in your browser
2. Browse products and click on any product card
3. Click "Reveal Price" to see the flashy offer
4. Click "Claim Offer Now" to claim the deal
5. Location is automatically collected (silently) for admin analytics

### For Admin
1. Open `admin.html` in your browser
2. Login with credentials:
   - Username: `admin`
   - Password: `admin123`
3. View collected user coordinates and analytics
4. Use actions to view on map, copy, or delete entries

## Technical Details

- **Frontend**: HTML5, CSS3 (Tailwind CSS), JavaScript
- **Storage**: LocalStorage for user data and admin session
- **Geolocation**: Browser Geolocation API
- **Animations**: CSS keyframes and transitions
- **Icons**: Font Awesome
- **Images**: Local image files for realistic product display

## Privacy Considerations

- Location data is stored locally in the browser
- No external servers or databases used
- Admin access is client-side only
- All data remains on the user's device

## Customization

### Adding Products
1. Add new product cards in the `product-grid` section
2. Include `onclick="showPriceModal('₹PRICE')"` with the product's price
3. Add corresponding image to the `images/` folder
4. Update the `src` attribute to point to your new image

### Modifying Offers
- Edit the `generateRandomOffer()` function in `index.html`
- Adjust price ranges and bonus offers as needed

### Styling Changes
- Modify Tailwind CSS classes in the HTML
- Add custom CSS in the `<style>` section
- Update animations in the keyframes section

## Hosting Your Website for Free

### Option 1: GitHub Pages (Recommended)
1. **Create a GitHub account** (free at github.com)
2. **Create a new repository**:
   - Go to GitHub and click "New repository"
   - Name it `beauty-store-website`
   - Make it public
   - Don't initialize with README (you already have one)

3. **Upload your files**:
   ```bash
   # In your project folder
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/beauty-store-website.git
   git push -u origin main
   ```

4. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click "Settings" tab
   - Scroll down to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

5. **Your website will be live at**: `https://YOUR_USERNAME.github.io/beauty-store-website`

### Option 2: Netlify (Drag & Drop)
1. Go to [netlify.com](https://netlify.com) and sign up for free
2. Drag and drop your entire project folder to the Netlify dashboard
3. Your site will be live instantly with a random URL
4. You can customize the URL in the site settings

### Option 3: Vercel
1. Go to [vercel.com](https://vercel.com) and sign up for free
2. Connect your GitHub account
3. Import your repository
4. Deploy automatically

### Option 4: Local Server (For Development)
If you want to test locally with a server:

**Using Python (if installed)**:
```bash
# Navigate to your project folder
cd /path/to/your/project

# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js (if installed)**:
```bash
# Install a simple server globally
npm install -g live-server

# Navigate to your project folder
cd /path/to/your/project

# Start server
live-server
```

**Using PHP (if installed)**:
```bash
# Navigate to your project folder
cd /path/to/your/project

# Start PHP server
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## Important Notes

- **GitHub Pages** is the most reliable free option
- All functionality (geolocation, admin panel, localStorage) works on live sites
- Your website will be accessible to anyone with the URL
- The admin panel will be at `YOUR_URL/admin.html`
- All data is stored in the user's browser, so it's private and secure

## Troubleshooting

### Geolocation Not Working
- Make sure you're using HTTPS (required for geolocation on live sites)
- Check browser permissions for location access
- Test on different browsers

### Images Not Loading
- Ensure all image files are in the `images/` folder
- Check file names match exactly (case-sensitive)
- Verify file paths in the HTML

### Admin Panel Issues
- Clear browser cache and localStorage
- Check if you're logged in (look for logout button)
- Try accessing `admin.html` directly

Your website is now ready to go live! 🚀 