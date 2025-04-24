# VibeTravels

## Table of Contents
- Project Description
- Tech Stack
- Getting Started Locally
- Available Scripts
- License

## Project Description

VibeTravels is a web application that uses artificial intelligence to transform simple travel notes into comprehensive travel plans. It's designed for groups of friends (up to 8 adults) who want to efficiently plan engaging trips based on their preferences, budget, and available time.

The application solves common trip planning challenges by:
- Automatically finding attractions that match group preferences
- Arranging attractions in a logical sequence
- Providing practical information about ticket prices, opening hours, and potential discounts
- Estimating total trip costs broken down by elements
- Ensuring quality and appeal of selected locations

VibeTravels streamlines the planning process through AI automation while considering individual preferences, budget constraints, time availability, and other factors affecting trip quality.

## Tech Stack

### Frontend
- **Astro 5**: For creating fast, efficient pages with minimal JavaScript
- **React 19**: For interactive components
- **TypeScript 5**: For static typing and improved IDE support
- **Tailwind 4**: For utility-first CSS styling
- **Shadcn/ui**: For accessible React components

### Backend
- **Supabase**: Comprehensive backend solution providing:
  - PostgreSQL database
  - SDK for Backend-as-a-Service capabilities
  - Built-in user authentication
  - Open-source solution that can be hosted locally or on a server

### AI Integration
- **OpenAI**: For communication with AI models

### CI/CD & Hosting
- **GitHub Actions**: For CI/CD pipelines
- **DigitalOcean**: For hosting the application via Docker image

## Getting Started Locally

### Prerequisites
- Node.js 22.14.0 (use NVM to install the correct version)
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/vibetravels.git
   cd vibetravels
   ```

2. Install the correct Node.js version using NVM:
   ```bash
   nvm use
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory with the necessary environment variables (refer to project documentation for required variables).

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and navigate to `http://localhost:4321`

## Available Scripts

- `npm run dev` - Starts the Astro development server
- `npm run build` - Builds the Astro project for production
- `npm run preview` - Previews the production build locally
- `npm run astro` - Runs Astro CLI commands
- `npm run lint` - Runs ESLint to check for code issues
- `npm run lint:fix` - Runs ESLint and automatically fixes issues where possible
- `npm run format` - Runs Prettier to format code

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

© 2025 VibeTravels. All rights reserved.
