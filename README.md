# 🌐 Facebook Clone - Full Featured Social Media UI

A complete, pixel-perfect Facebook clone featuring a login page, signup page, and home feed with stories, posts, and real-time interactions.

![Facebook Clone](https://img.shields.io/badge/Facebook-Clone-1877F2?style=for-the-badge&logo=facebook&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Deployed](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)

## 🎯 Features

### 🔐 Login Page (`index.html`)
- Authentic Facebook login interface
- Responsive design
- Email/phone number input
- Password field with security
- "Forgotten password" link
- "Create new account" button
- Multi-language footer
- Complete footer with links

### ✍️ Signup Page (`signup.html`)
- Modal-style signup form
- First name and surname fields
- Email/phone registration
- Password creation
- Date of birth selection (Day, Month, Year dropdowns)
- Gender selection (Female, Male, Custom)
- Terms and privacy policy agreement
- Responsive design

### 🏠 Home Feed (`home.html`)
- **Header Navigation**
  - Facebook logo
  - Search bar
  - Navigation icons (Home, Watch, Marketplace, Groups, Gaming)
  - Menu, Messenger, Notifications
  - Profile menu
  
- **Left Sidebar**
  - User profile
  - Friends
  - Groups
  - Marketplace
  - Watch
  - Memories
  - Saved items
  - Pages
  - Events
  
- **Main Feed**
  - Stories section (Create + View stories)
  - Create post box
  - News feed posts with:
    - Profile pictures
    - Post content
    - Images
    - Like, Comment, Share buttons
    - Reaction counts
    - Comment counts
    - Share counts
  
- **Right Sidebar**
  - Sponsored content
  - Contacts list with online status
  - Video call options

## 🚀 Live Demo

**Website URL:** https://51.120.24.98/

## 📁 Project Structure

```
facebook_signup_page_clone/
├── index.html          # Login page (main entry point)
├── signup.html         # User registration page
├── home.html           # Home feed after login
├── login.html          # Legacy redirect file
├── style.css           # Login page styles
├── signup.css          # Signup page styles
├── home.css            # Home feed styles
├── login.css           # Legacy styles
├── signu.css           # Legacy signup styles
├── README.md           # Project documentation
└── .github/
    └── workflows/
        └── deploy.yml  # CI/CD GitHub Actions workflow
```

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with Flexbox & Grid
- **Font Awesome 6.4.0** - Icons library
- **Responsive Design** - Mobile-first approach
- **GitHub Actions** - Automated deployment
- **Azure VM** - Hosting environment
- **Nginx** - Web server

## 📦 Installation & Setup

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/anshuman018/facebook_signup_page_clone.git
   cd facebook_signup_page_clone
   ```

2. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   # Or use a local server:
   python -m http.server 8000
   # Then visit: http://localhost:8000
   ```

### Production Deployment

The project uses automated CI/CD with GitHub Actions:

1. **Push to main branch**
   ```bash
   git add .
   git commit -m "Your changes"
   git push origin main
   ```

2. **Automatic deployment**
   - GitHub Actions triggers on push
   - Connects to Azure VM via SSH
   - Runs deployment script
   - Updates live site automatically

## 🔧 CI/CD Configuration

### GitHub Secrets Required
- `VM_HOST` - Azure VM IP address
- `VM_USER` - SSH username
- `DEPLOY_KEY` - SSH private key

### Deployment Script (`/home/azureuser/deploy.sh`)
```bash
#!/bin/bash
cd /var/www/html
git pull origin main
sudo systemctl reload nginx
```

## 🎨 Design Features

- ✅ Pixel-perfect Facebook UI replication
- ✅ Responsive design (Mobile, Tablet, Desktop)
- ✅ Smooth hover effects
- ✅ Custom scrollbars
- ✅ Modal overlays
- ✅ Grid and Flexbox layouts
- ✅ Professional color scheme
- ✅ Font Awesome icons
- ✅ Form validation styling

## 📱 Responsive Breakpoints

- **Desktop:** > 1100px
- **Tablet:** 768px - 1100px
- **Mobile:** < 768px

## 🌟 Pages Navigation

```
index.html (Login) → signup.html (Sign Up)
                  ↓
            home.html (Home Feed)
```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

## 👨‍💻 Author

**Anshuman**
- GitHub: [@anshuman018](https://github.com/anshuman018)

## 📄 License

This project is for educational purposes only. Facebook and its assets are trademarks of Meta Platforms, Inc.

## 🙏 Acknowledgments

- Design inspiration from [Facebook](https://facebook.com)
- Icons from [Font Awesome](https://fontawesome.com)
- Hosted on Azure VM
- Deployed with GitHub Actions

## 📞 Support

For issues or questions, please open an issue in the GitHub repository.

---

⭐ **Star this repo if you found it helpful!**

**Made with ❤️ by Anshuman**