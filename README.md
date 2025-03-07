# Blog Platform

A full-stack blog platform with user management and API integration built with React and Express.

## Features

- 🔐 User Authentication (Login/Register)
- 👤 Role-based Authorization (Admin & User roles)
- 📝 Blog Post Management (Create, Read, Delete)
- 💬 Comment System with AJAX
- 🌓 Dark Mode Support
- 🔍 External User Search Integration
- 📱 Responsive Design

## Tech Stack

- Frontend:
  - React with TypeScript
  - TanStack Query for data fetching
  - Tailwind CSS & shadcn/ui for styling
  - Wouter for routing
  - React Hook Form for form management
  - Zod for validation

- Backend:
  - Express.js
  - Passport.js for authentication
  - In-memory storage with TypeScript interfaces
  - Express Session for session management

## Getting Started

### Prerequisites

- Node.js 20.x or later
- npm 8.x or later

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/blog-platform.git
cd blog-platform
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## Usage

1. Register a new account at `/auth`
2. Create blog posts with title, content, and image URL
3. Comment on posts
4. Admin users can access the admin dashboard at `/admin` to manage users

## Development Notes

- The application uses in-memory storage by default
- Session data is stored in memory using memorystore
- External user data is fetched from JSONPlaceholder API

## API Routes

- Authentication:
  - POST `/api/register` - Register new user
  - POST `/api/login` - Login user
  - POST `/api/logout` - Logout user
  - GET `/api/user` - Get current user

- Blog Posts:
  - GET `/api/posts` - Get all posts
  - POST `/api/posts` - Create new post
  - DELETE `/api/posts/:id` - Delete post

- Comments:
  - GET `/api/posts/:id/comments` - Get post comments
  - POST `/api/posts/:id/comments` - Add comment

- Admin:
  - GET `/api/users` - Get all users (admin only)
  - DELETE `/api/users/:id` - Delete user (admin only)

- External:
  - GET `/api/external/users` - Fetch external users

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

MIT License
