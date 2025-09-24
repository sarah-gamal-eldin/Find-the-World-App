# 🌍 Find the World – Interactive Geography Quiz

**Find the World** is a web-based interactive geography quiz that challenges users to locate countries on a dynamic map. The application leverages **MapLibre GL** and **PMTiles** to deliver a smooth, responsive, and interactive map experience using **Natural Earth** vector tile sources.  

## 🔍 Features

- **Interactive Quiz Gameplay**: Users click on countries to answer questions. Immediate feedback is provided.  
- **Dynamic Map Styling**: Animated countries with hover effects, vibrant fill and outline colors.  
- **Responsive & Dark Themed UI**: Works on both desktop and mobile, with a dark raster basemap for better visual contrast.  
- **PMTiles Integration**: Efficient storage and fast retrieval of vector tiles for a smooth interactive experience.  

---

## 🌐 Live Demo

Try the app directly in your browser:  
[[https://pub-1986f349473349489dd23c0053575aad.r2.dev/app_data/app.html](https://pub-1986f349473349489dd23c0053575aad.r2.dev/app_data/app.html](https://pub-1986f349473349489dd23c0053575aad.r2.dev/app_data/app-1.html)

---

## 🗺️ Technical Details

### Map Data Sources

The app uses **Natural Earth** vector tiles (converted to PMTiles) for countries:

| Layer     | Source                     | PMTiles URL |
|-----------|----------------------------|-------------|
| Countries | Natural Earth 1:50m Admin 0 Countries | `https://pub-1986f349473349489dd23c0053575aad.r2.dev/app_data/admin_0_countries.pmtiles` |

### Map Configuration

- **Base Layer**: Dark raster tiles from CARTO (`dark_nolabels`), tile size 256.  
- **Vector Layers**:  
  - Countries: `fill` and `line` with hover effects and dynamic opacity.  
- **Interactivity**:  
  - Click on any country to show its name, whether the answer is correct or not.  
  - “Try Again” button to retry for incorrect clicks.  
  - Hover animations and interactive feedback to improve UX.  

### Technology Stack

- **Frontend**: HTML, CSS, JavaScript  
- **Mapping**: MapLibre GL JS  
- **Tile Storage**: PMTiles (vector tiles format)  
- **Tile Sources**: Natural Earth vector datasets, converted to PMTiles  
- **Raster Basemap**: CARTO Dark theme (`dark_nolabels`)  

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/find-the-world.git
cd find-the-world



