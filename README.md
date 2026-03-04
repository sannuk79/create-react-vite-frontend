# create-clean-react-vite

[![npm version](https://img.shields.io/npm/v/create-clean-react-vite.svg)](https://www.npmjs.com/package/create-clean-react-vite)
[![npm downloads](https://img.shields.io/npm/dm/create-clean-react-vite.svg)](https://www.npmjs.com/package/create-clean-react-vite)
[![license](https://img.shields.io/npm/l/create-clean-react-vite.svg)](https://github.com/sannuk79/create-react-vite-frontend/blob/main/LICENSE)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sannuk79/create-react-vite-frontend/blob/main/LICENSE)

> 🚀 **Ultra-clean React + Vite starter CLI** with Tailwind CSS, TypeScript, ESLint, and built-in payload validation.

---

## 📖 Table of Contents

- [Quick Start](#-quick-start)
- [Features](#-features)
- [What's Included](#-whats-included)
- [Installation](#-installation)
- [Usage](#-usage)
- [Payload Validation](#-payload-validation)
- [Project Structure](#-project-structure)
- [Available Scripts](#-available-scripts)
- [Tech Stack](#-tech-stack)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🚀 Quick Start

Create a new React + Vite project in seconds:

```bash
npx create-clean-react-vite myapp
cd myapp
npm run dev
```

| Command | Description |
|---------|-------------|
| `npx create-clean-react-vite myapp` | ✅ Creates a new clean React + Vite project |
| `npm install create-clean-react-vite` | ❌ Don't install as a dependency |

---

## ✨ Features

- **React 18** - Latest version with hooks
- **Vite 5** - Lightning fast HMR and build
- **Tailwind CSS 3** - Utility-first CSS framework
- **TypeScript 5** - Strict mode enabled for type safety
- **ESLint 8** - Code quality and consistency
- **payload-guard-filter** - Pre-configured API validation
- **Zero Demo Files** - Clean, production-ready structure
- **Minimal Dependencies** - Lightweight (~200MB node_modules)
- **Git Initialized** - Auto-initializes git repository

---

## 📦 What's Included

Your new project will include:

```
myapp/
├── src/
│   ├── main.tsx             # React entry point
│   ├── App.tsx              # Main App component
│   ├── index.css            # Global styles with Tailwind
│   ├── lib/
│   │   └── payloadGuard.ts  # Pre-configured validation shapes
│   ├── components/          # Your custom components
│   └── types/               # TypeScript type definitions
├── .eslintrc.json           # ESLint configuration
├── .gitignore
├── index.html               # HTML entry point
├── package.json
├── postcss.config.mjs       # PostCSS configuration
├── tailwind.config.ts       # Tailwind configuration
├── tsconfig.json            # TypeScript configuration
└── vite.config.ts           # Vite configuration
```

---

## 📥 Installation

### Prerequisites

- **Node.js** 18.17 or later
- **npm** or **yarn** package manager

### Create New Project

```bash
# Using npx (recommended)
npx create-clean-react-vite myapp

# Navigate to project
cd myapp

# Start development server
npm run dev
```

---

## 🔒 Payload Validation

Pre-defined validation shapes in `src/lib/payloadGuard.ts`:

```typescript
import { login, register, payload } from "@/lib/payloadGuard";

// Form validation example
function handleSubmit(formData: any) {
  // Validate login payload - only allowed fields returned
  const safe = login(formData);
  
  // Send safe data to API
  return safe;
}
```

### Available Shapes

| Shape | Fields |
|-------|--------|
| `login` | password, token, api_key |
| `register` | username, email, password |
| `payload` | data, message, value |

---

## 🏗️ Project Structure

### `src/`
Main source directory for your React application.

### `src/components/`
Reusable React components (empty by default).

### `src/lib/`
Utility functions and payload validation guards.

### `src/types/`
TypeScript type definitions and interfaces.

---

## 📖 Available Scripts

```bash
npm run dev      # Start development server at localhost:5173
npm run build    # Build for production
npm run preview  # Preview production build
npm run lint     # Run ESLint checks
```

---

## 🛠️ Tech Stack

| Package | Version | Description |
|---------|---------|-------------|
| **React** | Latest | UI library |
| **React DOM** | Latest | React DOM renderer |
| **Vite** | ^5 | Build tool |
| **TypeScript** | ^5 | Type safety |
| **Tailwind CSS** | ^3 | CSS framework |
| **ESLint** | ^8 | Code linting |
| **payload-guard-filter** | ^1.8.0 | API validation |

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development

```bash
# Clone the repository
git clone https://github.com/sannuk79/create-react-vite-frontend.git

# Navigate to project
cd create-clean-react

# Install dependencies
npm install

# Make your changes and test
```

---

## 📄 License

This project is licensed under the [MIT License](https://github.com/sannuk79/create-react-vite-frontend/blob/main/LICENSE).

---

## 🔗 Links

- **[npm Package](https://www.npmjs.com/package/create-clean-react-vite)**
- **[GitHub Repository](https://github.com/sannuk79/create-react-vite-frontend)**
- **[Report Issues](https://github.com/sannuk79/create-react-vite-frontend/issues)**

---

## 📞 Support

If you have any questions or need help:

- Open an issue on [GitHub](https://github.com/sannuk79/create-react-vite-frontend/issues)
- Check existing documentation

---

<div align="center">

**Made with ❤️ by [sannuk79](https://github.com/sannuk79)**

If you like this project, please ⭐ star the repository!

</div>
