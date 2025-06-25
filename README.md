# Slot Game Monorepo

This is a monorepo for a production-ready slot game, containing:

- **math-sdk**: Python backend for math/game logic
- **web-sdk**: SvelteKit + Pixi.js frontend, with Storybook and component libraries

## Getting Started

### Prerequisites
- Node.js 18.x (for web-sdk)
- Python 3.12+ (for math-sdk)
- [pnpm](https://pnpm.io/) (for JS package management)

### Setup
```bash
# Install JS dependencies
cd web-sdk
pnpm install

# (Optional) Set up Python venv for math-sdk
cd ../math-sdk
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Running the Frontend
```bash
cd web-sdk
pnpm run dev --filter=slot
```

### Running Storybook
```bash
cd web-sdk
pnpm run storybook --filter=slot
```

### Running the Backend
```bash
cd math-sdk
source venv/bin/activate
python your_backend_entry.py
```

---

