# WCTE Vendor Portal - Dance Competition 1099 Vendor Management

A complete web-based system for managing dance competition vendor time entries, payments, and 1099 contractor data.

## 🎯 Features

### For Vendors
- ✅ Email-based login (no password needed)
- ✅ Multiple pay structures supported:
  - Hourly rate with automatic overtime calculation
  - Full day / Half day rates
  - Per-routine payment
  - Fixed event payment
- ✅ Automatic payment calculations
- ✅ Expense tracking (travel, meals, lodging)
- ✅ Real-time submission confirmation

### For Office Staff
- ✅ Admin dashboard with all submissions
- ✅ Approve/reject workflow
- ✅ Payment tracking (pending → approved → paid)
- ✅ Filter and search functionality
- ✅ Export to CSV for accounting
- ✅ Email notifications for new submissions

## 🏗️ Architecture

```
Vendor Portal (HTML/JavaScript)
         ↓
    GitHub Pages (Free Hosting)
         ↓
    Embedded in Wix Studio (iframe)
         ↓
    Google Sheets (Database) + EmailJS (Notifications)
```

**Total Cost: $0** (using free tiers)

## 📋 Prerequisites

- Google Account (for Google Sheets)
- EmailJS Account (free tier: 300 emails/month)
- GitHub Account (for hosting)
- Wix Studio Site (for embedding)

## 🚀 Quick Start

1. **Read the Setup Guide:** `SETUP_GUIDE.md` contains detailed step-by-step instructions
2. **Create Google Sheet:** Set up your vendor database and time entry tracking
3. **Configure EmailJS:** Set up email notifications
4. **Deploy to GitHub Pages:** Host the portal for free
5. **Embed in Wix:** Add to your existing website

## 📁 Files Included

- `index.html` - Vendor time entry portal
- `admin.html` - Office admin dashboard
- `SETUP_GUIDE.md` - Complete setup instructions
- `google-apps-script.js` - Helper script for Google Sheets automation
- `README.md` - This file

## 🎨 Customization

### Branding
- Logo: Replace logo references in HTML
- Colors: Update CSS gradient values
- Text: Modify headers and labels as needed

### Pay Structures
Easily add new vendor pay types by:
1. Adding new entry in Google Sheets "Vendors" tab
2. Adding calculation logic in JavaScript

### Email Templates
Customize email notifications in EmailJS dashboard

## 📊 Data Collected

### Vendor Profile (One-time)
- Legal name, email, phone
- SSN/EIN (last 4 digits)
- Pay structure and rates
- W-9 status
- Payment preferences

### Time Entry (Per Event)
- Event date, name, location
- Role performed
- Time worked (based on pay type)
- Expenses and reimbursements
- Total calculated payment

## 🔒 Security Features

- No passwords stored (email-based access)
- Vendor data stored in your Google Sheet (you control access)
- Service account for API access (no user credentials exposed)
- HTTPS-only (GitHub Pages enforces SSL)

## 📱 Mobile Responsive

Both vendor portal and admin dashboard are fully responsive and work on:
- Desktop computers
- Tablets
- Mobile phones

## 🧪 Testing

### Test Accounts (included in SETUP_GUIDE.md)
- Hourly vendor: `judge1@example.com`
- Daily rate vendor: `instructor@example.com`
- Per-routine vendor: `judge2@example.com`
- Fixed rate vendor: `adjudicator@example.com`

## 📧 Support

**Technical Setup:**
- See detailed instructions in `SETUP_GUIDE.md`
- Google Sheets API docs: https://developers.google.com/sheets/api
- EmailJS docs: https://www.emailjs.com/docs/

**WCTE Specific:**
- Email: office@wctedance.com

## 📝 License

This system is created for World-Class Talent Experience (WCTE).
All rights reserved.

## 🎉 Credits

Built with:
- Vanilla JavaScript (no frameworks required)
- Google Sheets API
- EmailJS
- GitHub Pages

---

## Version History

**v1.0** (January 2025)
- Initial release
- Vendor portal with 4 pay structures
- Admin dashboard
- Google Sheets integration
- EmailJS notifications

---

**Ready to get started?** Open `SETUP_GUIDE.md` for step-by-step instructions!
