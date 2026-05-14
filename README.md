# jk-map (JKまっぷ)

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A simple, data-driven interactive map showcasing local businesses and tourist spots in Fukui Prefecture, Japan. This project is a static website built with a single HTML file and a CSV data source.

## Demo

View the live map: **https://code4fukui.github.io/jk-map/**

## Features

- **Interactive Map:** Displays points of interest on a map, powered by OpenStreetMap.
- **Detailed Information:** Click on a point to view details like business name, phone number, description, and regular holidays.
- **Categorized Points:** Businesses are grouped by categories such as dining (`飲食`), shopping (`買い物`), and lodging (`宿泊`).
- **CSV-Powered:** All map data is loaded directly from the `jk-map.csv` file, making it easy to update.
- **Zero-Build:** Runs directly in any modern web browser with no build step required.

## How It Works

The map is rendered using the `<csv-map>` web component, which is imported in `index.html`. This component dynamically fetches data from the `jk-map.csv` file, parses the `geo3x3` location data, and displays the points on the map.

## Usage and Data Customization

To run the project locally, simply open `index.html` in a web browser.

To modify the map's content, edit the `jk-map.csv` file. Add, remove, or update rows to change the points displayed. The CSV file uses the following columns:

- `名前`: Name of the location
- `電話番号`: Phone number
- `カテゴリー`: Category (e.g., 飲食 - Dining, 買い物 - Shopping)
- `icon`: URL for a custom map icon
- `概要`: A short description
- `定休日`: Regular closing days/holidays
- `geo3x3`: Geolocation identifier
- `キャッチコピー`: A marketing catchphrase

## License

This project is available under the MIT License.