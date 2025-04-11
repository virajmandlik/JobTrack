# Job Track - Career Compass

A comprehensive MERN stack application for tracking job applications, managing resumes, and monitoring your career progress.

## 🚀 Features

### Job Management
- Add new job applications with detailed information
- Track application status (Applied, Interview, Offer, Rejected)
- Filter and sort applications by status, date, and company
- Update application status and details
- Delete applications

### Company Management
- Add and manage company information
- Search companies
- Track jobs per company
- View company details and statistics

### Resume Management
- Upload and manage multiple resumes
- Set default resume
- Track resume usage in applications

### Statistics & Analytics
- View application trends over time
- Monitor response rates
- Track interview success rates
- Analyze application status distribution

### User Management
- Secure authentication
- User profile management
- Session management

## 🛠️ Tech Stack

### Frontend
- React 18 with TypeScript
- Vite for fast development
- React Router for navigation
- Chart.js for data visualization
- Tailwind CSS for styling
- Shadcn UI components
- React Query for data fetching
- Axios for API calls

### Backend
- Node.js with Express
- MongoDB with Mongoose
- JWT for authentication
- Bcrypt for password hashing
- CORS for cross-origin requests
- Morgan for logging

### Database
- MongoDB Atlas (Cloud-hosted)
- Mongoose ODM

### Deployment
- Frontend: Vercel
- Backend: Render/Railway
- Database: MongoDB Atlas

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account
- Git

### Frontend Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/job-track.git
cd job-track

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Start development server
npm run dev
```

### Backend Setup
```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Start development server
npm run dev
```

## 🔧 Environment Variables

### Frontend (.env)
```env
VITE_API_URL=http://localhost:5000/api
VITE_APP_NAME=Job Track
```

### Backend (.env)
```env
PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
NODE_ENV=development
```

## 📁 Project Structure

```
job-track/
├── src/
│   ├── components/     # Reusable UI components
│   ├── contexts/       # React contexts
│   ├── pages/          # Page components
│   ├── types/          # TypeScript types
│   ├── utils/          # Utility functions
│   └── App.tsx         # Main App component
├── backend/
│   ├── config/         # Configuration files
│   ├── controllers/    # Route controllers
│   ├── middleware/     # Express middleware
│   ├── models/         # Mongoose models
│   ├── routes/         # API routes
│   └── server.js       # Express server
└── README.md
```

## 🔐 Authentication Flow

1. User registers with email and password
2. Backend creates user and returns JWT token
3. Frontend stores token in localStorage
4. Token is sent with each API request
5. Protected routes verify token validity

## 📊 Data Models

### User
```typescript
interface User {
  name: string;
  email: string;
  password: string;
  profilePicture?: string;
}
```

### Job
```typescript
interface Job {
  role: string;
  company: string;
  status: 'Applied' | 'Interview' | 'Offer' | 'Rejected';
  dateApplied: Date;
  link?: string;
  notes?: string;
}
```

### Company
```typescript
interface Company {
  name: string;
  description?: string;
  website?: string;
  industry?: string;
  location?: string;
  size?: string;
}
```

## 🚀 Deployment

### Frontend (Vercel)
1. Push code to GitHub repository
2. Connect repository to Vercel
3. Configure environment variables
4. Deploy

### Backend (Render/Railway)
1. Push code to GitHub repository
2. Connect repository to Render/Railway
3. Configure environment variables
4. Deploy

### Database (MongoDB Atlas)
1. Create new cluster
2. Configure network access
3. Create database user
4. Get connection string

## 📝 API Endpoints

### Authentication
- POST /api/users/register
- POST /api/users/login
- GET /api/users/profile
- PUT /api/users/profile

### Jobs
- GET /api/jobs
- POST /api/jobs
- PUT /api/jobs/:id
- DELETE /api/jobs/:id

### Companies
- GET /api/companies
- POST /api/companies
- GET /api/companies/search
- PUT /api/companies/:id
- DELETE /api/companies/:id

### Statistics
- GET /api/statistics

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [React](https://reactjs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Vercel](https://vercel.com/)
- [Render](https://render.com/)
- [Railway](https://railway.app/)
