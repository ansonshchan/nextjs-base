# Next.js Base Project

A modern, production-ready Next.js application with TypeScript, Tailwind CSS, and comprehensive development tooling.

## 🚀 Tech Stack

### Core Framework

- **[Next.js 15.5.0](https://nextjs.org)** - React framework with App Router
- **[React 19.1.1](https://react.dev)** - Latest React with concurrent features
- **[TypeScript 5.9.2](https://www.typescriptlang.org)** - Type-safe JavaScript

### Styling & UI

- **[Tailwind CSS 4.1.12](https://tailwindcss.com)** - Utility-first CSS framework
- **[Geist Font](https://vercel.com/font)** - Modern font family optimized for UI
- **PostCSS** - CSS processing with Tailwind integration

### Development Tools

- **[ESLint 9.33.0](https://eslint.org)** - Code linting with Next.js and accessibility rules
- **[Prettier 3.6.2](https://prettier.io)** - Code formatting with Tailwind plugin
- **[Husky 9.1.7](https://typicode.github.io/husky)** - Git hooks for quality gates
- **[lint-staged 16.1.5](https://github.com/okonet/lint-staged)** - Run linters on staged files

## 📁 Project Structure

```
nextjs-base/
├── src/
│   └── app/                 # App Router directory
│       ├── layout.tsx       # Root layout component
│       ├── page.tsx         # Home page component
│       ├── globals.css      # Global styles with Tailwind
│       └── favicon.ico      # App favicon
├── public/                  # Static assets
├── .husky/                  # Git hooks configuration
├── eslint.config.mjs        # ESLint configuration
├── next.config.ts           # Next.js configuration
├── postcss.config.mjs       # PostCSS configuration
├── tailwind.config.ts       # Tailwind CSS configuration
├── tsconfig.json           # TypeScript configuration
└── package.json            # Dependencies and scripts
```

## 🛠️ Configuration Details

### TypeScript Configuration

- **Target**: ES2017 for broad compatibility
- **Module Resolution**: Bundler mode for optimal performance
- **Path Mapping**: `@/*` aliases to `./src/*`
- **Strict Mode**: Enabled for type safety

### ESLint Setup

- **Next.js Core Web Vitals**: Performance and accessibility rules
- **TypeScript Integration**: Type-aware linting
- **Prettier Integration**: Automatic code formatting
- **Accessibility**: JSX-A11Y plugin for inclusive development
- **Custom Rules**: Optimized for React 19 (no React import required)

### Prettier Configuration

- **Single Quotes**: Consistent string formatting
- **Trailing Commas**: All for cleaner diffs
- **Tab Width**: 2 spaces for readability
- **Tailwind Plugin**: Automatic class sorting

### Git Hooks (Husky)

- **Pre-commit**: Runs lint-staged to ensure code quality
- **Lint-staged**: Automatically fixes and formats staged files
  - JavaScript/TypeScript: ESLint fix + Prettier format
  - JSON/CSS/Markdown: Prettier format

### Build Optimization

- **Turbopack**: Enabled for faster development and builds
- **Font Optimization**: Automatic Geist font loading
- **Image Optimization**: Built-in Next.js image optimization

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm (recommended) or npm/yarn

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd nextjs-base

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

### Available Scripts

```bash
pnpm dev          # Start development server with Turbopack
pnpm build        # Build for production with Turbopack
pnpm start        # Start production server
pnpm lint         # Run ESLint
```

### Development Workflow

1. **Code**: Edit files in `src/app/`
2. **Auto-format**: Prettier runs on save (if configured in editor)
3. **Commit**: Husky automatically lints and formats staged files
4. **Build**: Turbopack provides fast builds and hot reloading

## 🎨 Styling System

### Tailwind CSS 4.x

- **CSS Variables**: Custom properties for theming
- **Dark Mode**: Automatic system preference detection
- **Custom Theme**: Extended with project-specific design tokens

### Design Tokens

```css
:root {
  --background: #ffffff;
  --foreground: #171717;
  --font-sans: var(--font-geist-sans);
  --font-mono: var(--font-geist-mono);
}
```

## 📦 Key Dependencies

### Production Dependencies

- `next`: React framework with App Router
- `react` & `react-dom`: React library and DOM renderer

### Development Dependencies

- `@types/*`: TypeScript definitions
- `eslint-*`: Linting ecosystem
- `prettier-*`: Code formatting tools
- `tailwindcss`: Utility-first CSS framework
- `husky` & `lint-staged`: Git workflow automation

## 🚀 Deployment

### Vercel (Recommended)

```bash
# Deploy to Vercel
vercel

# Or connect your Git repository for automatic deployments
```

### Other Platforms

This project can be deployed to any platform that supports Node.js:

- Netlify
- Railway
- DigitalOcean App Platform
- AWS Amplify

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs) - Learn about Next.js features and API
- [Tailwind CSS Docs](https://tailwindcss.com/docs) - Utility-first CSS framework
- [TypeScript Handbook](https://www.typescriptlang.org/docs) - TypeScript language reference

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run `pnpm lint` to check code quality
5. Commit your changes (Husky will run pre-commit hooks)
6. Push to your branch
7. Create a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
