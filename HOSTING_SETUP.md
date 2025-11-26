# Hosting rijultandon.engineer

## Option 1: Affordable Hosting (Recommended)

### Best Providers for Static Websites:
1. **Namecheap** (where you likely registered the domain)
   - Shared hosting: $2.88/month
   - Includes free SSL certificate
   - Easy file upload via cPanel/FTP

2. **Hostinger**
   - Shared hosting: $1.99/month
   - Great performance
   - Easy setup

3. **Bluehost**
   - WordPress-friendly
   - Good for static sites too
   - ~$2.95/month

## Setup Steps for Any Host

### Step 1: Upload Files via FTP
1. Download FTP client (FileZilla is free)
2. Connect using credentials from your host
3. Upload all files to `public_html/` folder:
   - index.html
   - styles.css
   - script.js
   - RIJUL_CV.pdf

### Step 2: Point Domain to Hosting
1. Go to your domain registrar (likely Namecheap)
2. Go to DNS settings
3. Update nameservers to your hosting provider's nameservers
   - OR point A records to hosting IP

### Step 3: Enable SSL/HTTPS
- Most hosts provide free SSL with Let's Encrypt
- Enable in cPanel or hosting dashboard
- This makes your site secure

## Step-by-Step via cPanel (Most Common)

1. **Login to cPanel**
   - URL: yourhosting.com:2083 or cpanel.rijultandon.engineer
   - Use credentials provided by host

2. **Upload Files**
   - Go to "File Manager"
   - Navigate to `public_html`
   - Upload all files here
   - Ensure index.html is in root

3. **Set Default Domain**
   - Go to "Addon Domains" or "Domains"
   - Ensure rijultandon.engineer points to public_html

4. **Enable SSL**
   - Go to "SSL/TLS Status"
   - Click "Install" for rijultandon.engineer

5. **Verify Site**
   - Visit https://rijultandon.engineer
   - Should see your portfolio

## Via FTP (FileZilla)

1. **Download FileZilla**: https://filezilla-project.org/

2. **Get FTP Credentials** from your host:
   - FTP/SFTP Server
   - Username
   - Password
   - Port (usually 21 or 22)

3. **Connect in FileZilla**:
   - File → Site Manager
   - New site
   - Enter FTP details
   - Click Connect

4. **Upload Files**:
   - Right pane: Navigate to public_html/
   - Left pane: Select your website files
   - Drag and drop to upload

5. **Verify**:
   - Visit https://rijultandon.engineer

## Free Alternative (If No Budget)

### Netlify (Free)
1. Push files to GitHub
2. Connect GitHub to Netlify
3. Deploy automatically
4. Add custom domain rijultandon.engineer
5. Free SSL included

**Steps:**
```bash
# Initialize git
git init
git add .
git commit -m "Initial portfolio"

# Push to GitHub (create repo first)
git remote add origin https://github.com/yourusername/portfolio.git
git push -u origin main

# Then connect to Netlify via their dashboard
```

## File Checklist Before Uploading

- [ ] index.html
- [ ] styles.css
- [ ] script.js
- [ ] RIJUL_CV.pdf
- [ ] All files in website folder

## Important Notes

- **index.html must be in root** (public_html/)
- **Ensure HTTPS is enabled** (for security)
- **Check file permissions** (644 for files, 755 for folders)
- **Wait 24-48 hours** for DNS propagation

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Site shows "coming soon" | Check if index.html is in public_html root |
| 404 error | Verify file names (case-sensitive on Linux) |
| HTTPS not working | Enable SSL in hosting dashboard |
| Slow loading | Check if CSS/JS files uploaded correctly |
| CV won't download | Ensure RIJUL_CV.pdf is in same folder as index.html |

## Support

Contact your hosting provider's support if you need help with:
- DNS settings
- FTP access
- SSL certificates
- cPanel navigation

---

Let me know which hosting provider you choose, and I can provide more specific instructions!
