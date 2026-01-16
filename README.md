# BattleGuess Website

A modern, responsive marketing website for the BattleGuess mobile app - an interactive educational platform for learning historical battles.

## 🎯 About BattleGuess

BattleGuess is an educational mobile app that helps users learn about historical battles through interactive quizzes, maps, and engaging narratives. The app covers six historical eras from ancient times to modern warfare.

## 🚀 Features

- **Responsive Design**: Works beautifully on desktop, tablet, and mobile devices
- **Modern UI**: Clean, modern design using BattleGuess color scheme (orange/amber theme)
- **Smooth Animations**: Scroll-triggered animations and interactive elements
- **Mobile Menu**: Hamburger menu for mobile navigation
- **SEO Optimized**: Semantic HTML and meta tags for better search visibility

## 📁 Project Structure

```
BattleGuess-Website/
├── index.html      # Main HTML file
├── styles.css      # All CSS styles and animations
├── script.js       # JavaScript for interactivity
└── README.md       # This file
```

## 🛠️ Setup

1. **Clone or download** this repository to your local machine

2. **Open the website**:
   - Simply open `index.html` in your web browser
   - Or use a local development server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (if you have http-server installed)
     npx http-server
     
     # Using PHP
     php -S localhost:8000
     ```

3. **View the website**:
   - Navigate to `http://localhost:8000` in your browser

## 🎨 Customization

### Colors

The website uses CSS variables defined in `styles.css`. You can easily change the color scheme by modifying these variables:

```css
:root {
    --primary: #F97316;        /* Main orange color */
    --secondary: #FDBA74;      /* Light orange */
    --accent: #C2410C;         /* Dark orange */
    /* ... more colors */
}
```

### Content

- **Hero Section**: Edit the hero title, description, and CTA buttons in `index.html`
- **Features**: Modify the feature cards in the Features section
- **Eras**: Update the era cards with your specific battles and content
- **Download Links**: Update the App Store and Google Play links in the Download section

## 📱 Sections

1. **Hero**: Main landing section with app overview and stats
2. **Features**: Highlights key app features with icons
3. **Eras**: Showcases six historical eras covered by the app
4. **How It Works**: Simple 3-step process explanation
5. **Download**: Call-to-action with app store links
6. **Footer**: Links and copyright information

## 🌐 Deployment & Hosting

This is a static website (HTML, CSS, JavaScript only), so it can be hosted on any static hosting service. Here are several popular options:

### Option 1: GitHub Pages (Free & Easy)

**Best for:** Quick free hosting with automatic deployments

1. **Create a GitHub repository:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/BattleGuess-Website.git
   git push -u origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** > **Pages** (left sidebar)
   - Under "Source", select **main** branch and `/ (root)` folder
   - Click **Save**

3. **Your site will be live at:**
   - `https://YOUR_USERNAME.github.io/BattleGuess-Website`

**Note:** If you use a custom domain, add a `CNAME` file in the root directory with your domain name.

---

### Option 2: Netlify (Recommended - Free & Easy)

**Best for:** Easy deployment with custom domain support and automatic HTTPS

#### Method A: Drag & Drop (Quickest)
1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag and drop your entire `BattleGuess-Website` folder
3. Your site is instantly live!

#### Method B: Git Integration (Automatic Deployments)
1. **Push to GitHub** (if you haven't already)
2. **Sign up/Login** at [netlify.com](https://www.netlify.com)
3. **Click "Add new site" > "Import an existing project"**
4. **Connect to GitHub** and select your repository
5. **Configure build settings:**
   - Build command: (leave empty)
   - Publish directory: `/` (root)
6. **Click "Deploy site"**
7. **Your site will be live** at `https://random-name-123.netlify.app`

#### Custom Domain (Netlify):
1. Go to **Site settings** > **Domain management**
2. Click **Add custom domain**
3. Follow the DNS setup instructions
4. SSL certificate is automatically provisioned (free!)

---

### Option 3: Vercel (Free & Fast)

**Best for:** Fast global CDN and excellent developer experience

#### Using Vercel CLI:
1. **Install Vercel CLI:**
   ```bash
   npm i -g vercel
   ```

2. **Deploy:**
   ```bash
   cd BattleGuess-Website
   vercel
   ```

3. **Follow the prompts:**
   - Set up and deploy? **Yes**
   - Which scope? (select your account)
   - Link to existing project? **No**
   - Project name? (press Enter for default)
   - Directory? (press Enter for `.`)

4. **Your site is live!** at `https://your-project.vercel.app`

#### Using Vercel Dashboard:
1. Go to [vercel.com](https://vercel.com) and sign up/login
2. Click **"Add New Project"**
3. Import your GitHub repository
4. Click **Deploy** (no build settings needed for static sites)

---

### Option 4: Cloudflare Pages (Free)

**Best for:** Fast CDN with excellent free tier

1. **Sign up/Login** at [pages.cloudflare.com](https://pages.cloudflare.com)
2. **Create a project** and connect your GitHub repository
3. **Build settings:**
   - Framework preset: **None**
   - Build command: (leave empty)
   - Build output directory: `/`
4. **Click "Save and Deploy"**
5. Your site will be live at `https://your-project.pages.dev`

---

### Option 5: Firebase Hosting (Free)

**Best for:** Integration with other Firebase services

1. **Install Firebase CLI:**
   ```bash
   npm install -g firebase-tools
   ```

2. **Login:**
   ```bash
   firebase login
   ```

3. **Initialize Firebase:**
   ```bash
   firebase init hosting
   ```
   - Select existing project or create new
   - Public directory: `.` (current directory)
   - Single-page app? **No**
   - Automatic builds? **No**

4. **Deploy:**
   ```bash
   firebase deploy
   ```

5. Your site will be live at `https://YOUR_PROJECT_ID.web.app`

---

### Option 6: Surge.sh (Free & Simple)

**Best for:** Command-line deployment, very simple

1. **Install Surge:**
   ```bash
   npm install -g surge
   ```

2. **Deploy:**
   ```bash
   cd BattleGuess-Website
   surge
   ```
   - Enter your email
   - Enter project domain (or press Enter for random)
   - Press Enter to confirm

3. Your site is live! Free custom domains available.

---

### Option 7: AWS S3 + CloudFront

**Best for:** Enterprise scale and AWS integration

1. Create an S3 bucket and enable static website hosting
2. Upload all files to the bucket
3. Configure CloudFront distribution
4. Point your domain to CloudFront

(More complex setup - see [AWS documentation](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html))

---

## 🚀 Quick Comparison

| Platform | Free Tier | Custom Domain | Ease of Use | Best For |
|----------|-----------|---------------|-------------|----------|
| **GitHub Pages** | ✅ Yes | ✅ Yes | ⭐⭐⭐⭐⭐ | Open source projects |
| **Netlify** | ✅ Yes | ✅ Yes | ⭐⭐⭐⭐⭐ | Most users (recommended) |
| **Vercel** | ✅ Yes | ✅ Yes | ⭐⭐⭐⭐⭐ | Developers |
| **Cloudflare Pages** | ✅ Yes | ✅ Yes | ⭐⭐⭐⭐ | Fast CDN |
| **Firebase** | ✅ Yes | ✅ Yes | ⭐⭐⭐ | Google ecosystem |
| **Surge** | ✅ Yes | ✅ Yes | ⭐⭐⭐⭐⭐ | Quick CLI deploys |

---

## 📝 Post-Deployment Checklist

After hosting your site:

- [ ] Test all pages load correctly
- [ ] Verify navigation links work
- [ ] Test mobile responsiveness
- [ ] Set up custom domain (optional)
- [ ] Enable HTTPS (usually automatic)
- [ ] Test contact forms/links (if applicable)
- [ ] Submit to Google Search Console (for SEO)
- [ ] Share your live URL!

---

## 🔗 Custom Domain Setup

Most platforms support custom domains:

1. **Purchase a domain** (Namecheap, Google Domains, etc.)
2. **Add domain in hosting platform:**
   - Netlify: Site settings > Domain management
   - Vercel: Project settings > Domains
   - GitHub Pages: Repository settings > Pages
3. **Configure DNS:**
   - Add CNAME or A record as instructed by your host
4. **Wait for SSL** (usually automatic, takes a few minutes)

---

## 💡 Recommendation

For most users, **Netlify** or **Vercel** are the best choices because they:
- Are completely free
- Support custom domains with free SSL
- Have automatic deployments from Git
- Are very easy to set up
- Offer great performance globally

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 License

This project is created for BattleGuess app. Modify and use as needed for your project.

## 🤝 Contributing

Feel free to submit issues or pull requests if you'd like to improve the website.

## 📞 Support

For questions or support, please contact the BattleGuess team.

---

Built with ❤️ for BattleGuess
