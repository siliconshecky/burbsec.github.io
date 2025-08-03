# BurbSec

A Svelte-based website for BurbSec security events and meetups.

## About

BurbSec hosts security meetups and events across different locations. This site provides information about upcoming events, locations, and sponsors.

## Project Structure

This is a SvelteKit application with the following structure:

- **Event Pages**: Individual pages for different BurbSec locations and events
  - Prime (`/prime`)
  - North (`/north`) 
  - South (`/south`)
  - East (`/east`)
  - West (`/west`)
  - Northwest (`/northwest`)
  - Galway (`/galway`)
  - Las Vegas (`/lasvegas`)
  - CigarSec (`/cigarsec`)
- **Sponsors**: Information about event sponsors (`/sponsors`)

## Development

### Prerequisites

- Node.js (version 16 or higher)
- npm

### Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

To build the application for production:

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## Technology Stack

- **Framework**: SvelteKit
- **Build Tool**: Vite
- **Styling**: Custom CSS
- **Deployment**: Static site generation

## Contributing

This site is open source. Feel free to submit issues and pull requests to improve the site.

## License

See [LICENSE](LICENSE) file for details.