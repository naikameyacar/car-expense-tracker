# 🚗 Car Expense Tracker Pro - Complete Setup Guide

A **mobile-first Progressive Web App (PWA)** for tracking vehicle expenses, fuel consumption, service records, and maintenance reminders. Designed specifically for **Indian users** with INR currency, kilometers, and KMPL fuel efficiency calculations.

## ✨ NEW Pro Features Added

### 1. 📷 Photo Attachments for Receipts
- **Upload photos** of fuel receipts, service invoices, and expense bills
- **Multiple photos** supported for service records
- **Drag & drop** support on desktop
- **Camera capture** on mobile devices
- **Full-screen viewer** to review photos
- Photos stored with entries for complete record-keeping

### 2. 👤 Driver Management
- **Add multiple drivers** to track who uses your vehicle
- **Assign drivers** to fuel, service entries
- **Driver selection** in timeline and reports
- Track expenses by driver
- Easy driver profile management

### 3. 📊 Fuel Price Trends
- **Visual charts** showing fuel price changes over time
- **Last 10 entries** trend analysis
- See how prices fluctuate
- Compare prices across dates
- Identify best times to refuel

### 4. 🔧 Service Cost Comparison
- **Bar charts** comparing costs by service type
- **Average costs** per service category
- **Total spending** by service type
- Identify expensive services
- Plan maintenance budget better

### 5. 📱 WhatsApp Reminders
- **Send reminders** directly to WhatsApp
- **One-tap sharing** from dashboard
- **Formatted messages** with vehicle details
- Set your WhatsApp number in settings
- Never miss PUC, insurance, or service dates

### 6. 🌙 Dark Mode
- **Toggle dark/light theme** from header or settings
- **Auto-saves preference** across sessions
- **Easy on the eyes** for night usage
- **Professional dark theme** with proper contrast
- Battery-friendly for OLED screens

## 📱 Core Features (Original)

- ✅ **Multi-vehicle support** - Track multiple cars/bikes
- ⛽ **Fuel tracking** - Record fuel entries with automatic KMPL calculation
- 🔧 **Service records** - Maintain complete service history
- 💰 **Expense tracking** - Track insurance, taxes, parking, tolls, etc.
- 🔔 **Reminders** - Get alerts for PUC, insurance, service due dates
- 📊 **Reports & Analytics** - Monthly summaries, category breakdown, cost per KM
- 📱 **Offline-first** - Works without internet, syncs when online
- 🔐 **Google Sign-In** - Secure authentication
- 📥 **Data Export** - Download CSV reports
- 🌐 **Installable PWA** - Add to home screen for app-like experience

### Indian Localization
- Currency: ₹ (INR)
- Distance: Kilometers (KM)
- Fuel efficiency: KMPL (Kilometers per Litre)
- Date format: DD/MM/YYYY (Indian format)

## 📱 Quick Start (User Guide)

### Installation
1. Open the app in your mobile browser
2. Tap the browser menu (⋮)
3. Select "Add to Home Screen" or "Install App"
4. The app icon will appear on your home screen

### First-Time Setup
1. Sign in with your Google account
2. Add your first vehicle (name, registration, fuel type, current odometer)
3. **(NEW)** Add drivers if multiple people use the vehicle
4. **(NEW)** Enable dark mode if preferred
5. **(NEW)** Set up WhatsApp reminders in Settings
6. Start tracking expenses!

### Adding Entries with Photos
- **Fuel**: Tap ➕ → Add Fuel → Fill details → **📷 Tap photo area** → Take/upload receipt photo
- **Service**: Tap ➕ → Add Service → Enter details → **📷 Add multiple invoice photos**
- **Expense**: Tap ➕ → Add Expense → **📷 Attach receipt** → Save

### Using Driver Management
1. Go to Dashboard → Tap **👤 Drivers** icon
2. Add drivers with name and phone number
3. When adding fuel/service entries, select the driver from dropdown
4. View entries filtered by driver in timeline

### Viewing Trends & Comparisons
1. Go to **Reports** tab
2. Switch to **Fuel Trends** tab to see price changes
3. Switch to **Service Cost** tab to compare service expenses
4. Charts update automatically as you add more data

### Setting Up WhatsApp Reminders
1. Go to **Settings** → WhatsApp Notifications
2. Toggle **Enable WhatsApp Reminders** ON
3. Enter your WhatsApp number (with country code, e.g., +919876543210)
4. From Dashboard reminders, tap **📱 Send** button
5. WhatsApp opens with pre-filled message

### Using Dark Mode
- **Quick toggle**: Tap 🌙/☀️ icon in header
- **Settings**: Go to Settings → Appearance → Toggle Dark Mode
- Preference saves automatically

## 🔧 Technical Setup (For Hosting)

### Option 1: Simple Hosting (No Google Sheets)

The app works completely offline using browser localStorage. Perfect for personal use.

**Steps:**
1. Download these files:
   - `car-expense-tracker-pro.html`
   - `manifest.json`
   - `sw.js`

2. Host on any web server:
   - **GitHub Pages**: Free, easy hosting
   - **Netlify/Vercel**: Free tier available
   - **Firebase Hosting**: Google integration ready
   - **Local**: Just open the HTML file in your browser

3. Access on mobile browser and install as PWA

### Option 2: With Google Sheets Integration

Follow the original README instructions for Google Sheets API setup.

## 📊 Photo Storage

Photos are stored as **base64 encoded images** in localStorage:
- Each photo stored with the entry
- Compressed for efficient storage
- No external server needed
- Export includes photo indicator
- Full-screen viewer for reviewing receipts

**Storage Tips:**
- Photos take up space in localStorage (~5MB limit per domain)
- Use camera compression when possible
- Consider exporting data regularly
- Service records support multiple photos per entry

## 🎯 Usage Tips for New Features

### Photo Attachments
1. **Take clear photos** in good lighting
2. **Capture entire receipt** including date and amount
3. **Multiple angles** for service invoices with parts list
4. **Tap any photo** in timeline or details to view full screen
5. **Photos export** with CSV as "Yes/No" indicator

### Driver Management
1. **Add all regular drivers** including yourself
2. **Assign driver** when adding fuel/service for accurate tracking
3. **Filter timeline** by driver to see their expenses
4. **Useful for family cars** or shared vehicles

### Fuel Price Trends
1. **Record consistent entries** for accurate trends
2. **Last 10 entries shown** - add more for better visualization
3. **Compare fuel types** if you use multiple
4. **Identify price patterns** for better refueling decisions

### Service Cost Comparison
1. **Categorize services properly** for accurate comparison
2. **Average costs shown** to spot unusually expensive services
3. **Plan future budgets** based on service history
4. **Compare across service centers** by tracking location

### WhatsApp Reminders
1. **Set number once** in settings
2. **Quick send** from dashboard reminders
3. **Message pre-formatted** with all details
4. **Useful for sharing** with family members
5. **Works offline** - sends when you open WhatsApp

### Dark Mode
1. **Auto-saves preference** across sessions
2. **Both header and settings** toggle available
3. **System-friendly** - won't override device settings
4. **OLED-optimized** pure black background
5. **All screens supported** including modals

## 📱 PWA Features

- **Offline Mode**: Full functionality without internet
- **Home Screen Install**: App-like experience
- **Background Sync**: Auto-sync when connection restored
- **Fast Loading**: Cached resources for instant access
- **Responsive**: Works on all screen sizes
- **Photo Capture**: Direct camera access on mobile

## 🆘 Troubleshooting

### Photos not uploading
- Check browser permissions for camera/files
- Ensure file size is reasonable (<5MB)
- Try different photo format (JPG works best)
- Check available localStorage space

### Dark mode not saving
- Clear browser cache and reload
- Check if localStorage is enabled
- Try toggling from settings instead of header

### WhatsApp not opening
- Verify number format (+91XXXXXXXXXX for India)
- Ensure WhatsApp is installed
- Check browser allows opening external apps
- Try re-entering the number

### Charts not showing
- Add at least 2 entries for trends
- Check if data exists for selected vehicle
- Reload the reports tab
- Verify entries have proper dates

### Driver not appearing in dropdown
- Refresh the page after adding driver
- Check driver was saved (go to Drivers screen)
- Try adding fuel entry again

## 🔒 Security & Privacy

- **Authentication**: Secure Google OAuth 2.0
- **Data Storage**: Your device + Google account only
- **Photos**: Stored locally, not uploaded anywhere
- **No Third-Party Access**: Your data stays with you
- **No Tracking**: No analytics or user tracking
- **WhatsApp**: Only sends when you tap the button

## 🌐 Browser Compatibility

- ✅ Chrome/Edge (Android/Desktop) - **Full support**
- ✅ Safari (iOS/Desktop) - **Full support**
- ✅ Firefox (Android/Desktop) - **Full support**
- ✅ Samsung Internet - **Full support**
- ✅ Dark mode works on all browsers
- ✅ Photo upload works on mobile and desktop

## 🎨 What's Different in Pro Version?

| Feature | Basic Version | **Pro Version** |
|---------|---------------|-----------------|
| Photo Receipts | ❌ | ✅ **Full support** |
| Driver Management | ❌ | ✅ **Multiple drivers** |
| Fuel Price Trends | ❌ | ✅ **Visual charts** |
| Service Comparison | ❌ | ✅ **Cost analysis** |
| WhatsApp Reminders | ❌ | ✅ **One-tap send** |
| Dark Mode | ❌ | ✅ **Full theme** |
| Timeline Photos | Basic | ✅ **Photo indicators** |
| Export Format | Basic CSV | ✅ **Enhanced CSV** |

## 📄 File Structure

```
car-expense-tracker-pro.html    (108KB - Complete app)
manifest.json                   (PWA configuration)
sw.js                          (Service worker)
README-PRO.md                  (This file)
```

## 🚀 Future Enhancements

Possible additions:
- [ ] Cloud photo storage option
- [ ] Trip tracking with routes
- [ ] Multi-language support (Hindi, Tamil, etc.)
- [ ] Voice input for quick entries
- [ ] OCR for receipt scanning
- [ ] Expense categories customization
- [ ] Fuel station locator
- [ ] Maintenance predictions with AI

## 📞 Support

For issues:
1. Check this README first
2. Clear browser cache and photos
3. Try incognito/private mode
4. Check localStorage limit (5MB)
5. Reinstall the PWA

---

**Version**: 2.0 Pro  
**Last Updated**: January 2026  
**Optimized for**: Mobile browsers & PWA in India  
**New Features**: Photos, Drivers, Trends, Comparisons, WhatsApp, Dark Mode

**Made with ❤️ in India**
