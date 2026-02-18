# Password Protection Setup

Your Italy Trip 2026 site now has password protection!

## 🔐 Current Password

**Password**: `Italy2026Ski`

Share this password with your wife. Both of you can access the site using this password.

## 🔄 How to Change the Password

1. Open `set-password.html` in your browser (locally, not on GitHub Pages)
2. Enter your new password
3. Click "Generate Hash"
4. Copy the generated hash
5. Open `auth.html` in a text editor
6. Find the line: `const passwordHash = '...'`
7. Replace the hash with your new one
8. Commit and push to GitHub

## 🚪 How It Works

- Main page: `index.html` (requires authentication)
- Login page: `auth.html` (shows password prompt)
- Password tool: `set-password.html` (helps you generate new password)

When someone visits your site, they'll see the login page first. After entering the correct password, they get access for that browser session.

## ⚠️ Security Notes

**This is CLIENT-SIDE protection** - it's better than nothing but not bank-level secure:

✅ **Prevents**: Casual access, accidental shares, search engine indexing
❌ **Doesn't prevent**: Determined technical users who inspect the code

For better security, consider:
- Moving to Netlify (has built-in password protection)
- Making GitHub repo private (requires GitHub Pro)
- Using a proper authentication service

## 📱 Mobile Access

The password works the same way on mobile devices. Just enter it once per browser session.
