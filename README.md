# Colour Website

A modern one-page website for the Colour app.

## Deploying to Vercel

### Option 1: Deploy via Vercel CLI (Recommended)

1. **Install Vercel CLI** (if not already installed):
   ```bash
   npm install -g vercel
   ```

2. **Navigate to the website folder**:
   ```bash
   cd website
   ```

3. **Deploy**:
   ```bash
   vercel
   ```

4. **Follow the prompts**:
   - Log in to Vercel if prompted
   - Select your scope/team
   - Link to existing project or create new one
   - Confirm the settings

5. **Deploy to production**:
   ```bash
   vercel --prod
   ```

### Option 2: Deploy via GitHub

1. **Push the website folder to a GitHub repository**

2. **Go to [vercel.com](https://vercel.com)** and sign in

3. **Click "Add New Project"**

4. **Import your GitHub repository**

5. **Configure the project**:
   - Root Directory: `website` (if website is a subfolder)
   - Framework Preset: Other
   - Build Command: (leave empty)
   - Output Directory: `.`

6. **Click "Deploy"**

### Option 3: Drag and Drop

1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag and drop the entire `website` folder
3. Vercel will automatically deploy it

## Custom Domain Setup

After deploying:

1. Go to your project on Vercel Dashboard
2. Click "Settings" → "Domains"
3. Add your custom domain (e.g., `colourapp.com`)
4. Follow Vercel's instructions to configure DNS:
   - For apex domain: Add an `A` record pointing to `76.76.21.21`
   - For subdomain: Add a `CNAME` record pointing to `cname.vercel-dns.com`

## Files

- `index.html` - Main landing page
- `privacy.html` - Privacy policy (required for App Store)
- `terms.html` - Terms of service
- `vercel.json` - Vercel configuration

## Updating the App Store Link

The App Store link in the website is set to:
```
https://apps.apple.com/app/id6758033488
```

This should work once your app is approved and live on the App Store.

## Adding Assets

You may want to add:
- `favicon.png` - Browser tab icon (32x32 or 64x64)
- `og-image.png` - Social sharing image (1200x630 recommended)
- App screenshots for the hero section
