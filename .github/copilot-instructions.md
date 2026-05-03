# Copilot Instructions for Dr. Amrit Pal's Academic Website

## Project Overview
This is a static HTML/CSS website showcasing Dr. Amrit Pal's academic profile at Vellore Institute of Technology Chennai. The site consists of interconnected pages with consistent styling and navigation patterns.

## Architecture & File Structure

**Pages:**
- `index.html` - Main homepage with hero section, qualifications, and navigation
- `students.html`, `students1.html`, `students2 Fist photo.html` - Student gallery/profile pages
- `Teaching.html` - Teaching information and course details
- `image/` - Static assets (profile images, campus photos)

**Styling Approach:**
- Inline CSS within `<style>` tags (no external stylesheets)
- Mobile-first responsive grid layout using CSS Grid and Flexbox
- Consistent color scheme: dark header (#0f172a, #04171a), light background (#f4f7fb)
- Reusable CSS classes: `.container` (width constraint), `.card` (content blocks), `.grid` (responsive layout)

## Key Patterns & Conventions

1. **HTML Structure:** Each page has identical header/nav layout - update navigation links consistently across all HTML files when adding new pages
2. **Responsive Design:** Use `flex-wrap: wrap`, `grid-template-columns: repeat(auto-fit, minmax(...))`, and viewport meta tags
3. **Color Palette:** 
   - Header/Footer: `#0f172a`, `#04171a` (dark navy)
   - Accent: `#1d4ed8` (headings), `#c2c5ce` (hover)
   - Background: `#f4f7fb` (light)
4. **Profile Images:** Use `.profile-img` class with 180px circle borders for consistency (see index.html)
5. **Navigation:** All pages link to `index.html`, `Teaching.html`, and student pages via consistent menu structure

## Common Development Tasks

- **Adding new pages:** Duplicate an existing HTML file, maintain header/nav structure, add to menu links in all files
- **Image optimization:** Place in `image/` folder; reference via relative paths
- **CSS updates:** Modify inline `<style>` blocks; test responsive behavior by resizing browser
- **File naming:** Avoid special characters in filenames (note: "students2 Fist photo.html" uses unusual naming - stick to kebab-case: `students-page-name.html`)

## No Build/Test Setup
This is a static site - no build process, package.json, or testing framework. Simply open HTML files in browser or use VS Code's Live Server extension for local development.
