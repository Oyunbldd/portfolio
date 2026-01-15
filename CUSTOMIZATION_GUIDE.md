# Customization Guide

This guide will help you personalize your portfolio website according to the requirements.

## ✅ Completed Changes

1. **Meta Tags & Title** - Updated with portfolio description
2. **Services Section** - Changed to showcase your skills (Web Development, Responsive Design, UI/UX)
3. **Portfolio Section** - Updated with coding projects template
4. **About Section** - Converted to Academic Journey timeline
5. **Favorites Section** - Added new section for Activities, Food, and Sports
6. **Navigation** - Updated to include Favorites section
7. **Contact Form** - Added TODO comments for email configuration
8. **Accessibility** - Added alt text to images

## 📝 What You Need to Customize

### 1. Hero Section (Masthead)
**File:** `index.html` (around line 50-55)
- Update the welcome message if desired
- The current text is: "Welcome To My Portfolio!" and "Developer & Student"

### 2. Services Section
**File:** `index.html` (around line 58-100)
- Already updated with generic services, but you can modify:
  - Service titles and descriptions
  - Icons (change Font Awesome icons if needed)

### 3. Portfolio Section - **IMPORTANT**
**File:** `index.html` (around line 108-195 and modals 451-650)

You need to replace all `[Project Name X]` placeholders with:
- **Project Names** - Replace `[Project Name 1]` through `[Project Name 6]` with your actual project names
- **Project Descriptions** - Fill in the `[Brief project description]` and detailed descriptions
- **Technologies** - Replace `[List technologies]` with actual tech stack (e.g., "HTML, CSS, JavaScript, React")
- **Dates** - Replace `[Project Date]` with actual dates
- **Project Types** - Replace `[Academic/Personal/Hackathon Project]` with the actual type
- **Categories** - Replace `[Category]` with appropriate categories

**Example:**
```html
<h2 class="text-uppercase">Todo List App</h2>
<p class="item-intro text-muted">A responsive todo application built with React</p>
...
<p><strong>Technologies Used:</strong> React, JavaScript, CSS, LocalStorage API</p>
<ul class="list-inline">
  <li>Date: December 2023</li>
  <li>Type: Personal Project</li>
  <li>Category: Web Development</li>
</ul>
```

### 4. About Section - Academic Journey
**File:** `index.html` (around line 196-289)

Replace all placeholder brackets with your actual information:
- `[YEAR] - [YEAR]` - Replace with actual years
- `[activities/clubs]` - List your high school activities
- `[Field of Study]` - Your major/degree program
- `[University Name]` - Your university name
- `[Year/Semester]` - Current academic status
- `[Degree Program]` - Your degree program
- `[current projects/research]` - What you're working on
- `[future academic goals]` - Your plans

**Example:**
```html
<h4>2020 - 2022</h4>
<h4 class="subheading">High School</h4>
...
<p class="text-muted">
  Completed high school education. Developed foundational knowledge in mathematics, science, and computer basics. 
  Participated in Computer Science Club and Math Team. This period sparked my initial interest in technology and programming.
</p>
```

### 5. Favorites Section
**File:** `index.html` (around line 290-336)

Replace the placeholder lists with your actual favorites:

**Activities:**
- Replace `[Activity 1]`, `[Activity 2]`, etc. with your favorite activities
- Examples: Hiking, Reading, Gaming, Photography, Drawing, Learning new technologies

**Food:**
- Replace `[Food 1]`, `[Food 2]`, etc. with your favorite foods
- Examples: Pizza, Sushi, Italian cuisine, Homemade desserts

**Sports:**
- Replace `[Sport 1]`, `[Sport 2]`, etc. with your favorite sports
- Examples: Basketball, Soccer, Tennis, Swimming, Esports

### 6. Contact Form Email Configuration
**File:** `assets/mail/contact_me.php` (line 19)

⚠️ **IMPORTANT:** Update the email address:
```php
$to = 'yourname@yourdomain.com'; // Replace with YOUR email address
```

Also update line 22 if you have a custom domain:
```php
$headers = "From: noreply@yourdomain.com\n"; // Update with your domain
```

**Note:** For GitHub Pages deployment, PHP won't work. You'll need to:
- Use a form service like Formspree, Netlify Forms, or EmailJS
- Or set up a serverless function
- Or use a third-party contact form service

### 7. Footer
**File:** `index.html` (around line 437-450)
- Update copyright year if needed
- Update social media links (currently placeholder `#!`)
- Update Privacy Policy and Terms of Use links if you have them

### 8. Portfolio Images
**Location:** `assets/img/portfolio/`

Replace the placeholder images with screenshots of your actual projects:
- `01-thumbnail.jpg` and `01-full.jpg` - Project 1 images
- `02-thumbnail.jpg` and `02-full.jpg` - Project 2 images
- ... and so on

**Recommended sizes:**
- Thumbnails: ~400x300px
- Full images: ~1200x900px

### 9. About Timeline Images
**Location:** `assets/img/about/`

Replace with images representing your academic journey:
- `1.jpg` - High school period
- `2.jpg` - University start
- `3.jpg` - Academic growth
- `4.jpg` - Current status

## 🚀 Deployment to GitHub Pages

1. **Create a GitHub repository** (if you haven't already)
2. **Push your code** to the repository
3. **Go to Settings** → **Pages**
4. **Select source branch** (usually `main` or `master`)
5. **Select folder** (`/root`)
6. **Save** - Your site will be available at `https://yourusername.github.io/repository-name`

**Important Notes:**
- PHP contact form won't work on GitHub Pages (static hosting only)
- Consider using Formspree, Netlify Forms, or EmailJS for the contact form
- Make sure all image paths are relative (they already are)

## 📋 Checklist Before Submission

- [ ] All `[Project Name X]` replaced with actual project names
- [ ] All project descriptions filled in
- [ ] Technologies listed for each project
- [ ] Academic timeline filled with your information
- [ ] Favorites section updated (Activities, Food, Sports)
- [ ] Portfolio images replaced with project screenshots
- [ ] About timeline images replaced
- [ ] Contact form configured (or alternative solution)
- [ ] Social media links updated (if applicable)
- [ ] Test website on different screen sizes (responsive design)
- [ ] Deploy to GitHub Pages
- [ ] Test all links and navigation

## 🎨 Optional Enhancements

- Add links to your GitHub repositories in portfolio modals
- Add live demo links for projects
- Customize colors in CSS (primary color is `#fed136` - yellow)
- Add more sections if needed
- Add animations or transitions
- Optimize images for web (compress before uploading)

## 📞 Need Help?

If you encounter any issues:
1. Check browser console for errors (F12)
2. Verify all file paths are correct
3. Ensure images are in the correct folders
4. Test locally before deploying

Good luck with your portfolio! 🎉
