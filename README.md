# Communication Tracking System

A comprehensive solution for managing company communications and tracking engagement. The React-based Calendar Application is designed to help organizations maintain strong professional relationships by tracking interactions, scheduling follow-ups, and managing engagement frequency. It serves as a centralized platform for logging past communications and planning future ones, ensuring timely and consistent follow-ups.

## Features

- **Company Management**: Create, update, and delete company profiles with detailed information
- **Communication Tracking**: Log and track various communication methods (Email, LinkedIn, Phone)
- **Dashboards**:
  - Admin Dashboard: Manage companies and communication methods
  - User Dashboard: Track communications and view calendar
  - Reporting Dashboard: Analyze communication trends and effectiveness
- **Calendar Integration**: Schedule and view upcoming communications
- **Analytics**: Visualize communication patterns and engagement metrics
- **Theme Support**: colour background theme 

## Setup Instructions

### Prerequisites

- Node.js (v16 or higher)
- Yarn package manager

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/communication-tracker.git
   ```
2. Navigate to the project directory:
   ```bash
   cd communication-tracker
   ```
3. Install dependencies:
   ```bash
   yarn install
   ```

### Running the Application

1. Start the development server:
   ```bash
   yarn start
   ```
2. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

### Building for Production

1. Create a production build:
   ```bash
   yarn build
   ```
2. Serve the build files using a static server:
   ```bash
   serve -s build
   ```

### Deploying to Netlify

1. Install the Netlify CLI (if not already installed):
   ```bash
   npm install -g netlify-cli
   ```
2. Login to your Netlify account:
   ```bash
   netlify login
   ```
3. Initialize a new site:
   ```bash
   netlify init
   ```
4. Build the project:
   ```bash
   yarn build
   ```
5. Deploy to Netlify:
   ```bash
   netlify deploy --prod
   ```
6. Follow the prompts to complete the deployment

Alternatively, you can connect your GitHub repository to Netlify for continuous deployment:
1. Push your code to a GitHub repository
2. Go to the Netlify dashboard and select "New site from Git"
3. Choose your repository and configure the build settings:
   - Build command: `yarn build`
   - Publish directory: `build`
4. Click "Deploy site"

## Project Structure

```
src/
├── App.js                # Main application component
├── index.js              # Application entry point
├── theme.js              # Theme configuration
├── context/              # Context providers
│   └── ThemeContext.js   # Theme management context
├── modules/              # Application modules
│   ├── admin/            # Admin-specific components
│   │   ├── AdminDashboard.js
│   │   ├── CompanyManagement.js
│   │   └── CommunicationMethodManagement.js
│   ├── user/             # User-specific components
│   │   ├── UserDashboard.js
│   │   └── EnhancedCalendar.js
│   └── reporting/        # Reporting components
│       └── ReportingDashboard.js
public/                   # Static assets
```

## Known Limitations

1. **Data Persistence**: Currently uses in-memory state management. Data is lost on page refresh.
2. **Authentication**: No user authentication implemented.
3. **Form Validation**: Limited validation in company management forms.

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeatureName`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeatureName`)
5. Create a new Pull Request

## License

MIT License

Copyright (c) 2024 Your Name

Permission is hereby granted...
