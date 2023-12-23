# Vite React App with Auth0 Authentication

This project is a simple user login application built using Vite, React, TypeScript, and integrated with Auth0 for secure user authentication.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Features

- **User Authentication:** Allows users to securely sign up, log in, and log out using Auth0 authentication.
- **Protected Routes:** Implements protected routes that can only be accessed by authenticated users.
- **Type Safety:** Written in TypeScript, providing type safety throughout the application.

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (at least v14.x.x)
- npm or Yarn
- Auth0 account for authentication setup

## Installation

1. Clone the repository: 
   ```bash
   git clone <repository-url>
   ```

2. Install dependencies:
   ```bash
   cd your-project-folder
   npm install   # or yarn install
   ```

## Configuration

### Auth0 Setup

To use Auth0 for authentication, follow these steps:

1. **Create an Auth0 Account:**
   Sign up or log in to your Auth0 account: [Auth0 Dashboard](https://manage.auth0.com/).

2. **Create a New Application:**
   - Go to the Applications section and create a new application.
   - Choose `Single Page Web Applications` as the application type.
   - Set the allowed callback URLs and logout URLs for your application (e.g., `http://localhost:3000/callback`).

3. **Get Auth0 Credentials:**
   - Collect the `Domain` and `Client ID` from the created Auth0 application.
   - Update the configuration in the project to include these credentials.

4. **Environment Variables:**
   Store your Auth0 credentials as environment variables or in a configuration file (e.g., `.env` or `.env.local`). Never expose your credentials in the codebase.

## Usage

After setting up the project and configuring Auth0:

1. Run the development server:
   ```bash
   npm run dev   # or yarn dev
   ```

2. Access the application in your browser at `http://localhost:3000`.

## Folder Structure

```
your-project-folder/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── AuthButton.tsx
│   │   └── ...
│   ├── pages/
│   │   ├── Home.tsx
│   │   ├── Profile.tsx
│   │   └── ...
│   ├── App.tsx
│   └── index.tsx
├── .gitignore
├── package.json
├── README.md
└── ...
```

## Dependencies

- **React:** JavaScript library for building user interfaces
- **Vite:** Next-generation frontend tooling
- **Auth0:** Secure authentication and authorization platform
- **TypeScript:** Typed JavaScript at any scale
