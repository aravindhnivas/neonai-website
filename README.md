# NeonAI Website

A modern, responsive website for NeonAI built with SvelteKit, TypeScript, and TailwindCSS.

## Features

- Modern, responsive design
- TypeScript support
- TailwindCSS for styling
- Contact form with validation
- Project showcase
- Team section
- About page with company mission and goals

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm (v7 or higher)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/neonai-website.git
cd neonai-website
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open [http://localhost:5173](http://localhost:5173) in your browser.

## Project Structure

```
src/
├── routes/           # SvelteKit routes
│   ├── +layout.svelte
│   ├── +page.svelte
│   ├── about/
│   ├── projects/
│   └── contact/
├── app.css          # Global styles
└── app.d.ts         # TypeScript declarations
```

## Development

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run check` - Check types and lint code

## Deployment

The website is configured to deploy on Vercel. Simply push to the main branch to trigger a deployment.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

NeonAI - <contact@neonai.com>
