# Windows Setup Instructions

## Prerequisites

- Node.js >= 22.16
- pnpm >= 10.22.0

Install pnpm if not already installed:
```bash
npm install -g pnpm
```

## Setup Steps

### 1. Clone and Pull Latest
```bash
git pull
```

### 2. Install Dependencies
```bash
pnpm install
```

### 3. Build (First Time Only)
```bash
pnpm build > build.log 2>&1
```

Check for build errors:
```bash
tail -n 20 build.log
```

### 4. Start Development Server
```bash
pnpm dev
```

This starts:
- **Backend:** http://localhost:5678
- **Frontend:** http://localhost:8080

## Other Commands

| Command | Description |
|---------|-------------|
| `pnpm dev` | Start backend + frontend only |
| `pnpm dev:all` | Start all packages (slower) |
| `pnpm dev:be` | Start backend only |
| `pnpm dev:fe` | Start frontend only |
| `pnpm build` | Build all packages |
| `pnpm test` | Run all tests |
| `pnpm lint` | Lint code |
| `pnpm typecheck` | Run type checks |
