# LoveLink Web - Password Reset Page

This is the password reset page for the LoveLink mobile app.

## Setup Instructions

### 1. Update Supabase Credentials

Edit `index.html` and replace `YOUR_SUPABASE_ANON_KEY_HERE` with your actual Supabase anon key:

```javascript
const SUPABASE_URL = 'https://tfrhdxatjsyobmyffuzg.supabase.co';
const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY_HERE';  // Replace this!
```

You can find your anon key in:
- Supabase Dashboard → Settings → API → anon public key

### 2. Deploy to GitHub Pages

1. Create a new repository on GitHub called `lovelink-web`
2. Push this code:

```bash
git init
git add .
git commit -m "LoveLink password reset page"
git remote add origin https://github.com/YOUR_USERNAME/lovelink-web.git
git branch -M main
git push -u origin main
```

3. Go to repository Settings → Pages
4. Source: Deploy from branch `main`
5. Your site will be live at: `https://YOUR_USERNAME.github.io/lovelink-web`

### 3. Configure Supabase

1. Go to Supabase Dashboard → Authentication → URL Configuration
2. Set **Site URL** to: `https://YOUR_USERNAME.github.io/lovelink-web`
3. Add to **Redirect URLs**: `https://YOUR_USERNAME.github.io/lovelink-web`

### 4. Test It

1. Open the LoveLink app
2. Go to Login → Forgot Password
3. Enter your email
4. Check your email and click the reset link
5. You should see the branded reset page

## Alternative: Deploy to Netlify

1. Go to https://app.netlify.com/drop
2. Drag and drop this folder
3. Use the Netlify URL in Supabase settings

## Files

- `index.html` - Password reset page
- `README.md` - This file
- `.gitignore` - Git ignore file

## Customization

- Edit the colors in the `<style>` section to match your brand
- Update the logo emoji or add a custom image
- Modify the success/error messages as needed
