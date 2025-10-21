# Overview

Pipo is a mobile-first productivity companion application built with React and Express. The app features a penguin mascot named Pipo who helps users manage their daily tasks, reminders, calendar events, and journal entries through an interactive chat interface. The application supports both text and voice interactions, provides streak tracking for journaling habits, and offers a comprehensive suite of productivity tools in a friendly, engaging mobile interface.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript and Vite for development
- **UI Components**: Shadcn/UI component library with Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Mobile-First Design**: Responsive design optimized for mobile devices with bottom navigation

## Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Language**: TypeScript with ES modules
- **API Pattern**: RESTful API with JSON responses
- **Development Setup**: Hot module replacement with Vite integration for development
- **Error Handling**: Centralized error handling middleware with structured JSON responses

## Data Storage
- **ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL (configured for Neon Database)
- **Schema**: Shared schema definitions between client and server using Drizzle Zod
- **Migration System**: Drizzle Kit for database schema migrations
- **Development Storage**: In-memory storage implementation for development/testing

## Authentication & Session Management
- **Session Storage**: PostgreSQL session store using connect-pg-simple
- **User Management**: Simple user system with streak tracking for engagement
- **Demo Mode**: Default user system for demonstration purposes

## Key Features Architecture
- **Chat System**: Real-time messaging with Pipo mascot, supporting both text and voice input
- **Voice Recognition**: Browser-based speech recognition with fallback text input
- **Productivity Tools**: Integrated reminders, todos, calendar events, and journal entries
- **Streak System**: Gamification through daily journaling streak tracking
- **Mobile Navigation**: Tab-based bottom navigation with badge notifications

## External Dependencies

- **Database**: Neon Database (PostgreSQL-compatible serverless database)
- **UI Components**: Radix UI primitives for accessible component foundations
- **Icons**: Lucide React for consistent iconography
- **Date Handling**: date-fns for date manipulation and formatting
- **Voice Input**: Browser Web Speech API for voice recognition functionality
- **Development Tools**: Replit-specific plugins for development environment integration