# Ecommerce Stationery & Sports Store - GitHub Wiki Setup

This repository contains the documentation for the Ecommerce Stationery & Sports Store project, formatted for GitHub Wiki.

## 📋 Contents

- **Home.md** - Main wiki page with dropdown navigation
- **wiki.txt** - Original HTML documentation
- **Delivery_Pickup_Flow.png** - Flow diagram for delivery/pickup process
- **Ecommerce_Stationery_Sports_Presentation.pdf** - Project presentation
- **Ecommerce_Stationery_Sports_Report.pdf** - Project report

## 🚀 Setting up GitHub Wiki

### Option 1: Using GitHub's Wiki Feature

1. **Enable Wiki on your repository:**
   - Go to your GitHub repository
   - Click on "Settings" tab
   - Scroll down to "Features" section
   - Check "Wikis" to enable it

2. **Create the Home page:**
   - Click on the "Wiki" tab in your repository
   - Click "Create the first page"
   - Copy the contents of `Home.md` from this repository
   - Paste it into the wiki editor
   - Click "Save Page"

### Option 2: Using GitHub CLI

```bash
# Clone the wiki repository (if it exists)
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.wiki.git

# Copy the Home.md file
cp Home.md /path/to/wiki/repo/

# Commit and push
cd /path/to/wiki/repo/
git add Home.md
git commit -m "Add main wiki page with dropdown navigation"
git push origin main
```

### Option 3: Manual Setup

1. Create a new repository named `YOUR_REPO.wiki`
2. Upload the `Home.md` file as the main page
3. The wiki will be automatically available at `https://github.com/YOUR_USERNAME/YOUR_REPO/wiki`

## 🎯 Features of the Wiki

- **Dropdown Navigation**: Easy switching between different documentation pages
- **Responsive Design**: Works well on desktop and mobile devices
- **Clean Markdown**: Properly formatted for GitHub's markdown renderer
- **Interactive Elements**: JavaScript-powered page switching

## 📄 Wiki Pages

1. **Product Listing App (MVP)** - Initial product browsing functionality
2. **End-Consumer App** - Full ecommerce platform for customers
3. **Admin Dashboard** - Management interface for shop owners

## 🔧 Customization

You can customize the wiki by:

- Modifying the CSS styles in the `<style>` section
- Adding more pages to the dropdown
- Changing colors and fonts
- Adding images or diagrams

## 📝 Notes

- GitHub Wikis support HTML, CSS, and JavaScript
- The dropdown navigation works client-side
- All content is preserved in a single markdown file for easy maintenance
- The wiki is automatically versioned with Git

## 🤝 Contributing

To contribute to the documentation:

1. Edit the `Home.md` file
2. Test the changes locally
3. Submit a pull request or update the wiki directly

---

**Note**: Make sure to replace `YOUR_USERNAME` and `YOUR_REPO` with your actual GitHub username and repository name.
