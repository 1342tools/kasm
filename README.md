# KASM - Attack Surface Management Tool (formerly Kanti)

KASM is a web application designed for Attack Surface Management (ASM). It helps you discover, analyze, and manage your organization's digital assets.

## Technology Stack

*   **Backend:** Go (Gin framework)
*   **Frontend:** SvelteKit (with Vite)
*   **Styling:** Tailwind CSS
*   **Database:** SQLite
*   **Visualization:** D3.js, vis-network

## Prerequisites

*   Go 
*   Node.js and npm

## Running the Application

### 1. Backend Setup

The backend server handles the API logic and database interactions.

```bash
# Navigate to the backend directory
cd backend

# Install Go dependencies (if needed, based on go.mod)
go mod tidy

# Run the backend server
go run main.go
```

The backend server will start on `http://localhost:8080` by default.

### 2. Frontend Setup

The frontend provides the user interface.

```bash
# Navigate to the frontend directory
cd frontend

# Install Node.js dependencies
npm install

# Start the frontend development server
npm run dev
```

The frontend development server will start, typically on `http://localhost:5173`. Open this URL in your browser to access the application.

## Building for Production

### Frontend

```bash
cd frontend
npm run build
```

This command builds the optimized frontend assets into the `frontend/build` directory (or as configured in `svelte.config.js`).

### Backend

```bash
cd backend
go build -o kanti-backend main.go
```

This command compiles the backend into an executable file named `kanti-backend`. You would then need to configure a production environment (database, etc.) and run the executable.
