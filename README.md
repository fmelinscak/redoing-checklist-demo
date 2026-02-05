# DOI Research Matrix App

A simple, static, single-page, frontend-only application for managing DOI research data.

## Features

- **DOI Input**: Enter a DOI to automatically fetch article title from Crossref API
- **Title Field**: Auto-populated from DOI or manually editable
- **Assessment Matrix**: Radio button matrix for data collection with placeholder labels
- **Data Export**: Download data as JSON or PDF
- **Data Persistence**: Automatically saves data to browser localStorage

## Technologies Used

- Vue.js 3 (CDN)
- Bootstrap 5 (CDN)
- jsPDF (CDN)
- Crossref API

## Usage

1. Open `index.html` in a web browser
2. **(Optional)** Edit the `mailto` parameter in the Crossref API call (line ~189) with your contact email for better API support
3. Enter a DOI (e.g., `10.1371/journal.pone.0000000`)
4. The title will be automatically fetched from Crossref
5. Fill in the assessment matrix by selecting radio buttons
6. Download your data using the JSON or PDF buttons
7. Data is automatically saved and will persist across browser sessions

## Local Development

Simply open the `index.html` file in your browser. No build process or server required.

For development with live reload, you can use any simple HTTP server:

```bash
# Python 3
python3 -m http.server 8080

# Node.js (with http-server)
npx http-server -p 8080
```

Then visit `http://localhost:8080/index.html`