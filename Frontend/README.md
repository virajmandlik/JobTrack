# Job Track Career Compass

A modern web application to help job seekers track their job applications, manage their career progress, and organize their job search process.

## Features

- **User Authentication**: Secure login and registration system
- **Job Application Tracking**: Track all your job applications in one place
- **Application Status Management**: Monitor application status (Applied, Interview, Offer, Rejected)
- **Company Management**: Save and manage information about companies you're interested in
- **Job Search**: Search and save job listings from various sources
- **Statistics Dashboard**: Visualize your job search progress with charts and metrics
- **Resume Management**: Upload and manage multiple versions of your resume
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **Frontend**: React, TypeScript, Vite
- **UI Components**: Custom components with modern design
- **State Management**: React Context API
- **API Communication**: Axios
- **Authentication**: JWT-based authentication
- **Data Visualization**: Charts for statistics and analytics

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/job-track-career-compass.git
cd job-track-career-compass/Frontend
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Create a `.env` file in the root directory with the following variables:
```
VITE_API_URL=https://your-backend-api-url.com
```

4. Start the development server
```bash
npm run dev
# or
yarn dev
```

5. Open your browser and navigate to `http://localhost:5173`

## Project Structure

```
src/
├── api.ts                 # API communication utilities
├── config.ts              # Configuration and environment variables
├── contexts/              # React Context providers
│   ├── AuthContext.tsx    # Authentication state management
│   ├── CompanyContext.tsx # Company data management
│   ├── SavedJobContext.tsx # Saved jobs management
│   └── StatisticsContext.tsx # Statistics and analytics
├── pages/                 # Application pages
│   ├── Dashboard.tsx      # Main dashboard
│   ├── Login.tsx          # Login page
│   ├── Register.tsx       # Registration page
│   └── ...                # Other pages
├── components/            # Reusable UI components
└── types/                 # TypeScript type definitions
```

## Usage

1. **Register/Login**: Create an account or log in to access your dashboard
2. **Add Job Applications**: Track new job applications with details like company, role, and status
3. **Update Application Status**: Change the status of your applications as you progress
4. **View Statistics**: Check your application metrics and progress on the dashboard
5. **Manage Companies**: Add and update information about companies you're interested in
6. **Save Jobs**: Save interesting job listings for later reference

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to all contributors who have helped shape this project
- Inspired by the need for better job application tracking tools 
