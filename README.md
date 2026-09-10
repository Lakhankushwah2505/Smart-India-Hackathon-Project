# Smart-India-Hackathon-Project
Energy and Resource Management For Polar Research Stations



Frontend Folder Structure.

polar-energy-dashboard/
├── public/
│   └── index.html
├── src/
│   ├── api/
│   │   ├── client.js                 # axios/fetch wrapper, base URL config
│   │   ├── energyApi.js              # calls to backend: /status, /forecast, /dispatch
│   │   └── alertsApi.js              # calls for safety/alerts endpoints
│   │
│   ├── assets/
│   │   └── icons/                    # any custom icons/images
│   │
│   ├── components/
│   │   ├── common/
│   │   │   ├── MetricCard.jsx        # reusable stat card (SoC, fuel, etc.)
│   │   │   ├── StatusBadge.jsx       # "nominal / warning / critical" badge
│   │   │   └── Panel.jsx             # generic bordered card wrapper
│   │   │
│   │   ├── dashboard/
│   │   │   ├── DashboardHeader.jsx   # station name + status
│   │   │   ├── MetricsRow.jsx        # battery/fuel/solar/wind cards
│   │   │   ├── EnergyFlowChart.jsx   # stacked bar: solar/wind/diesel over time
│   │   │   ├── ForecastVsActualChart.jsx  # line chart, forecast vs real load
│   │   │   └── AlertsPanel.jsx       # safety/maintenance alert list
│   │   │
│   │   └── layout/
│   │       ├── Sidebar.jsx           # nav (if multi-page: dashboard/history/settings)
│   │       └── TopBar.jsx
│   │
│   ├── hooks/
│   │   ├── useEnergyStatus.js        # polling/live-state hook
│   │   ├── useForecastData.js
│   │   └── useAlerts.js
│   │
│   ├── pages/
│   │   ├── Dashboard.jsx             # main page, composes dashboard/* components
│   │   ├── History.jsx               # past seasons/fuel usage trends (optional)
│   │   └── Settings.jsx              # thresholds, safety margins config (optional)
│   │
│   ├── context/
│   │   └── EnergySystemContext.jsx   # global state: current SoC, fuel, alerts
│   │
│   ├── utils/
│   │   ├── formatters.js             # number/unit formatting (kW, %, days)
│   │   └── constants.js              # thresholds, colors, refresh intervals
│   │
│   ├── styles/
│   │   └── globals.css               # base styles, CSS variables/theme
│   │
│   ├── App.jsx
│   └── main.jsx                      # entry point (if Vite) or index.js (if CRA)
│
├── .env                              # API base URL, keys
├── package.json
├── vite.config.js                    # or react-scripts config if CRA
└── README.md
