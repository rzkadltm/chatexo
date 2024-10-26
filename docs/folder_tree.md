Chatexo/
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py                  # Main entry point for FastAPI app
│   │   ├── core/
│   │   │   ├── config.py            # Configuration settings (e.g., database, API keys)
│   │   │   ├── security.py          # Security-related configurations (auth, JWT)
│   │   ├── api/
│   │   │   ├── __init__.py
│   │   │   ├── routes/              # Routes for different features
│   │   │   │   ├── chat.py          # Chat routes
│   │   │   │   ├── call.py          # Call routes
│   │   │   │   ├── video_call.py    # Video call routes
│   │   │   ├── dependencies.py      # Common dependencies for routes
│   │   ├── models/
│   │   │   ├── __init__.py
│   │   │   ├── user.py              # User model
│   │   │   ├── message.py           # Message model
│   │   │   ├── call_session.py      # Call session model
│   │   ├── schemas/                 # Data validation schemas
│   │   │   ├── __init__.py
│   │   │   ├── user.py
│   │   │   ├── message.py
│   │   │   ├── call_session.py
│   │   ├── services/                # Service layer for business logic
│   │   │   ├── __init__.py
│   │   │   ├── chat_service.py      # Chat service logic
│   │   │   ├── call_service.py      # Call service logic
│   │   ├── utils/                   # Utility functions
│   │   │   ├── __init__.py
│   │   │   ├── db.py                # Database connection and setup
│   │   │   ├── logging.py           # Custom logging configuration
│   ├── tests/                       # Unit and integration tests for backend
│   │   ├── __init__.py
│   │   ├── test_main.py
│   │   ├── test_chat.py
│   │   ├── test_call.py
│   ├── Dockerfile                   # Dockerfile for backend
│   ├── requirements.txt             # Python dependencies for FastAPI
│   ├── alembic/                     # Alembic for database migrations
│   │   ├── versions/
│   │   ├── env.py
│   │   ├── README
│   │   ├── alembic.ini
│   ├── README.md                    # Backend documentation
│
├── frontend/
│   ├── public/                      # Public assets
│   │   ├── index.html
│   │   ├── favicon.ico
│   ├── src/
│   │   ├── App.jsx                  # Root component
│   │   ├── index.jsx                # Entry point
│   │   ├── components/              # Reusable components
│   │   │   ├── ChatComponent.jsx    # Chat UI component
│   │   │   ├── CallComponent.jsx    # Call UI component
│   │   │   ├── VideoCallComponent.jsx # Video call UI component
│   │   ├── pages/                   # Application pages
│   │   │   ├── HomePage.jsx
│   │   │   ├── ChatPage.jsx
│   │   │   ├── CallPage.jsx
│   │   ├── hooks/                   # Custom hooks
│   │   ├── services/                # API calls and frontend service logic
│   │   │   ├── chatService.js       # API calls for chat
│   │   │   ├── callService.js       # API calls for call
│   │   │   ├── videoCallService.js  # API calls for video call
│   ├── tests/                       # Unit and integration tests for frontend
│   │   ├── App.test.js
│   ├── Dockerfile                   # Dockerfile for frontend
│   ├── package.json                 # Node dependencies
│   ├── vite.config.js               # Configuration for Vite (or Webpack, if chosen)
│   ├── README.md                    # Frontend documentation
│
├── docker-compose.yml               # Docker Compose for orchestrating containers
├── .env                             # Environment variables
├── .gitignore                       # Ignored files and directories
├── README.md                        # Project-level documentation
└── docs/
    ├── architecture.md              # Architectural overview
    ├── api_docs.md                  # API documentation
    ├── setup_guide.md               # Setup and installation guide
