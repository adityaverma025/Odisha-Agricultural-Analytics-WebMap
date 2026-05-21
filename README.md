Markdown
# Odisha Agricultural Analytics: Interactive Web GIS Dashboard

An interactive, responsive Web GIS application designed to visualize and correlate key agricultural parameters—**Average Rainfall**, **Rice Yield**, and **Fertilizer Application Rates**—across all 30 districts of Odisha, India. 

This project bridges the gap between raw statistical data tables and spatial visualization, allowing users to dynamically explore how environmental inputs directly impact crop productivity at the grassroots level.

🌍 **[Explore the Live Interactive Map Here](https://adityaverma025.github.io/Odisha-Agricultural-Analytics-WebMap/#7/20.210/84.437)**

---

## 🚀 Key Features

* **Dynamic Multi-Layer Toggle:** Built with an expanded layer tree control that allows users to seamlessly switch between three thematic maps:
  * **Average Rainfall (mm)** (Meters/Decimals)
  * **Rice Yield (Kg/Ha)** (Crop Productivity Metrics)
  * **Fertilizer Applied (kg/Ha)** (Input Optimization Scale)
* **Intelligent Data Symbology:** Implemented **Natural Breaks (Jenks)** classification to group district attributes naturally, highlighting geographic variances accurately while maintaining high contrast.
* **Responsive Hover & Interactivity:** Features high-responsiveness with a "Highlight on Hover" feature that lights up district borders, paired with interactive popups utilizing "Visible with Data" inline styling to keep attribute cards completely clean.
* **Localized District Search:** Includes a localized search layout widget allowing users to type and search for specific districts (e.g., Cuttack, Ganjam, Puri) and zoom instantly to their metrics.

---

## 🗺️ Preview

<img width="3200" height="1904" alt="Screenshot 2026-05-21 102125" src="https://github.com/user-attachments/assets/2300bfbf-0fb0-4d0a-96c6-056787477821" />


---

## 🛠️ Tech Stack & Tools

* **Core GIS Platform:** QGIS Desktop 3.44 (Long-Term Release)
* **Web Mapping Engine:** Leaflet (JavaScript library for mobile-friendly interactive maps)
* **Data Pipelines & Parsing:** SQL, Python, QGIS Field Calculator (`to_int` data-type casting)
* **Frontend Web Stack:** HTML5, CSS3, JavaScript (ES6)
* **Deployment & Hosting:** GitHub Pages

---

## 📂 Repository Structure

```text
├── css/                 # Map styles and user-interface layouts
├── js/                  # Leaflet core libraries and configuration code
├── layers/              # Geospatial vector datasets converted to GeoJSON/JS
├── index.html           # Main application entry point webpage
└── README.md            # Project documentation and guide
```

📈 Methodology
Data Pre-processing: Raw agricultural text inputs were cleaned and converted. Text-based string columns (like odisha_agri_Fertilizer) were systematically cast into permanent, query-able numeric fields using the QGIS Field Calculator expression: to_int("odisha_agri_Fertilizer").

Thematic Symbology: Vector polygon layers were duplicated to maintain three distinct, independent visual scales. Inverted color ramps were manually applied to specific variables to match precise design guidelines (e.g., higher values mapped to lighter shades for specialized visual distinction).

Web Deployment: The mapping infrastructure was compiled utilizing the qgis2web parsing engine, optimizing it into a lightweight, fully responsive Leaflet bundle ready for server-less web deployment.

🧑‍💻 Author

Aditya Verma

B.Sc. (Hons.) Agriculture Student

📂 [Check out my GitHub Profile](https://github.com/adityaverma025)

💼 [Connect with me on LinkedIn](https://www.linkedin.com/public-profile/settings/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_self_edit_contact_info%3Be4UT8rXxT%2F%2BHCd%2FA39z5Eg%3D%3D)

Feel free to star ⭐ this repository if you found it useful for agricultural spatial analysis!
