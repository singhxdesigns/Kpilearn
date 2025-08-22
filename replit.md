# Overview

This is a comprehensive KPI Flashcards application built for Product Managers and Designers to master business metrics and key performance indicators. The app provides an interactive flashcard system with 45 carefully curated KPIs across different difficulty levels, search functionality, bookmarking, and progress tracking. Users can practice daily with random flashcards or explore specific difficulty levels to learn essential metrics for product management, UX design, marketing, analytics, and business strategy.

## Recent Changes

**August 2025 - Major KPI Expansion:**
- Expanded from 15 to 45 KPIs covering comprehensive product and design metrics
- Added specialized categories: UX/Design metrics, E-commerce KPIs, Advanced Analytics
- Included essential concepts: System Usability Scale, T2D3 framework, Rule of 40, Magic Number
- Enhanced coverage for modern product roles with practical, real-world metrics
- Fixed critical application errors and improved stability

**August 2025 - KPI Library Addition:**
- Added comprehensive KPI Library page for browsing all metrics
- Implemented advanced filtering by difficulty, category, and search
- Created expandable card layout with detailed explanations
- Added quick stats showing distribution across difficulty levels
- Maintains existing gamification while providing reference functionality

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **React + TypeScript**: Built with React 18 and TypeScript for type safety and modern development practices
- **Vite**: Used as the build tool and development server for fast hot module replacement
- **Routing**: Wouter for lightweight client-side routing with support for nested routes
- **UI Framework**: Radix UI components with shadcn/ui styling system providing accessible, customizable components
- **Styling**: Tailwind CSS with CSS variables for theming, custom animations, and responsive design
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Local Storage**: Custom hooks for persisting user preferences, bookmarks, and progress data

## Backend Architecture
- **Express.js**: RESTful API server with middleware for request logging and error handling
- **TypeScript**: Consistent typing across frontend and backend with shared schema definitions
- **In-Memory Storage**: MemStorage class implementing storage interface for KPIs, user progress, and study sessions
- **Development Server**: Custom Vite integration for development with HMR support
- **API Structure**: Clean REST endpoints for KPIs by difficulty, search functionality, and user progress tracking

## Data Storage Solutions
- **Database ORM**: Drizzle ORM configured for PostgreSQL with schema definitions in TypeScript
- **Schema Design**: Structured tables for KPIs, user progress, and study sessions with proper relationships
- **Local Persistence**: Browser localStorage for user data, bookmarks, and session state
- **Development Mode**: In-memory storage implementation for development and testing

## Authentication and Authorization
- **User Identification**: UUID-based user identification stored in localStorage
- **Session Management**: Stateless approach with client-side user tracking
- **No Authentication**: Simplified user experience without login requirements for MVP

## External Dependencies
- **Neon Database**: Serverless PostgreSQL database for production data storage
- **Radix UI**: Comprehensive component library for accessible UI primitives
- **TanStack Query**: Data fetching and caching library for optimal user experience
- **Font Awesome**: Icon library for visual enhancements and user interface elements
- **Google Fonts**: Typography with multiple font families (DM Sans, Geist Mono, Architects Daughter)