# Yoshino Digital Map (kidssafe-yoshino)

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

This repository contains the data and code for the **Yoshino District Discovery Map** (吉野地区発見マップ), an interactive community safety and discovery map for the Yoshino district in Echizen City, Japan.

The map is built using the [KidsSafe project by Code for FUKUI](https://github.com/code4fukui/kidssafe/) and is designed to be easily updated by community members using simple CSV files.

## Features

- **Interactive Map**: View community-submitted points of interest, safety locations (like AEDs), and local landmarks.
- **CSV-Powered**: All point data is managed through simple CSV files (e.g., [`aed.csv`](aed.csv)), which can be edited with spreadsheet software like Excel or Numbers.
- **Route Overlays**: Displays GeoJSON data for paths and routes, such as school routes (`tsugakuro.geojson`).
- **Rich Details**: Click on any point to see more information, including descriptive text, photos, and a direct link to Google Street View.
- **Keyword Filter**: Instantly filter visible map points by typing in the search bar.
- **Mobile-Friendly**: A responsive design that works on any device and can be added to your smartphone's home screen for quick access.
- **Multilingual Support**: The map interface can be switched to other languages.

## How to Manage Map Data

Anyone can contribute to the map by updating the data files in this repository.

### Updating Existing Data

1.  Navigate to the data file you want to change (e.g., [`yoshino_R7tanken_07shisetsu.csv`](yoshino_R7tanken_07shisetsu.csv)).
2.  Click the "Download raw file" button to save it to your computer.
3.  Open and edit the file in a spreadsheet program.
4.  Upload the modified file back to the repository to update the map.

### Adding a New Data Layer

1.  Download the [`template.csv`](template.csv) file.
2.  Open it in a spreadsheet program and add your new points of interest. Each point should have at least a `lat` (latitude) and `lng` (longitude). You can add any other columns you need (e.g., `名称` for name, `説明` for description, `写真` for a photo).
3.  Save the file in CSV format with a descriptive name (e.g., `historic_sites.csv`).
4.  Download the [`index.csv`](index.csv) file.
5.  Add a new row to `index.csv` to register your new data layer, specifying the filename, the name to display on the map, and a default icon.
6.  Upload both your new CSV file and the updated `index.csv` to the repository.

### Adding Custom Icons

1.  Prepare your icon as a PNG image with a unique, simple filename (e.g., `shrine_icon.png`).
2.  Upload the image file to the [`icon`](icon) folder in this repository.
3.  In your data CSV or in [`index.csv`](index.csv), enter the new filename in the `icon` column for the corresponding data points.
4.  Commit the changes. The map will now display your custom icon.

## License

MIT License — see [LICENSE](LICENSE).