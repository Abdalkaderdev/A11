# A11: 360° Virtual Apartment Tour

## Overview
A11 is a Marzipano-based 360° virtual tour web application for exploring an apartment interactively. Users can navigate between rooms, zoom, and view hotspots for information and navigation.

## Features
- 360° panoramic views of all apartment spaces
- Interactive scene switching between rooms
- View control buttons for navigation and zoom
- Fullscreen mode support (with fallback)
- Autorotate toggle
- Hotspots for navigation and information
- Responsive design for desktop and mobile

## Available Spaces
The following spaces are available in this virtual tour:

- bathroom
- kitchen
- hall
- balcony
- room
- edition view
- bathroom2
- master bathroom
- master room
- balcony.

## Technology Stack
- [Marzipano](http://www.marzipano.net/) (panorama viewer)
- JavaScript (ES5/ES6)
- HTML5 & CSS3
- [screenfull.js](https://github.com/sindresorhus/screenfull.js) (fullscreen API)
- [bowser](https://github.com/lancedikson/bowser) (browser detection)

## How to Use
- **Navigation:** Use the on-screen arrows or drag with your mouse/finger to look around.
- **Zoom:** Use the plus (+) and minus (-) buttons or your mouse wheel.
- **Switch Scenes:** Click on a room name in the scene list to jump to that space.
- **Fullscreen:** Click the fullscreen button to enter/exit fullscreen mode. If not supported, an alert will notify you.
- **Autorotate:** Toggle autorotation with the play/pause button.
- **Hotspots:** Click hotspots in the view to navigate or see more info.

## Project Structure
```
a11/
  app-files/
    data.js           # Tour configuration and scene data
    index.html        # Main HTML file
    index.js          # Main JavaScript logic
    style.css         # Stylesheet
    img/              # UI and hotspot images
    tiles/            # Panorama image tiles for each scene
    vendor/           # Third-party libraries (Marzipano, screenfull, bowser, etc.)
  LICENSE.txt         # License information
  README.md           # This documentation
```

## Local Development
1. **Install a local web server** (required for Marzipano to load images):
   - Python 3: `python -m http.server 8000`
   - Node.js: `npx serve app-files`
2. **Open your browser** and go to `http://localhost:8000/app-files/` (or the appropriate URL for your server).
3. **Enjoy the tour!**

## Customization Tips
- **Add/Edit Scenes:** Modify `app-files/data.js` to add or update scenes, hotspots, and settings.
- **Change UI:** Edit `app-files/style.css` and `app-files/index.html` for layout and style changes.
- **Replace Images:** Update images in `app-files/img/` and panorama tiles in `app-files/tiles/`.
- **Settings:** Toggle features like fullscreen and view controls in the `settings` object in `data.js`.

## License
This project is based on the Marzipano Tool and is licensed under the Apache License 2.0. See [LICENSE.txt](LICENSE.txt) for details. Some third-party libraries are under their own licenses.

## Author & Contact
- Original template: Google Inc. (Marzipano Tool)
- Customization: [Your Name Here]
- Contact: [your.email@example.com] 