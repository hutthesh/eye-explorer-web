# Embiggen Your Eyes Explorer

A production-ready, AI-integrated web application for exploring NASA's gigapixel universe with dual user roles and comprehensive features.

## Features

### Landing Page
- Animated starfield background with parallax effects
- Futuristic design with glowing typography
- Dual login paths for Normal Users and NASA Scientists

### Authentication System
- Secure email/password authentication
- Two-Factor Authentication (2FA) for NASA Scientists
- Remember Me functionality
- Password reset capability
- Demo accounts for quick testing
- Protected routes with role-based access control

### Normal User Features
1. **Dashboard** - Overview of exploration statistics and recent activity
2. **Weather & Space Conditions** - Live atmospheric and space weather data
3. **Gigapixel Image Explorer** - Deep zoom viewer with OpenSeadragon
   - Zoom, pan, and rotate controls
   - Spectral layer overlays (RGB, Infrared, Ultraviolet, X-Ray)
   - Annotation tools
   - Export functionality
4. **Annotations** - Manage saved annotations with tags and notes
5. **AI Explorer Bot** - Intelligent chatbot for space exploration queries
   - Context-aware responses
   - Suggested questions
   - Voice and image input support
6. **Favorites** - Save and organize favorite discoveries
7. **Time-lapse Generator** - Create videos from NASA imagery
8. **Profile Management** - Customize settings, theme, and language
9. **Contact Support** - Get help with technical issues

### NASA Scientist Features
1. **Dashboard** - Advanced analytics and research overview
2. **Dataset Explorer** - Upload and manage research datasets
   - Support for GeoTIFF, FITS, CSV formats
   - Metadata management
   - Preview and download capabilities
3. **AI Models** - Upload, train, and deploy ML models
   - TensorFlow and PyTorch support
   - Training metrics visualization
   - Model inference and accuracy reports
4. **Data Analytics** - Interactive charts and temporal analysis
   - Recharts visualizations
   - Spectral analysis
   - Comparative studies
5. **Research Insights** - AI-generated research summaries
6. **Collaborative Annotations** - Team-based dataset annotation
7. **Admin Tools** - System configuration and management
8. **AI Research Assistant** - Advanced AI-powered research tools
9. **Profile Management** - Account settings and preferences
10. **Support Center** - Documentation and help resources

## Demo Credentials

### Normal User
- Email: `demo@gmail.com`
- Password: `demo@12345`

### NASA Scientist
- Email: `scientist@nasa.gov`
- Password: `nasa@2024`
- 2FA Code: `123456`

## Technology Stack

- **Frontend**: React 18, TypeScript, Vite
- **Routing**: React Router DOM
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **Image Viewer**: OpenSeadragon
- **Charts**: Recharts
- **Authentication**: Supabase
- **State Management**: React Context API

## Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## Project Structure

```
src/
├── components/          # Reusable components
│   ├── Starfield.tsx   # Animated starfield background
│   ├── Sidebar.tsx     # Collapsible navigation sidebar
│   ├── DashboardLayout.tsx
│   └── ProtectedRoute.tsx
├── contexts/           # React contexts
│   └── AuthContext.tsx # Authentication state management
├── pages/             # Page components
│   ├── LandingPage.tsx
│   ├── UserLogin.tsx
│   ├── ScientistLogin.tsx
│   ├── user/          # Normal user pages
│   └── scientist/     # NASA scientist pages
├── lib/               # Utility libraries
│   └── supabase.ts   # Supabase client configuration
├── App.tsx           # Main application with routing
└── main.tsx          # Application entry point
```

## Key Features Implementation

### Authentication Flow
- Session-based authentication with localStorage persistence
- Protected routes redirect unauthorized users
- Role-based access control prevents cross-role access
- 2FA implementation for enhanced security

### Responsive Design
- Mobile-first approach with Tailwind breakpoints
- Collapsible sidebar for better mobile experience
- Fully responsive layouts across all screen sizes

### Accessibility
- ARIA labels and roles throughout
- Keyboard navigation support
- Screen reader compatible
- Sufficient color contrast ratios

### Performance
- Code splitting with React Router
- Optimized animations with Framer Motion
- Efficient re-rendering with React Context
- Lazy loading for heavy components

## Future Enhancements

- Real NASA API integration for live data
- OpenAI GPT API integration for AI chatbot
- Database persistence with Supabase
- File upload and storage functionality
- Real-time collaboration features
- Video generation for time-lapses
- Advanced ML model deployment

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This project is created for educational and demonstration purposes.
