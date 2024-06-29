## Description

# EventFlow

EventFlow is a scalable event booking system built with NestJS microservices architecture. This project aims to provide
a comprehensive solution for managing events, bookings, and user interactions efficiently.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
- [Usage](#usage)
- [Microservices](#microservices)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication and authorization
- Event creation and management
- Booking system with real-time updates
- Notification service for booking confirmations and reminders
- Admin dashboard for event organizers
- Scalable microservices architecture

## Technologies Used

- **Frontend:** React, TypeScript, Next.js
- **Backend:** NestJS, TypeORM, PostgreSQL, Docker
- **Microservices:** NestJS Microservices
- **Other:** Redis, RabbitMQ

## Getting Started

### Prerequisites

- Node.js (>=14.x)
- Docker
- PostgreSQL
- Redis
- RabbitMQ

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/EventFlow.git
   cd EventFlow

## Installation

```bash
$ pnpm install
```

## Running the app

```bash
# development
$ pnpm run start

# watch mode
$ pnpm run start:dev

# production mode
$ pnpm run start:prod
```

## Test

```bash
# unit tests
$ pnpm run test

# e2e tests
$ pnpm run test:e2e

# test coverage
$ pnpm run test:cov
```

## Usage

Once the application is up and running, you can access the frontend at http://localhost:3000 and the backend API
at http://localhost:3001.

## Microservices
EventFlow is composed of several microservices, each responsible for a specific domain within the system:

User Service: Manages user registration, authentication, and profiles.
Event Service: Handles event creation, updates, and deletions.
Booking Service: Manages event bookings and related notifications.
Notification Service: Sends email and SMS notifications for bookings and reminders.
Admin Service: Provides tools for event organizers to manage their events and view statistics.
Each microservice communicates through a message broker (RabbitMQ) and uses Redis for caching and session management.
