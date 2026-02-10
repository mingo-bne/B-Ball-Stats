# Basketball Stats Tracker - iOS Installation Guide

## 📱 How to Install as an iOS App

This is a Progressive Web App (PWA) that works like a native iOS app without needing the App Store!

### Installation Steps for iPhone/iPad:

1. **Open in Safari**
   - Open Safari browser (must be Safari, not Chrome)
   - Navigate to the app URL where you've hosted the files

2. **Add to Home Screen**
   - Tap the Share button (square with arrow pointing up) at the bottom
   - Scroll down and tap "Add to Home Screen"
   - Edit the name if desired (default: "Stats Tracker")
   - Tap "Add" in the top right

3. **Launch the App**
   - Find the app icon on your home screen
   - Tap to launch - it opens fullscreen like a native app!

### Features:

✅ **Works Offline** - Track stats even without internet connection
✅ **Auto-saves Data** - Your games are automatically saved locally
✅ **Full Screen** - No browser bars, looks like a native app
✅ **Home Screen Icon** - Beautiful basketball icon
✅ **Fast Loading** - Cached for instant access

## 🌐 Hosting Your PWA

To make this available for installation, you need to host these files on a web server with HTTPS:

### Files to Upload:
- basketball-stats-tracker.html (rename to index.html)
- manifest.json
- service-worker.js
- icon-120.png
- icon-152.png
- icon-167.png
- icon-180.png
- icon-192.png
- icon-512.png

### Free Hosting Options:

1. **GitHub Pages** (Easiest)
   - Create a GitHub account
   - Create a new repository
   - Upload all files
   - Enable GitHub Pages in Settings
   - Access via: https://yourusername.github.io/repo-name

2. **Netlify** (Drag & Drop)
   - Go to netlify.com
   - Drag and drop your folder
   - Get instant HTTPS URL

3. **Vercel**
   - Similar to Netlify
   - Free tier available
   - vercel.com

4. **Firebase Hosting**
   - Google's hosting platform
   - Free tier available
   - firebase.google.com

### Requirements:
- ✅ HTTPS (required for PWA)
- ✅ All files in same directory
- ✅ Service worker must be in root directory

## 📝 Customization

### Change App Name:
Edit `manifest.json`:
```json
"name": "Your Team Stats",
"short_name": "Team Stats"
```

### Change App Colors:
Edit `manifest.json`:
```json
"background_color": "#YOUR_COLOR",
"theme_color": "#YOUR_COLOR"
```

### Change Icon:
Replace the icon-*.png files with your own basketball team logo
(must maintain the same sizes)

## 🔧 Testing

1. Host the files on a web server with HTTPS
2. Open in Safari on your iPhone
3. Add to home screen
4. Test offline by enabling Airplane mode
5. Verify data persists after closing and reopening

## 💡 Tips

- Data is saved automatically - no need to manually save
- Each game is stored locally on the device
- Export to CSV to backup important games
- Works on iPhone and iPad
- Supports both portrait and landscape modes
- Optimized for iOS notch and home indicator

## 🆘 Troubleshooting

**App won't install:**
- Make sure you're using Safari (not Chrome)
- Ensure the site is HTTPS
- Check that service-worker.js is in the root directory

**Data not saving:**
- Check browser storage isn't full
- Ensure you haven't disabled local storage in Safari settings

**App not working offline:**
- Make sure you opened it at least once while online
- Service worker needs to cache files on first visit

## 📊 What Gets Saved

The app automatically saves:
- Team roster (all players with jersey numbers)
- Complete game statistics for each player
- Play-by-play log
- Game information (teams, date)

All data is stored locally on your device using localStorage.

---

Need help? The app works entirely offline once installed, so you can track stats anywhere - even in gyms with no signal! 🏀
