# GMC Swimming Team Records Dashboard

A clean, mobile-responsive dashboard displaying GMC Swimming team records.

## Quick Setup for GitHub Pages

### 1. Create GitHub Repository
- Go to github.com and create a new repository
- Name it something like `gmc-swimming-records`
- Make it public
- Don't initialize with README (we have one)

### 2. Upload Your Files
Two ways to do this:

**Option A: GitHub Web Interface (Easiest)**
- Click "uploading an existing file"
- Drag these files: `index.html`, `README.md`
- Drag the entire `assets` folder
- Commit changes

**Option B: Command Line**
```bash
git init
git add .
git commit -m "Initial commit - GMC Swimming Records"
git remote add origin https://github.com/YOUR-USERNAME/gmc-swimming-records.git
git push -u origin main
```

### 3. Enable GitHub Pages
- Go to repository Settings
- Click "Pages" in left sidebar
- Under "Source", select "main" branch
- Click Save
- Your site will be live at: `https://YOUR-USERNAME.github.io/gmc-swimming-records/`

### 4. Add Your Logo
- Compress your PNG logo (use tinypng.com to get under 50KB)
- Upload it to `assets/images/` folder
- Name it exactly: `logo.png`

## File Structure
```
your-repo/
├── index.html              # Main dashboard page
├── README.md              # This file
└── assets/
    ├── data/
    │   └── records.json   # Team records data
    └── images/
        └── logo.png       # Your logo (you'll add this)
```

## Updating Records

When you need to update records (typically once per season):

1. **Edit the JSON file**: Open `assets/data/records.json`
2. **Update the record**: Find the event and modify the name, time, or date
3. **Update the timestamp**: Change the date in `index.html` (search for "Last updated")
4. **Commit changes**: Push to GitHub and the site updates automatically

### Example JSON Record
```json
{
  "event_number": 3,
  "gender": "Women",
  "distance": "200",
  "stroke": "Freestyle",
  "time": "1:58.94",
  "first_name": "Kathryn",
  "last_name": "Snover",
  "age": "15",
  "date": "9/24/2016",
  "meet": "Region Championship"
}
```

## Adding Swimmer Photos (Future)

When ready to add photos:
1. Create `assets/images/swimmers/` folder
2. Upload photos named: `firstname-lastname.jpg` (lowercase, no spaces)
3. Compress photos first (aim for under 200KB each)
4. Example: `kathryn-snover.jpg`

## Brand Colors Used
- Navy: `#00205B` (backgrounds, headers)
- White: `#FFFFFF` (text, table backgrounds)
- Light Blue: `#8DC8E8` (accents, subtitles)
- Trophy Gold: `#D4AF37` (record times)
- Lane Silver: `#C1C6C8` (borders)

## Fonts
- **Oswald Bold**: Titles and headings
- **Montserrat**: Body text and names
- **Source Sans Pro**: Subtitles
- **Source Serif Pro**: Dates and captions

All fonts load from Google Fonts automatically.

## Support
This is a static site (no database, no server costs). It will continue working as long as GitHub Pages is available (which is free forever for public repos).

To pass this to a future coach: Give them access to the GitHub repo. Everything they need is here.
