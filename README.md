Initial Folder Structure
- urlShortner(with infinte analytics)


urlShortener/
├── backend/
│   ├── src/
│   │   ├── config/         # DB connection, env vars
│   │   ├── controllers/    # Business logic (shorten, redirect, analytics)
│   │   ├── models/         # DB schemas
│   │   ├── routes/         # API endpoints
│   │   ├── services/       # External APIs, analytics processing
│   │   ├── workers/        # Background jobs (Kafka/Redis queues)
│   │   ├── utils/          # Helper functions
│   │   └── index.js        # Entry point
│   ├── tests/              # Unit/integration tests
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/     # UI components
│   │   ├── pages/          # Page-level components (Next.js/React Router)
│   │   ├── hooks/          # Custom React hooks
│   │   ├── services/       # API calls to backend
│   │   └── App.js
│   ├── public/             # Static assets (logo, icons)
│   └── package.json
│
├── .github/workflows/      # CI/CD configs
├── docker-compose.yml      # For backend, frontend, db, cache
├── README.md
└── package.json            # If you have shared scripts or monorepo mgmt