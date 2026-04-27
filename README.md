# Puter

An open-source, self-hostable cloud operating system. Run it on your own server and get a full desktop experience in your browser.

## Features

- 🖥️ Full desktop environment in the browser
- 📁 File system with cloud storage
- 🔒 Self-hosted — your data stays on your server
- 🐳 Docker support for easy deployment
- 🌐 Multi-user support

## Quick Start

### Using Docker (recommended)

```bash
# Clone the repo
git clone https://github.com/your-org/puter.git
cd puter

# Copy the example env file
cp .env.example .env

# Start with Docker Compose
docker compose up -d
```

Then open your browser and navigate to `http://localhost:4100`.

### Manual Setup

**Requirements:**
- Node.js 16+
- npm 8+

```bash
# Install dependencies
npm install

# Start the server
npm start
```

## Configuration

Copy `.env.example` to `.env` and edit the values as needed.

| Variable | Description | Default |
|----------|-------------|---------|
| `PUTER_PORT` | Port to listen on | `4100` |
| `PUTER_DATA_DIR` | Directory for persistent data | `./data` |

## Development

```bash
# Install dependencies
npm install

# Run in development mode (with hot reload)
npm run dev
```

## Deployment

See the [Docker workflow](.github/workflows/docker-image.yaml) for how images are built and published.

Pre-built Docker images are available on GitHub Container Registry:

```bash
docker pull ghcr.io/your-org/puter:latest
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

## License

[AGPL-3.0](LICENSE)
