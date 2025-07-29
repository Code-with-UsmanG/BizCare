# BizCare Legal Pages Deployment Guide

This repository contains the Terms & Conditions and Privacy Policy web pages for the BizCare mobile application. These pages are designed to be responsive, professional, and user-friendly.

## Files Included

1. `index.html` - Landing page with app information
2. `terms_and_conditions.html` - Terms & Conditions page
3. `privacy_policy.html` - Privacy Policy page
4. `styles.css` - Shared styles for all pages
5. `bizcare_logo.png` - BizCare logo (you need to add this)
6. `app_screenshot.png` - App screenshot for the landing page (you need to add this)

## Deployment Instructions

### 1. Prepare the Files

- Add your BizCare logo as `bizcare_logo.png` to the same directory as the HTML files
- Add an app screenshot as `app_screenshot.png` for the landing page
- Review and update the content in the HTML files if needed

### 2. Deploy to Your Web Server

#### Option 1: Traditional Web Hosting

1. Upload all files to your web hosting service (e.g., cPanel, Plesk)
2. Ensure the files are placed in the correct directory (e.g., `public_html` or `www`)
3. Make sure the files have the correct permissions (typically 644 for files)

#### Option 2: GitHub Pages

1. Create a new GitHub repository
2. Upload all files to the repository
3. Go to repository Settings > Pages
4. Select the branch to deploy (e.g., main) and save
5. Your site will be available at `https://yourusername.github.io/repositoryname/`

#### Option 3: Netlify or Vercel

1. Create an account on [Netlify](https://www.netlify.com/) or [Vercel](https://vercel.com/)
2. Connect your GitHub repository or upload the files directly
3. Follow the deployment instructions on the platform
4. Your site will be available at the provided URL

### 3. Update URLs in the App

After deploying the web pages, update the URLs in the Flutter app:

1. Open `lib/screens/login_screen.dart`
2. Locate the following lines:
```dart
final String _termsUrl = 'https://bizcare.pk/terms_and_conditions.html';
final String _privacyUrl = 'https://bizcare.pk/privacy_policy.html';
```
3. Replace these URLs with your actual deployed URLs
4. Rebuild and deploy your Flutter app

## Customization

You can customize the appearance of the web pages by modifying the `styles.css` file. The main color scheme is based on the BizCare green (#00A884), but you can change it to match your branding.

## Testing

Before deploying to production, test the web pages on various devices and browsers to ensure they are responsive and function correctly. The pages are designed to be mobile-friendly and should work well on all screen sizes.

## Support

If you have any questions or need assistance with the deployment, please contact the development team. 