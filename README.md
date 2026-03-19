# Reactopedia

A comprehensive, interactive learning platform for React developers. Reactopedia provides an intuitive interface to explore React concepts, tutorials, hooks documentation, and code snippets with live code execution capabilities.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Build & Deployment](#build--deployment)
- [Project Architecture](#project-architecture)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

Reactopedia is a next-generation learning platform designed to help developers master React through interactive tutorials, curated articles, and hands-on code examples. With features like user authentication, personalized learning paths, and a dark/light theme, it provides a modern and accessible learning experience.

**Project ID:** reactopedia-66149  
**Hosted On:** Firebase

## ✨ Features

### Core Learning Features
- **React Concepts Library** - Comprehensive documentation on React fundamentals and advanced concepts
- **Interactive Tutorials** - Step-by-step guides for learning React patterns and best practices
- **React Hooks Documentation** - Detailed reference and examples for all React Hooks
- **Code Snippet Showcase** - Live code examples with syntax highlighting and execution capabilities

### User Experience
- **User Authentication** - Secure Firebase-based authentication system
- **Personalized Dashboard** - User-specific content recommendations and learning progress
- **Dark/Light Theme** - System-aware theme switching for comfortable reading
- **Advanced Search** - Fast, fuzzy search functionality across all articles and concepts
- **Categorized Content** - Browse articles by topics and categories
- **Responsive Design** - Fully responsive UI optimized for desktop, tablet, and mobile devices

### Editor & Execution
- **Monaco Editor Integration** - Professional-grade code editor embedded in the application
- **Live Code Execution** - Run and test React code snippets in real-time
- **Syntax Highlighting** - Beautiful syntax highlighting for multiple programming languages

## 🛠️ Technology Stack

### Frontend Framework & Build Tools
- **React 18.2.0** - Modern UI library with hooks and concurrent rendering
- **Vite 6.3.5** - Next-generation frontend build tool
- **React Router 6.30.1** - Client-side routing and navigation

### Styling & UI Components
- **Tailwind CSS 4.1.7** - Utility-first CSS framework
- **Bootstrap 5.3.6** - Popular CSS framework for responsive design
- **React Bootstrap 2.10.10** - Bootstrap components for React
- **Lucide React 0.511.0** - Beautiful, consistent SVG icons
- **React Icons 4.12.0** - Popular icon library

### Code Editor & Execution
- **Monaco Editor for React 4.7.0** - Professional code editor component
- **React Live 4.1.8** - Live code execution in the browser
- **React Syntax Highlighter 15.6.1** - Syntax highlighting for code blocks

### Backend & Database
- **Firebase 11.8.1** - Backend-as-a-service for authentication and real-time data
- **Firestore** - Cloud-hosted NoSQL database

### Utilities & Enhancement
- **Fuse.js 7.1.0** - Lightweight fuzzy search library
- **use-debounce 10.0.4** - React hook for debouncing values
- **Vercel Analytics 1.5.0** - Performance and analytics monitoring

### Development Tools
- **ESLint** - Code quality and consistency
- **PostCSS 8.5.3** - CSS transformation tool
- **AutoPrefixer 10.4.21** - Automatic vendor prefixes for CSS
- **React Types** - TypeScript definitions for React

## 📁 Project Structure

```
my-react-app/
├── public/                 # Static assets
├── src/
│   ├── components/        # Reusable UI components
│   │   ├── Auth.jsx       # Authentication component
│   │   ├── Navbar.jsx     # Navigation bar
│   │   ├── Search.jsx     # Search functionality
│   │   ├── CodeSnippet.jsx # Code display component
│   │   ├── ConceptCard.jsx # Concept card display
│   │   ├── Footer.jsx     # Footer component
│   │   └── Header.jsx     # Header component
│   ├── context/           # React Context for state management
│   │   ├── ThemeContext.jsx   # Dark/Light theme state
│   │   ├── ArticlesContext.jsx # Articles state
│   │   └── userContext.jsx    # User authentication state
│   ├── pages/            # Page components (routes)
│   │   ├── Home.jsx      # Landing/dashboard page
│   │   ├── ArticlePage.jsx    # Article listing page
│   │   ├── ArticleDetail.jsx  # Individual article view
│   │   ├── CategoryPage.jsx   # Articles by category
│   │   ├── Tutorial.jsx       # Tutorial section
│   │   ├── Hooks.jsx          # React Hooks documentation
│   │   ├── EditPage.jsx       # Article editing page
│   │   └── About.jsx          # About page
│   ├── hooks/            # Custom React hooks
│   │   └── useTheme.js   # Theme management hook
│   ├── Services/         # API and service layer
│   │   └── api.js        # API calls and utilities
│   ├── data/            # Static data and constants
│   │   ├── sampleData.js # Sample article data
│   │   ├── reactConcepts.js # React concept definitions
│   │   └── Docs.json     # Documentation data
│   ├── img/             # Image assets
│   ├── App.jsx          # Root component with routing
│   ├── App.css          # App global styles
│   ├── firebase.js      # Firebase configuration
│   ├── index.css        # Global styles
│   ├── main.jsx         # Application entry point
│   └── reportWebVitals.js # Web Vitals monitoring
├── eslint.config.js     # ESLint configuration
├── vite.config.js       # Vite configuration
├── package.json         # Project dependencies
├── index.html           # HTML template
└── README.md           # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed on your machine:
- **Node.js** (v16 or higher) - [Download](https://nodejs.org/)
- **npm** (v7 or higher) or **yarn** - Comes with Node.js
- **Git** - For version control

### Installation

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd my-react-app
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```
   
   Or using yarn:
   ```bash
   yarn install
   ```

3. **Environment Configuration**
   
   The Firebase configuration is already included in `src/firebase.js`. For production deployment, ensure to update the credentials:
   ```javascript
   const firebaseConfig = {
     apiKey: "YOUR_API_KEY",
     authDomain: "YOUR_AUTH_DOMAIN",
     projectId: "YOUR_PROJECT_ID",
     storageBucket: "YOUR_STORAGE_BUCKET",
     messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
     appId: "YOUR_APP_ID",
     measurementId: "YOUR_MEASUREMENT_ID"
   };
   ```

## 💻 Usage

### Development Server

Start the development server with hot module replacement (HMR):

```bash
npm run dev
```

The application will be available at `http://localhost:5173`

### Building for Production

Create an optimized production build:

```bash
npm run build
```

The production-ready files will be generated in the `dist/` directory.

### Preview Production Build

Test the production build locally:

```bash
npm run preview
```

### Development Commands Reference

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with HMR |
| `npm run build` | Create optimized production build |
| `npm run preview` | Preview production build locally |
| `npm start` | Alias for `npm run dev` |

## 🏗️ Build & Deployment

### Production Build Process

Vite performs the following optimizations during build:

1. **Code Splitting** - Automatic chunk splitting for optimal loading
2. **Tree Shaking** - Removes unused code for smaller bundle sizes
3. **Minification** - Minifies JavaScript and CSS
4. **Asset Optimization** - Compresses images and static assets

### Deployment Recommendations

#### Firebase Hosting
Since the project uses Firebase, deployment to Firebase Hosting is recommended:

```bash
npm install -g firebase-tools
firebase login
firebase init hosting
npm run build
firebase deploy
```

#### Other Platforms
- **Vercel** - Optimized for Vite projects, [Deploy Guide](https://vercel.com/docs/frameworks/vite)
- **Netlify** - Supports Vite builds, [Deploy Guide](https://docs.netlify.com/frameworks/vite/)
- **AWS Amplify** - Full-stack AWS services integration

## 🏛️ Project Architecture

### State Management

The application uses **React Context API** for global state management:

- **ThemeContext** - Manages dark/light theme preference
- **UserContext** - Handles user authentication state and user data
- **ArticlesContext** - Manages articles and content data

### Component Hierarchy

```
App
├── Router
├── Navbar (Navigation)
├── Routes
│   ├── Auth (Login Page)
│   ├── Home (Dashboard)
│   ├── ArticlePage (Articles List)
│   ├── ArticleDetail (Single Article)
│   ├── CategoryPage (Filtered Articles)
│   ├── Tutorial (Tutorials Section)
│   ├── Hooks (Hooks Documentation)
│   ├── EditPage (Article Editor)
│   └── About (About Page)
└── Footer (Footer)
```

### Data Flow

1. **User Authentication** → Firebase Auth
2. **Content Retrieval** → Firestore / Static Data
3. **Theme Preference** → ThemeContext
4. **Search & Filter** → Fuse.js (Client-side)
5. **Code Execution** → Monaco Editor + React Live

## ⚙️ Configuration

### Vite Configuration

Configured in `vite.config.js` with React plugin for Fast Refresh support.

### ESLint Configuration

Code quality rules are defined in `eslint.config.js`.

### Styling

- **Tailwind CSS** - Configure in `tailwind.config.js` (if present)
- **Bootstrap** - Imported in components via react-bootstrap
- **PostCSS** - Configured via `postcss.config.js`

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Code Standards
- Follow ESLint rules
- Use consistent naming conventions
- Write descriptive commit messages
- Test your changes before submitting

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📧 Support

For issues, questions, or suggestions, please open an issue on the repository or contact the development team.

---

**Last Updated:** March 2026  
**Version:** 0.0.0
