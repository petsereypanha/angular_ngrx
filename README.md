# Angular NgRx Fundamentals

A product management application built with Angular 16 and NgRx for state management. This project demonstrates the fundamentals of using NgRx Store for managing application state in an Angular application.

## Features

- 📦 Product listing and management
- 🔄 State management with NgRx Store
- 🛠️ NgRx DevTools integration
- 🎨 Component-based architecture
- 📝 In-memory data service for development

## Project Structure

```
src/
├── app/
│   ├── products/           # Products feature module
│   │   ├── state/         # NgRx state management
│   │   ├── product-edit/  # Edit product component
│   │   ├── product-page/  # Single product view
│   │   ├── products-list/ # Products list component
│   │   └── products-page/ # Products page container
│   ├── home/              # Home component
│   ├── utils/             # Utility functions
│   └── environments/      # Environment configurations
```

## Prerequisites

- Node.js (v16 or higher recommended)
- pnpm (or npm/yarn)
- Angular CLI v16

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd ngrx
```

2. Install dependencies:
```bash
pnpm install
```

## Development Server

Run the development server:

```bash
pnpm start
```

Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## NgRx Store

This application uses NgRx Store for state management. The current implementation includes:

- **Products State**: Manages product-related state including the `showProductCode` toggle
- **Store DevTools**: Integrated for debugging and time-travel debugging

### State Structure

```typescript
{
  products: {
    showProductCode: boolean
  }
}
```

## Build

Build the project:

```bash
pnpm run build
```

The build artifacts will be stored in the `dist/` directory.

## Technologies Used

- **Angular 16** - Frontend framework
- **NgRx Store 16** - State management
- **RxJS 7** - Reactive programming
- **TypeScript 4.9** - Programming language
- **Angular In-Memory Web API** - Mock backend for development

## Available Scripts

- `pnpm start` - Start development server
- `pnpm run build` - Build the application
- `pnpm run watch` - Build in watch mode

## Development Notes

- The application uses an in-memory data service for API simulation during development
- NgRx DevTools are enabled for state debugging (install the Redux DevTools browser extension)
- Product code visibility can be toggled using the NgRx store

## Learn More

- [Angular Documentation](https://angular.io/docs)
- [NgRx Documentation](https://ngrx.io/docs)
- [RxJS Documentation](https://rxjs.dev/)

## License

This project is for educational purposes.
