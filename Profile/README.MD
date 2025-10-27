# Eventify Project Structure

Complete overview of the project structure.

## Directory Tree

```
Evenitfy/
├── Backend/                          # Node.js/Express Backend API
│   ├── src/
│   │   ├── config/                  # Configuration files
│   │   │   ├── database.js          # MongoDB connection
│   │   │   └── README.md
│   │   ├── controllers/             # Request handlers
│   │   │   ├── authController.js    # Authentication logic
│   │   │   ├── eventController.js   # Event management logic
│   │   │   └── README.md
│   │   ├── middleware/              # Custom middleware
│   │   │   ├── auth.js              # JWT authentication
│   │   │   ├── asyncHandler.js      # Async error handler
│   │   │   ├── errorHandler.js      # Global error handler
│   │   │   └── README.md
│   │   ├── models/                  # Mongoose models
│   │   │   ├── User.js              # User model
│   │   │   ├── Event.js             # Event model
│   │   │   ├── Ticket.js            # Ticket model
│   │   │   ├── Payment.js           # Payment model
│   │   │   └── README.md
│   │   ├── routes/                   # API routes
│   │   │   ├── auth.js              # Auth routes
│   │   │   ├── events.js            # Event routes
│   │   │   ├── user.js              # User routes
│   │   │   ├── tickets.js           # Ticket routes
│   │   │   ├── payments.js          # Payment routes
│   │   │   ├── analytics.js         # Analytics routes
│   │   │   └── README.md
│   │   ├── utils/                    # Utility functions
│   │   │   ├── upload.js            # File upload config
│   │   │   ├── email.js              # Email utility
│   │   │   └── README.md
│   │   └── server.js                 # Application entry point
│   ├── .env.example                  # Environment variables template
│   ├── .gitignore                    # Git ignore rules
│   ├── package.json                  # Dependencies and scripts
│   ├── README.md                     # Backend documentation
│   └── LICENSE
│
├── Frontend/                          # Next.js Frontend Application
│   ├── src/
│   │   ├── app/                      # Next.js app directory
│   │   │   ├── page.tsx             # Homepage
│   │   │   ├── dashboard/page.tsx   # Dashboard
│   │   │   ├── events/page.tsx      # Events page
│   │   │   ├── admin/page.tsx       # Admin page
│   │   │   ├── login/               # Login routes
│   │   │   ├── signup/              # Signup routes
│   │   │   ├── onboarding/page.tsx  # Onboarding
│   │   │   ├── forgot-password/     # Password reset
│   │   │   └── test-flow/           # Testing flows
│   │   ├── components/              # React components
│   │   │   ├── auth/                # Authentication components
│   │   │   ├── dashboard/           # Dashboard components
│   │   │   ├── events/              # Event components
│   │   │   ├── layout/              # Layout components
│   │   │   ├── sections/            # Page sections
│   │   │   ├── ui/                  # UI components
│   │   │   └── ...
│   │   ├── contexts/                # React contexts
│   │   │   ├── AuthContext.tsx      # Auth state
│   │   │   └── UserContext.tsx      # User state
│   │   ├── data/                     # Mock data
│   │   ├── hooks/                    # Custom hooks
│   │   ├── lib/                      # Utilities
│   │   └── types/                    # TypeScript types
│   ├── public/                       # Static assets
│   ├── package.json
│   ├── next.config.js
│   ├── tailwind.config.js
│   ├── tsconfig.json
│   └── README.md
│
├── Final-presentation/               # Project presentations
├── images/                           # Assets
├── SETUP.md                          # Setup instructions
├── PROJECT_STRUCTURE.md             # This file
└── README.md                         # Main project README
```

## Backend Features

### Authentication & Authorization
- JWT-based authentication
- Role-based access control (Attendee, Organizer, Admin)
- Password hashing with bcrypt
- Protected routes middleware

### Models
- **User**: User accounts and profiles
- **Event**: Event details, dates, location, pricing
- **Ticket**: Ticket bookings and management
- **Payment**: Payment processing and tracking

### API Endpoints
- `/api/auth` - Authentication
- `/api/events` - Event management
- `/api/users` - User profiles
- `/api/tickets` - Ticket operations
- `/api/payments` - Payment processing
- `/api/analytics` - Analytics and reports

### Middleware
- Authentication middleware
- Error handling
- Async wrapper for async/await

### Utilities
- File upload (Multer)
- Email sending (Nodemailer)
- Image processing ready

## Frontend Features

### Pages
- Homepage with hero, features, pricing
- User authentication (login/signup)
- Dashboard (attendee/organizer views)
- Event management
- Admin panel

### Components
- Reusable UI components
- Form components
- Dashboard widgets
- Authentication modals
- Event cards and listings

### State Management
- Context API for global state
- Auth context for authentication
- User context for user data

## Technology Stack

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT
- Bcrypt
- Stripe (ready)
- Cloudinary (ready)

### Frontend
- Next.js 13+ (App Router)
- React
- TypeScript
- Tailwind CSS
- Framer Motion

## Getting Started

See `SETUP.md` for detailed setup instructions.

## Development

### Start Backend
```bash
cd Backend && npm run dev
```

### Start Frontend
```bash
cd Frontend && npm run dev
```

## Project Status

✅ Basic structure created
✅ Backend API foundation
✅ Frontend Next.js app
🔄 In development

