# Weather Web App

A browser-based weather application built with HTML, CSS, and vanilla JavaScript. It shows current conditions, hourly forecasts, a 5-day forecast, and outdoor activity suggestions. The project was developed as a SheCodes Plus final project.

**Live demo:** [weather-app-shemmee.netlify.app](https://weather-app-shemmee.netlify.app)

## Project location

All source code is in the `Weather-App/` folder:

```
weather app/
└── Weather-App/
    ├── index.html          # Main page and UI structure
    ├── package.json        # Parcel dev server and build scripts
    ├── src/
    │   ├── app.js          # Weather logic, APIs, carousel
    │   └── style.css       # Layout and styling
    ├── images/             # Icons, background, activity illustrations
    ├── .github/workflows/  # GitHub Pages deployment
    ├── LICENSE
    └── README.md           # Upstream project readme
```

## Features

- **City search** — Type a city name and press Enter to load weather data.
- **Geolocation** — On load, requests browser location and shows local weather (if permission is granted).
- **Current weather** — City, country, temperature (°C), condition text, and icon.
- **Temperature toggle** — Switch display between Celsius and Fahrenheit.
- **Today's forecasts** — Next 6 hourly slots with time, icon, and temperature.
- **5-day forecast** — Daily min/max temperatures, icons, and descriptions.
- **Activity carousel** — Rotating outdoor activity suggestions with prev/next controls and auto-advance every 5 seconds.
- **Live date and time** — Current weekday, date, and 12-hour clock on the main card.

## Tech stack

| Layer        | Technology                          |
|-------------|--------------------------------------|
| Markup      | HTML5                                |
| Styling     | CSS3 (Poppins via Google Fonts)      |
| Logic       | Vanilla JavaScript                 |
| HTTP        | Axios (CDN), `fetch`                 |
| Icons       | Font Awesome                         |
| Dev server  | Parcel (`parcel-bundler`)            |
| Hosting     | Netlify (demo), GitHub Pages (workflow)|

## APIs used

| API | Purpose |
|-----|---------|
| [SheCodes Weather API](https://www.shecodes.io/learn/apis/weather) | Current weather, 5-day forecast, city search |
| [OpenWeatherMap API](https://openweathermap.org/) | Hourly forecast data (`/data/2.5/forecast`) |

API keys are configured in `Weather-App/src/app.js`. For your own deployment, replace them with your keys and avoid committing secrets to public repos.

## Getting started

### Option 1 — Open in browser (quickest)

1. Open `Weather-App/index.html` in a modern browser (Chrome, Edge, Firefox).
2. Allow location access when prompted, or search for a city in the search bar.

### Option 2 — Run with Parcel (recommended for development)

```bash
cd "Weather-App"
npm install
npm start
```

- `npm start` — Starts Parcel and opens the app.
- `npm run build` — Production build via Parcel.

## How to use

1. **Search:** Enter a city name in **Search City** and press **Enter**.
2. **Your location:** Allow geolocation when the page loads to see weather for your position.
3. **Units:** Use **Convert to Fahrenheit** / **Convert to Celsius** under the main temperature.
4. **Activities:** Use the chevron buttons or wait for the carousel to auto-rotate.

## Deployment

- **Netlify:** Referenced in the app footer as the hosted environment for the public demo.
- **GitHub Pages:** `.github/workflows/static.yml` deploys the repository to GitHub Pages on pushes to `main`.

## Credits

- Coded by [Chaimae Lamirine](https://www.shecodes.io/graduates/73033-chaimae-lamirine)
- Open source: [github.com/shemmee/Weather-App](https://github.com/shemmee/Weather-App)
- Illustrations: [Icons8 — 3D Casual Life](https://icons8.com/illustrations/style--3d-casual-life)
- SheCodes Plus workshop project

## License

The repository includes a **GNU GPL v3** license file (`Weather-App/LICENSE`). See that file for full terms.

---

*Local copy path: `c:\Users\manoj\Desktop\plm\weather app`*
