# Smart-India-Hackathon-Project
Energy and Resource Management For Polar Research Stations



## FRONTEND FOLDER STRUCTURE

```
frontend/
├── public/
│   ├── favicon.ico
│   └── index.html
├── src/
│   ├── assets/                 # Static images, icons, station diagrams
│   ├── components/
│   │   ├── common/             # Buttons, cards, badges, loaders
│   │   ├── dashboard/
│   │   │   ├── MetricCard.jsx
│   │   │   ├── EnergyFlowChart.jsx
│   │   │   ├── ForecastChart.jsx
│   │   │   ├── AlertsPanel.jsx
│   │   │   └── StatusHeader.jsx
│   │   └── layout/
│   │       ├── Sidebar.jsx
│   │       ├── Navbar.jsx
│   │       └── PageLayout.jsx
│   ├── pages/
│   │   ├── Dashboard.jsx        # Main energy overview page
│   │   ├── Forecasts.jsx        # Detailed forecast vs actual views
│   │   ├── Alerts.jsx           # Full alert/maintenance log
│   │   └── Settings.jsx         # Thresholds, safety margins config
│   ├── services/
│   │   ├── api.js               # Axios/fetch instance, base config
│   │   ├── energyService.js      # Endpoints: battery, solar, wind, diesel
│   │   ├── forecastService.js    # Forecast data endpoints
│   │   └── alertService.js       # Alerts/safety endpoints
│   ├── hooks/
│   │   ├── useEnergyData.js      # Custom hook for live/polled energy state
│   │   ├── useForecastData.js
│   │   └── useAlerts.js
│   ├── context/
│   │   └── DashboardContext.jsx  # Global state (station status, theme, etc.)
│   ├── utils/
│   │   ├── formatters.js         # Number/date/unit formatting
│   │   └── constants.js          # Thresholds, color codes, labels
│   ├── styles/
│   │   ├── globals.css
│   │   └── variables.css
│   ├── App.jsx
│   ├── main.jsx                  # Entry point (Vite) or index.js (CRA)
│   └── routes.jsx                # Route definitions
├── .env.example
├── .gitignore
├── package.json
├── vite.config.js                # or webpack config if using CRA
└── README.md
```
