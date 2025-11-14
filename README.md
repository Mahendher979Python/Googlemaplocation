# Googlemaplocation
✅ GitHub Description (Ready to Copy & Paste)
🏠 Home / Company Location Map Integration
This project includes an interactive Google Map section to display the company’s location on the homepage. The map helps users easily find our office, navigate directions, and understand nearby landmarks.

🌍 Map Features
Custom map styles (light, dark, satellite, simple gray).
Location marker with company details.
Smooth zoom controls.
Fully responsive for mobile and desktop.
Supports multiple address integration, such as Home, Office, Store, or Branch locations.

🗺️ Adding Your Own Map
To change the map style or location, update the JavaScript snippet:

function initMap() {
  const location = { lat: 17.3850, lng: 78.4867 }; // Change to your location

  const map = new google.maps.Map(document.getElementById("map"), {
    zoom: 14,
    center: location,
    styles: mapStyle, // Custom map style
  });

  const marker = new google.maps.Marker({
    position: location,
    map: map,
    title: "Company Location",
  });
}

🎨 Adding Custom Map Styles

Add a custom map style JSON:

const mapStyle = [
  {
    elementType: "geometry",
    stylers: [{ color: "#ebe3cd" }],
  },
  {
    elementType: "labels.text.fill",
    stylers: [{ color: "#523735" }],
  }
];

You can generate styles from:
Google Maps Style Wizard or SnazzyMaps.com

📍 How to Use
Add the map <div id="map"></div> in your HTML.
Include the Google Maps API script with your API key.
Add the JavaScript map initialization code.
Customize the location and map style.

🔧 Technologies Used
HTML
CSS
JavaScript
Google Maps JavaScript API
