# Tanvi Patel Portfolio

A portfolio website showcasing Tanvi Patel's work as an urban planner and analyst.

## 🚀 Deployment

This project is deployed on Vercel and works perfectly for static hosting.

## 📁 Project Structure

```
├── index.html          # Main portfolio page
├── work.html           # Work showcase page
├── contact.html        # Contact information
├── styles.css          # Main stylesheet
├── assets/             # Images and media files
└── qgis-project/       # QGIS web map project
    ├── index.html      # Interactive map page
    ├── layers/         # Map data layers
    ├── resources/      # Libraries and resources
    └── styles/         # Map styling
```

## 🗺️ QGIS Map Integration

The QGIS map is fully functional and includes:
- Interactive map layers
- Spatial analysis visualizations
- NSW planning system data
- Sydney LGA information

### Large Files Note

Some large QGIS data files (137MB and 198MB) have been removed from this repository for Vercel compatibility. To restore full map functionality:

1. **Option 1: Host externally** - Upload the large `.js` files to a CDN or file hosting service
2. **Option 2: Use alternative hosting** - Deploy the full project on a platform that supports larger files (Netlify, GitHub Pages with LFS)

### Files to host externally:
- `qgis-project/layers/LGA_2024_AUST_GDA2020_2.js` (137MB)
- `qgis-project/layers/PurchasedHouses2021_1.js` (198MB)

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- QGIS Web Export
- OpenLayers
- Font Awesome Icons

## 📱 Features

- Responsive design
- Interactive QGIS maps
- Professional portfolio layout
- Contact information
- Social media links

## 🔗 Links

- **LinkedIn**: [Tanvi Patel](https://www.linkedin.com/in/tanvi-patel-ua3014/)
- **Email**: tanvipatel2596@gmail.com
- **Portfolio**: [Adobe Portfolio](https://ptanvi2596490a.myportfolio.com/)

## 🚀 Quick Start

1. Clone the repository
2. Open `index.html` in a web browser
3. Navigate through the portfolio pages
4. Access the interactive map at `qgis-project/index.html`

## 📄 License

This project is for portfolio purposes only.
