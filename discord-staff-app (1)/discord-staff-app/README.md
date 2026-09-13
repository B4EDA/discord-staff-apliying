# Discord Staff Application System

A professional Discord staff and moderator application system with an integrated admin panel. Features real-time application management, scenario-based evaluation, and server level tracking.

## Features

✨ **Application Form**
- Discord username with validation
- Server level indicator (1-50 scale)
- Real-world moderation scenario question
- Time commitment selection
- Comprehensive background questions
- Email collection for follow-up

✨ **Admin Panel**
- Real-time application tracking
- Filter applications by status (New, Accepted, Rejected)
- Detailed application review modal
- Quick accept/reject actions
- Statistics dashboard
- Application history management

✨ **Data Storage**
- Secure browser-based storage (localStorage)
- All data saved locally
- Admin notifications accessible from panel
- No server required

✨ **Responsive Design**
- Mobile-friendly interface
- Works on all devices
- Modern UI with gradient design
- Smooth animations

## Tech Stack

- Pure HTML5
- CSS3 (No frameworks)
- Vanilla JavaScript (No dependencies)
- localStorage for data persistence

## Quick Start

### Option 1: Deploy on Vercel (Recommended)

1. **Fork or Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/discord-staff-app.git
   cd discord-staff-app
   ```

2. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/discord-staff-app.git
   git push -u origin main
   ```

3. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Select your GitHub repository
   - Click "Deploy"
   - Your site will be live in seconds!

### Option 2: Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/discord-staff-app.git
   cd discord-staff-app
   ```

2. **Start a local server**
   ```bash
   # Using Python 3
   python -m http.server 3000
   
   # Or using Node.js
   npx http-server -p 3000
   ```

3. **Open in browser**
   - Navigate to `http://localhost:3000`
   - Start accepting applications!

## Usage

### For Applicants

1. Click **"Apply Now"** tab
2. Fill in all required fields:
   - Discord username
   - Full name and email
   - Age (must be 13+)
   - Server level (1-50 scale)
   - Answer the moderation scenario
   - Select time commitment
   - Choose role to apply for
3. Accept terms and submit
4. See confirmation message
5. Admin will review and reach out

### For Admins

1. Click **"Admin Panel"** tab
2. View statistics at the top:
   - Total applications
   - New applications
   - Accepted/Rejected counts
3. Filter applications:
   - All: See all applications
   - New: Only unreviewed applications
   - Accepted: Approved applicants
   - Rejected: Declined applications
4. Click **"View"** to see full application details
5. In the detail modal:
   - Review all answers
   - Check server level and scenario response
   - Click "Accept" or "Reject" to update status
6. Delete applications as needed
7. Use "Clear All Data" to reset everything (caution: irreversible)

## Application Questions

### Moderation Scenario
The application includes a realistic moderation scenario:
> "You're moderating the server when a member starts sending spam messages and mentions a controversial topic that's causing conflict. The member claims they're just joking around. Other members are getting upset and reporting the messages."

Applicants must describe how they would handle this situation as a moderator. Their response helps assess:
- Decision-making skills
- Community management approach
- Conflict resolution abilities
- Fairness and professionalism

## Server Level Scale

- **1-5**: New Member
- **6-15**: Active Member
- **16-30**: Regular Contributor
- **31-50**: Trusted / Legend Status

## Data Privacy

⚠️ **Important:** This application stores all data in browser's localStorage. This means:
- Data is stored locally on each browser
- Data persists across page refreshes
- Clearing browser cache will erase all data
- No data is sent to external servers
- This is suitable for single-device admin usage

## Customization

### Change the Moderation Scenario
Edit line ~450 in `index.html`:
```html
<p>Your custom scenario here...</p>
```

### Modify Server Level Labels
Update the level labels in the range slider (lines ~520-525):
```html
<span>New Member</span>
<span>Your Label</span>
<span>Another Label</span>
```

### Change Colors
Modify the gradient colors in CSS (search for `#667eea` and `#764ba2`):
```css
background: linear-gradient(135deg, #YOUR_COLOR 0%, #YOUR_COLOR_2 100%);
```

## File Structure

```
discord-staff-app/
├── index.html          # Complete application (HTML + CSS + JS)
├── package.json        # Project metadata
├── vercel.json         # Vercel deployment config
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Deployment URLs

After deployment, share these links:
- **Apply Form**: `https://your-domain.com`
- **Admin Panel**: `https://your-domain.com` (click Admin tab)

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Troubleshooting

### Applications not saving?
- Check if localStorage is enabled in browser settings
- Try clearing browser cache and refreshing
- Ensure you're using a compatible browser

### Admin panel shows no apps?
- Verify applications were submitted from the same browser
- localStorage is device/browser specific
- Try submitting a test application

### Styles not loading correctly?
- Hard refresh the page (Ctrl+Shift+R or Cmd+Shift+R)
- Clear browser cache
- Check browser console for errors

## Future Enhancements

Potential features for future versions:
- [ ] Email notifications integration
- [ ] Database backend (MongoDB, Firebase)
- [ ] User authentication for admins
- [ ] Scheduled review reminders
- [ ] Bulk export (PDF, CSV)
- [ ] Application comments/notes
- [ ] Custom questions builder
- [ ] Multiple admin accounts
- [ ] Email sending on accept/reject
- [ ] Discord webhook integration

## License

MIT License - Feel free to use and modify for your community!

## Support

Having issues? 
- Check this README thoroughly
- Review browser console for errors
- Ensure JavaScript is enabled
- Try a different browser

---

**Made with ❤️ for Discord Communities**
