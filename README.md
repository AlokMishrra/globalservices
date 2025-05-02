# Global Services Website

A full-stack web application built with React, Vite, Node.js, and PostgreSQL.

## Prerequisites

- Node.js >= 18
- PostgreSQL database (or Neon account)

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
# Database
DATABASE_URL=your_database_url

# Server
PORT=3000
NODE_ENV=development

# Security
JWT_SECRET=your_jwt_secret
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/AlokMishrra/globalservices.git
cd globalservices
```

2. Install dependencies:
```bash
npm install
```

3. Set up your environment variables as described above.

4. Run database migrations:
```bash
npm run db:push
```

## Development

Run the development server:
```bash
npm run dev
```

## Production Build

Build the application:
```bash
npm run build
```

Start the production server:
```bash
npm start
```

## Deployment

This application can be deployed to various platforms:

### Heroku

1. Create a new Heroku app
2. Add PostgreSQL addon
3. Deploy using Git:
```bash
heroku git:remote -a your-app-name
git push heroku main
```

### Netlify

1. Connect your GitHub repository
2. Set build command: `npm run build`
3. Set publish directory: `dist/public`
4. Add environment variables in Netlify dashboard

### Railway/Render

1. Create new project
2. Connect GitHub repository
3. Set build command: `npm run build`
4. Set start command: `npm start`
5. Add environment variables

## Project Structure

```
├── client/               # Frontend React application
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/      # Page components
│   │   └── lib/        # Utilities and helpers
├── server/              # Backend Node.js application
│   ├── api/            # API routes
│   └── db.ts           # Database configuration
├── shared/             # Shared types and utilities
└── dist/              # Production build output
```

## Features

- Modern React with TypeScript
- Server-side rendering capabilities
- Database ORM with Drizzle
- Authentication system
- File upload functionality
- Admin dashboard
- Blog system
- Portfolio management
- Contact form
- Responsive design

## License

MIT
