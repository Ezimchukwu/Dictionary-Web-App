# Dictionary Web App

## Overview

This is a modern dictionary web application built with React and TypeScript that allows users to search for word definitions, pronunciations, and examples. The application features a clean, responsive design with search functionality, loading states, error handling, and a "Word of the Day" feature. It integrates with the Dictionary API to fetch comprehensive word data including phonetics, meanings, synonyms, and audio pronunciations.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern development
- **Build Tool**: Vite for fast development and optimized production builds
- **UI Framework**: shadcn/ui components built on Radix UI primitives for accessibility
- **Styling**: Tailwind CSS with CSS variables for consistent theming and responsive design
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod validation for type-safe forms

### Backend Architecture
- **Runtime**: Node.js with Express.js server framework
- **Language**: TypeScript with ES modules for modern JavaScript features
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **Session Management**: connect-pg-simple for PostgreSQL-backed session storage
- **Development**: Hot module replacement via Vite integration in development mode

### Data Storage Solutions
- **Primary Database**: PostgreSQL via Neon Database for production scalability
- **ORM**: Drizzle ORM with type-safe schema definitions and migrations
- **Schema Validation**: Zod for runtime type validation and schema generation
- **Session Storage**: PostgreSQL-based session storage for user authentication
- **Fallback Storage**: In-memory storage implementation for development/testing

### Authentication and Authorization
- **Session-based Authentication**: Uses PostgreSQL-backed sessions via connect-pg-simple
- **User Management**: Basic user model with username/password authentication
- **Type Safety**: Shared TypeScript schemas between client and server for user types

## External Dependencies

### Third-party APIs
- **Dictionary API**: Free Dictionary API (api.dictionaryapi.dev) for word definitions, pronunciations, and examples
- **Audio Playback**: Browser Web Audio API for pronunciation audio playback

### Key External Libraries
- **UI Components**: Radix UI primitives for accessible, unstyled components
- **Styling**: Tailwind CSS for utility-first styling with custom design tokens
- **Data Fetching**: TanStack Query for robust API state management with caching and error handling
- **Form Management**: React Hook Form with Hookform Resolvers for Zod integration
- **Database**: Neon Database serverless PostgreSQL with Drizzle ORM
- **Icons**: Lucide React for consistent icon system
- **Date Handling**: date-fns for date manipulation and formatting
- **Development Tools**: Replit-specific plugins for development environment integration

### Database Configuration
- **Connection**: PostgreSQL via DATABASE_URL environment variable
- **Migrations**: Drizzle Kit for database schema migrations and management
- **Type Generation**: Automatic TypeScript type generation from database schema

### Development Environment
- **Replit Integration**: Custom Vite plugins for Replit-specific development features
- **Error Handling**: Runtime error overlay for better development experience
- **Hot Reload**: Vite HMR integration with Express server for seamless development