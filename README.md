# 🚗 Vehicle Maintenance Tracker

A Progressive Web App (PWA) for tracking your vehicle's maintenance and service history. Works offline and can be installed on your iPhone home screen!

## Features

- ✅ Track maintenance, repairs, and inspections
- 💰 Monitor service costs and spending
- 📊 View statistics and filter by service type
- 📱 Mobile-first design optimized for iPhone
- 🔄 Works offline after first visit
- 🏠 Installable as a home screen app
- 💾 All data stored locally on your device

## Setup Instructions for GitHub Pages

### 1. File Structure
Create these files in your repository:

```
your-repo/
├── index.html          (main app file)
├── manifest.json       (PWA configuration)
├── sw.js              (service worker)
├── icon-192.png       (app icon - small)
├── icon-512.png       (app icon - large)
└── README.md          (this file)
```

### 2. Generate Icons

1. Open `icon-generator.html` in your browser
2. Click the download buttons to get both icon sizes
3. Save them as `icon-192.png` and `icon-512.png`
4. Add them to your repository

**Alternative:** Use any image editor to create icons with your preferred design. Recommended specs:
- 192x192px for the small icon
- 512x512px for the large icon
- PNG format with transparent or solid background

### 3. Enable GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" section
3. Under "Source", select your main branch
4. Click "Save"
5. Your app will be live at: `https://yourusername.github.io/your-repo-name/`

### 4. Update Paths (if needed)

If your app is in a subdirectory, update these paths in your files:

**In manifest.json:**
```json
"start_url": "/your-repo-name/",
```

**In sw.js:**
```javascript
const urlsToCache = [
  '/your-repo-name/',
  '/your-repo-name/index.html',
  // ... etc
];
```

**In index.html:**
```html
<link rel="manifest" href="/your-repo-name/manifest.json">
```

## Installing on iPhone

1. Open the app in Safari (not Chrome)
2. Tap the Share button (square with arrow)
3. Scroll and tap "Add to Home Screen"
4. Customize the name if desired
5. Tap "Add"

The app will now appear on your home screen with a custom icon!

## Usage Tips

- **Add Entry**: Tap the purple + button in the bottom right
- **Filter Logs**: Use the filter buttons (All, Maintenance, Repair, Inspection)
- **Delete Entry**: Tap the × button on any log entry
- **Track Costs**: Add optional costs to see your total spending
- **Offline Access**: The app works without internet after first load

## Data Storage

- All data is stored locally in your browser's localStorage
- Data persists across sessions
- No data is sent to any server
- To backup data, consider screenshotting or manually exporting

## Customization Ideas

- Change the color scheme in the CSS
- Add more service types
- Include vehicle details (make, model, year)
- Add reminders for upcoming maintenance
- Export data to CSV
- Add photos of receipts

## Troubleshooting

**App won't install:**
- Make sure you're using Safari on iOS
- Check that all files are uploaded to GitHub
- Verify manifest.json is accessible at your GitHub Pages URL

**Icons not showing:**
- Ensure icon-192.png and icon-512.png are in the root directory
- Check file names match exactly (case-sensitive)
- Clear browser cache and try again

**Service worker not working:**
- Check browser console for errors
- Make sure sw.js is in the root directory
- Update cache name in sw.js if making changes

## Browser Support

- ✅ iOS Safari (recommended)
- ✅ Chrome Mobile
- ✅ Firefox Mobile
- ✅ Desktop browsers (responsive design)

## License

Free to use and modify for personal use.

## Contributing

Feel free to fork and customize for your needs!

---

**Need help?** Check the browser console (F12) for error messages.
