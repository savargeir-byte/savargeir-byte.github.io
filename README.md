# Aurora Vision Developer Website

This is the developer website for Aurora Vision iOS app, required for AdMob app-ads.txt verification.

## Setup Instructions

1. **Create new GitHub repository:**

   - Repository name: `savargeir-byte.github.io` (must match your username exactly)
   - Description: "Aurora Vision Developer Website"
   - Public repository
   - Initialize with README: No (we'll push these files)

2. **Upload these files to the new repo:**

   ```bash
   # Clone the new repo
   git clone https://github.com/savargeir-byte/savargeir-byte.github.io.git
   cd savargeir-byte.github.io

   # Copy files from this folder
   cp ../Nor-uljos/github-pages-setup/* .

   # Commit and push
   git add .
   git commit -m "Initial commit: Add app-ads.txt and landing page"
   git push
   ```

3. **Enable GitHub Pages:**

   - Go to: https://github.com/savargeir-byte/savargeir-byte.github.io/settings/pages
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/ (root)`
   - Save

4. **Wait 2-5 minutes** for GitHub Pages to deploy

5. **Verify app-ads.txt is live:**

   - Open: https://savargeir-byte.github.io/app-ads.txt
   - Should show: `google.com, pub-1625281157866154, DIRECT, f08c47fec0942fa0`

6. **Update App Store Connect:**

   - Go to App Store Connect
   - Your app → App Information
   - Developer Website: `https://savargeir-byte.github.io`
   - Save

7. **Update AdMob:**
   - Go to AdMob console
   - App settings → App-ads.txt
   - Click "Check for updates"

## Files Included

- `app-ads.txt` - AdMob verification file (required)
- `index.html` - Simple landing page (optional but recommended)
- `README.md` - Setup instructions (this file)

## Troubleshooting

If app-ads.txt doesn't work:

1. Check the file is accessible: https://savargeir-byte.github.io/app-ads.txt
2. Verify HTTP status is 200 (not 404)
3. Ensure content matches exactly (no extra spaces or BOM)
4. Wait 10-15 minutes for AdMob to re-crawl
5. Clear browser cache and try again

## Support

For issues with Aurora Vision app, contact: [your-email@example.com]
