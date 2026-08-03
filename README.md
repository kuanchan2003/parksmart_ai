# parksmart_ai

ParkSmart AI - Intelligent parking management system powered by AI agents.

## Project Structure

```
parksmart-ai/
├── apps/
│   ├── backend/
│   │   ├── app/
│   │   │   ├── api/          # API routes and endpoints
│   │   │   ├── agents/       # AI agents
│   │   │   ├── core/         # Core configuration and utilities
│   │   │   ├── models/       # Database models
│   │   │   ├── schemas/      # Pydantic schemas
│   │   │   ├── repositories/ # Data access layer
│   │   │   ├── services/     # Business logic
│   │   │   ├── rules/        # Business rules
│   │   │   └── tools/        # AI agent tools
│   │   ├── tests/            # Backend tests
│   │   ├── alembic/          # Database migrations
│   │   ├── pyproject.toml
│   │   └── Dockerfile
│   └── frontend/
│       ├── app/              # Next.js app router
│       ├── components/       # React components
│       ├── features/         # Feature modules
│       ├── hooks/            # Custom React hooks
│       ├── lib/              # Utility libraries
│       ├── types/            # TypeScript types
│       ├── package.json
│       └── Dockerfile
├── docs/                     # Documentation
├── scripts/                  # Utility scripts
├── docker-compose.yml
├── .env.example
├── .gitignore
└── README.md
```

## Tech Stack

- **Backend**: FastAPI, SQLAlchemy, Alembic, LangChain
- **Frontend**: Next.js, React, TypeScript, Tailwind CSS
- **Database**: PostgreSQL
- **Cache**: Redis
- **AI**: OpenAI / LangChain agents

## Getting Started

1. Copy the environment file:
   ```bash
   cp .env.example .env
   ```

2. Start the services with Docker Compose:
   ```bash
   docker-compose up -d
   ```

3. Access the applications:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:8000
   - API Docs: http://localhost:8000/docs

## Development

### Backend

```bash
cd apps/backend
pip install -e ".[dev]"
uvicorn app.main:app --reload
```

### Frontend

```bash
cd apps/frontend
npm install
npm run dev
```

## License

TBD