# Frontend Structure Documentation

## Overview
This document outlines the comprehensive frontend structure for the Library Management System (LMS) built with React.js, Vite, and modern development practices.

## Directory Structure

```
frontend/
├── public/                          # Static assets served directly
│   ├── book.jpg
│   ├── book.png
│   ├── book.svg
│   └── books.svg
├── src/
│   ├── components/                  # Reusable React components
│   │   ├── ui/                     # Basic UI components
│   │   │   ├── Button/
│   │   │   │   ├── Button.jsx
│   │   │   │   ├── Button.css
│   │   │   │   └── index.js
│   │   │   ├── Input/
│   │   │   ├── Modal/
│   │   │   ├── Card/
│   │   │   ├── Table/
│   │   │   ├── Loading/
│   │   │   └── index.js
│   │   ├── forms/                  # Form-specific components
│   │   │   ├── LoginForm/
│   │   │   ├── RegisterForm/
│   │   │   ├── BookForm/
│   │   │   ├── UserForm/
│   │   │   └── index.js
│   │   ├── layout/                 # Layout components
│   │   │   ├── Navbar/
│   │   │   │   ├── Navbar.jsx
│   │   │   │   ├── Navbar.css
│   │   │   │   └── index.js
│   │   │   ├── Sidebar/
│   │   │   ├── Footer/
│   │   │   ├── Header/
│   │   │   └── index.js
│   │   ├── common/                 # Common/shared components
│   │   │   ├── ProtectedRoute/
│   │   │   │   ├── ProtectedRoute.jsx
│   │   │   │   ├── ProtectedRoute.css
│   │   │   │   └── index.js
│   │   │   ├── ErrorBoundary/
│   │   │   ├── LoadingSpinner/
│   │   │   ├── Toast/
│   │   │   └── index.js
│   │   └── index.js                # Component exports
│   ├── pages/                      # Page components
│   │   ├── auth/                   # Authentication pages
│   │   │   ├── Login/
│   │   │   │   ├── Login.jsx
│   │   │   │   ├── Login.css
│   │   │   │   └── index.js
│   │   │   ├── Register/
│   │   │   └── index.js
│   │   ├── admin/                  # Admin-specific pages
│   │   │   ├── Dashboard/
│   │   │   ├── BookManagement/
│   │   │   ├── UserManagement/
│   │   │   ├── Reports/
│   │   │   └── index.js
│   │   ├── member/                 # Member-specific pages
│   │   │   ├── Dashboard/
│   │   │   ├── BookSearch/
│   │   │   ├── MyBorrowings/
│   │   │   ├── Profile/
│   │   │   └── index.js
│   │   ├── shared/                 # Shared pages
│   │   │   ├── Home/
│   │   │   ├── NotFound/
│   │   │   └── index.js
│   │   └── index.js                # Page exports
│   ├── contexts/                   # React Context providers
│   │   ├── AuthContext.jsx
│   │   ├── ThemeContext.jsx
│   │   ├── NotificationContext.jsx
│   │   └── index.js
│   ├── hooks/                      # Custom React hooks
│   │   ├── useAuth.js
│   │   ├── useApi.js
│   │   ├── useLocalStorage.js
│   │   ├── useDebounce.js
│   │   └── index.js
│   ├── services/                   # API and external services
│   │   ├── api/
│   │   │   ├── auth.js
│   │   │   ├── books.js
│   │   │   ├── users.js
│   │   │   ├── borrowings.js
│   │   │   └── index.js
│   │   ├── storage/
│   │   │   ├── localStorage.js
│   │   │   └── sessionStorage.js
│   │   └── index.js
│   ├── utils/                      # Utility functions
│   │   ├── validation.js
│   │   ├── formatting.js
│   │   ├── dateUtils.js
│   │   ├── stringUtils.js
│   │   └── index.js
│   ├── constants/                  # Application constants
│   │   ├── api.js
│   │   ├── routes.js
│   │   ├── roles.js
│   │   ├── messages.js
│   │   └── index.js
│   ├── types/                      # TypeScript type definitions (if using TS)
│   │   ├── auth.js
│   │   ├── book.js
│   │   ├── user.js
│   │   └── index.js
│   ├── assets/                     # Static assets
│   │   ├── images/
│   │   │   ├── logos/
│   │   │   ├── backgrounds/
│   │   │   └── illustrations/
│   │   ├── icons/
│   │   │   ├── svg/
│   │   │   └── png/
│   │   └── styles/
│   │       ├── globals.css
│   │       ├── variables.css
│   │       ├── components.css
│   │       └── themes/
│   ├── config/                     # Configuration files
│   │   ├── api.js
│   │   ├── routes.js
│   │   ├── theme.js
│   │   └── index.js
│   ├── App.jsx                     # Main App component
│   ├── main.jsx                    # Application entry point
│   └── style.css                   # Global styles
├── package.json
├── vite.config.js
├── .env.example
├── .gitignore
└── README.md
```

## Component Organization

### 1. UI Components (`components/ui/`)
Basic, reusable UI elements that don't contain business logic:
- **Button**: Primary, secondary, danger, success variants
- **Input**: Text, email, password, number, textarea
- **Modal**: Confirmation, information, form modals
- **Card**: Content cards with headers, bodies, footers
- **Table**: Data tables with sorting, pagination
- **Loading**: Spinners, skeletons, progress bars

### 2. Form Components (`components/forms/`)
Form-specific components with validation and business logic:
- **LoginForm**: User authentication form
- **RegisterForm**: User registration form
- **BookForm**: Add/edit book form
- **UserForm**: Add/edit user form
- **SearchForm**: Book search form

### 3. Layout Components (`components/layout/`)
Components that define the overall page structure:
- **Navbar**: Navigation bar with user menu
- **Sidebar**: Admin/member sidebar navigation
- **Footer**: Site footer
- **Header**: Page headers with breadcrumbs

### 4. Common Components (`components/common/`)
Shared components used across the application:
- **ProtectedRoute**: Route protection wrapper
- **ErrorBoundary**: Error handling wrapper
- **LoadingSpinner**: Global loading indicator
- **Toast**: Notification system

## Page Organization

### 1. Authentication Pages (`pages/auth/`)
- **Login**: User login page
- **Register**: User registration page

### 2. Admin Pages (`pages/admin/`)
- **Dashboard**: Admin overview and statistics
- **BookManagement**: Add, edit, delete books
- **UserManagement**: Manage library members
- **Reports**: System reports and analytics

### 3. Member Pages (`pages/member/`)
- **Dashboard**: Member overview and quick actions
- **BookSearch**: Search and browse books
- **MyBorrowings**: View current and past borrowings
- **Profile**: User profile management

### 4. Shared Pages (`pages/shared/`)
- **Home**: Landing page
- **NotFound**: 404 error page

## Services Layer

### API Services (`services/api/`)
- **auth.js**: Authentication API calls
- **books.js**: Book-related API calls
- **users.js**: User management API calls
- **borrowings.js**: Borrowing system API calls

### Storage Services (`services/storage/`)
- **localStorage.js**: Local storage utilities
- **sessionStorage.js**: Session storage utilities

## Custom Hooks (`hooks/`)

- **useAuth**: Authentication state management
- **useApi**: API call management with loading/error states
- **useLocalStorage**: Local storage state management
- **useDebounce**: Debounced value for search inputs

## Utilities (`utils/`)

- **validation.js**: Form validation functions
- **formatting.js**: Data formatting utilities
- **dateUtils.js**: Date manipulation functions
- **stringUtils.js**: String manipulation utilities

## Constants (`constants/`)

- **api.js**: API endpoints and configuration
- **routes.js**: Application routes
- **roles.js**: User roles and permissions
- **messages.js**: Success/error messages

## Assets Organization

### Images (`assets/images/`)
- **logos/**: Application logos and branding
- **backgrounds/**: Background images
- **illustrations/**: UI illustrations

### Icons (`assets/icons/`)
- **svg/**: SVG icons for better scalability
- **png/**: PNG icons when needed

### Styles (`assets/styles/`)
- **globals.css**: Global CSS variables and resets
- **variables.css**: CSS custom properties
- **components.css**: Component-specific styles
- **themes/**: Theme variations (light/dark)

## Configuration (`config/`)

- **api.js**: API base URL and configuration
- **routes.js**: Route definitions and navigation
- **theme.js**: Theme configuration
- **index.js**: Configuration exports

## Best Practices

### 1. Component Structure
Each component should have its own directory with:
- Component file (`.jsx`)
- Styles file (`.css`)
- Index file for clean imports
- Tests (when applicable)

### 2. Import/Export Strategy
- Use index files for clean imports
- Prefer named exports over default exports
- Group imports: React, third-party, local

### 3. File Naming
- Use PascalCase for components
- Use camelCase for utilities and hooks
- Use kebab-case for CSS files

### 4. State Management
- Use React Context for global state
- Use local state for component-specific data
- Use custom hooks for shared logic

### 5. Styling
- Use CSS modules or styled-components
- Follow BEM methodology for CSS classes
- Use CSS custom properties for theming

## Migration Guide

To migrate from the current structure to this new structure:

1. **Move existing components** to appropriate directories
2. **Update import paths** in all files
3. **Create index files** for clean exports
4. **Reorganize styles** into the assets/styles directory
5. **Update configuration** files
6. **Test all functionality** after migration

## Development Workflow

1. **Create new components** in appropriate directories
2. **Follow naming conventions** consistently
3. **Use TypeScript** for better type safety (optional)
4. **Write tests** for critical components
5. **Document components** with JSDoc comments
6. **Use ESLint and Prettier** for code quality

This structure provides a scalable, maintainable foundation for the LMS frontend application.
