# Universal Clock & Weather Widget for Notion

This is a generic, customizable widget—not branded for a specific person or workspace.

## Features
- Automatic greeting, date, and live clock
- Name customization
- City-based weather lookup and refresh
- 12-hour or 24-hour time
- Custom background, card, accent, clock, and text colours
- "Copy custom link" creates a URL with settings in the query string, suitable for a personalized Notion embed
- Responsive layout for narrow embeds

## Publish using GitHub Pages
1. Create a public GitHub repository, e.g. `notion-clock-weather-widget`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. The URL will look like `https://YOUR-USERNAME.github.io/notion-clock-weather-widget/`.
7. Open the published URL, click **Customize**, enter a name and city, choose colours, and click **Apply changes**.
8. Click **Copy custom link**. Paste that personalized URL into Notion using `/embed`.

## How users personalize it
The widget is universal. Each person can use the Customize panel to preview their own name, city, time format and colours. For a shareable, reproducible setup, use **Copy custom link** and embed that URL in Notion.

## Weather and privacy
- Weather and geocoding are provided by Open-Meteo. A network connection is required; no API key is needed for this basic use.
- The city is sent to Open-Meteo's public geocoding API to find weather coordinates.
- The widget does not require a user account or store private credentials.
- GitHub Pages content and URL parameters are public to anyone who has the URL. Do not include sensitive information.
- If a city is entered, the widget uses that city's timezone for both the clock/date and weather. If no city is entered, the clock uses the viewer's device timezone.
<!-- Trigger a fresh Pages build -->
