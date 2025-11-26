# NetPrint - IP & Location Detection Service

A sleek, modern web service that automatically detects and displays your public IP address and location information in real-time.

## 🌟 Features

- **Real-time IP Detection**: Automatically detects your public IP address
- **Location Details**: Shows country, city, region, and timezone
- **Network Information**: Displays ISP and AS Number details
- **Dark Mode**: Beautiful dark theme optimized for eye comfort
- **Responsive Design**: Works perfectly on desktop and mobile devices
- **Fast & Lightweight**: Minimal dependencies and fast loading times
- **Privacy Focused**: No tracking or data storage

## 🚀 Live Demo

Visit the live service: [NetPrint on GitHub Pages](https://pourjanali.github.io/NetPrint/)

## 🛠️ Installation

### Option 1: GitHub Pages (Recommended)
1. Fork this repository
2. Enable GitHub Pages in your repository settings
3. Your service will be live at `https://pourjanali.github.io/NetPrint/`

### Option 2: Local Development
```bash
# Clone the repository
git clone https://github.com/pourjanali/NetPrint.git

# Navigate to the project directory
cd NetPrint

# Open index.html in your browser
open index.html
```

### Option 3: Self-hosting
Upload the `index.html` file to any web server or static hosting service.

## 📁 Project Structure

```
NetPrint/
├── index.html          # Main application file
├── favicon.png         # Website favicon
└── README.md          # Project documentation
```

## 🔧 How It Works

NetPrint uses two reliable APIs to fetch your IP and location data:

1. **Primary API**: `ipapi.co/json/` - Provides comprehensive location data
2. **Fallback API**: `ip-api.com/json/` - Backup service for reliability

### Data Points Collected:
- Public IP Address
- Country
- City
- Region/State
- Timezone
- Internet Service Provider (ISP)
- Autonomous System Number (ASN)

## 🌐 API Usage

You can also use NetPrint programmatically:

```bash
# Get your IP information as JSON
curl https://ipapi.co/json/
```

Example response:
```json
{
  "ip": "192.168.1.1",
  "city": "New York",
  "region": "New York",
  "country": "US",
  "timezone": "America/New_York",
  "org": "Example ISP Inc.",
  "asn": "AS12345"
}
```

## 🎨 Customization

### Changing Colors
Edit the CSS variables in the `<style>` section to customize the appearance:

```css
/* Main background */
background-color: #121212;

/* Header gradient */
background: linear-gradient(135deg, #1e3c72, #2a5298);

/* Card background */
background-color: #1e1e1e;
```

### Adding New Data Points
Add new information cards in the HTML:

```html
<div class="info-card">
    <div class="info-label">New Field:</div>
    <div class="info-value" id="new-field">Loading...</div>
</div>
```

And update the JavaScript:
```javascript
document.getElementById('new-field').textContent = data.new_field;
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Areas for Improvement:
- Add IPv6 support
- Implement copy-to-clipboard functionality
- Add network speed test
- Create JSON API endpoint
- Add multiple language support

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **Sponsored by**: [Pourjanali](https://pourjanali.ir/)
- **IP API Services**: [ipapi.co](https://ipapi.co/) & [ip-api.com](https://ip-api.com/)
- **Hosting**: [GitHub Pages](https://pages.github.com/)
- **Font**: [Roboto](https://fonts.google.com/specimen/Roboto) by Google

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/pourjanali/NetPrint/issues) page
2. Create a new issue with detailed information
3. Contact: [Pourjanali Website](https://pourjanali.ir/)

## 🌟 Star History

If you find this project useful, please consider giving it a star ⭐ on GitHub!

---

**Made with ❤️ by [Pourjanali](https://pourjanali.ir/)**

*Simple, fast, and reliable IP detection service*
