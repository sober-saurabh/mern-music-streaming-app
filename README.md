# mern-music-streaming-app
Professional music streaming app with audio visualization, EQ, and analytics

# 🎵 MERN Music Streaming Application

<div align="center">
  <img src="https://img.shields.io/badge/React-18.2.0-blue?style=for-the-badge&logo=react" alt="React" />
  <img src="https://img.shields.io/badge/Node.js-18+-green?style=for-the-badge&logo=node.js" alt="Node.js" />
  <img src="https://img.shields.io/badge/MongoDB-7.0+-green?style=for-the-badge&logo=mongodb" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Express.js-4.18+-lightgrey?style=for-the-badge&logo=express" alt="Express" />
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="License" />
</div>

<div align="center">
  <h3>🎶 Professional Music Streaming Platform with Advanced Audio Processing</h3>
  <p>A full-stack music streaming application featuring real-time audio visualization, 10-band equalizer, multi-format support, and comprehensive analytics.</p>
</div>

## ✨ Features

### 🎵 **Core Music Features**
- **Advanced Audio Player** - Play/pause/skip/repeat/shuffle with seamless transitions
- **Multi-Format Support** - MP3, FLAC, WAV, AAC, OGG, M4A with automatic format detection
- **10-Band Equalizer** - Real-time audio processing with custom presets (Rock, Pop, Jazz, Classical)
- **Audio Visualization** - Real-time frequency spectrum display using Web Audio API
- **Smart Playlist Management** - Create, edit, share, and collaborate on playlists

### 📊 **Analytics & Admin**
- **Detailed Play Analytics** - Track individual song plays, completion rates, and user engagement
- **Format Distribution** - Monitor audio quality preferences and storage usage
- **User Dashboard** - Comprehensive statistics for administrators
- **Real-time Monitoring** - Live user activity and system performance metrics

### 🎨 **Modern UI/UX**
- **Glassmorphism Design** - Contemporary visual aesthetics with backdrop blur effects
- **Responsive Layout** - Seamless experience across desktop, tablet, and mobile
- **Dark Theme Optimized** - Easy on the eyes with professional color schemes
- **Smooth Animations** - 60fps transitions and micro-interactions

### 🔒 **Security & Performance**
- **JWT Authentication** - Secure user sessions with role-based access control
- **File Upload Validation** - Comprehensive audio format and size validation
- **Rate Limiting** - API protection against abuse and DDoS
- **Database Optimization** - Indexed queries and efficient data structures

## 🚀 Quick Start

### Prerequisites
- **Node.js** (v16 or higher)
- **MongoDB** (local installation or Atlas cloud)
- **Git** for version control

### 1. Clone Repository
```bash
git clone https://github.com/sober-saurabh/mern-music-streaming-app.git
cd mern-music-streaming-app
```

### 2. Install Dependencies
```bash
npm run install:all
```

### 3. Environment Setup
```bash
# Backend environment
cp backend/.env.example backend/.env
# Edit backend/.env with your MongoDB URI and JWT secret

# Frontend environment
cp frontend/.env.example frontend/.env
# Edit frontend/.env if needed
```

### 4. Start Development
```bash
# Start both frontend and backend
npm run dev

# Or separately:
npm run dev:backend  # Backend on http://localhost:5000
npm run dev:frontend # Frontend on http://localhost:3000
```

## 🐳 Docker Deployment

### Quick Start with Docker
```bash
# Build and run all services
npm run docker:up

# Access the application
# Frontend: http://localhost:3000
# Backend API: http://localhost:5000
# MongoDB: localhost:27017
```

## 🌐 Production Deployment

### Railway (Recommended)
```bash
# Install Railway CLI
npm install -g @railway/cli

# Deploy
railway login
railway create mern-music-app
railway up
```

### Other Platforms
- **Netlify + MongoDB Atlas** - Frontend on Netlify, API on Railway
- **Vercel** - Full-stack deployment with serverless functions
- **Heroku** - Traditional PaaS deployment
- **AWS/GCP/Azure** - Cloud provider deployment

## 📱 API Documentation

### Authentication Endpoints
```
POST /api/auth/register    # User registration
POST /api/auth/login       # User login
GET  /api/auth/profile     # Get user profile
```

### Track Management
```
GET    /api/tracks         # Get all tracks
POST   /api/tracks         # Upload new track
PUT    /api/tracks/:id     # Update track
DELETE /api/tracks/:id     # Delete track
POST   /api/tracks/:id/play # Record play event
```

### Analytics (Admin Only)
```
GET /api/analytics/overview    # General statistics
GET /api/analytics/tracks/:id  # Detailed track analytics
GET /api/analytics/users       # User engagement metrics
```

## 🎯 Browser Support

| Browser | Version | Status |
|---------|---------|---------|
| Chrome | 80+ | ✅ Full Support |
| Firefox | 75+ | ✅ Full Support |
| Safari | 13+ | ✅ Full Support |
| Edge | 80+ | ✅ Full Support |

**Requirements:** Web Audio API, ES6+, Canvas API

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guide](docs/CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

### Development Setup
```bash
# Install dependencies for both frontend and backend
npm run install:all

# Run development servers concurrently
npm run dev

# Run tests
npm test

# Build for production
npm run build
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Web Audio API** for advanced audio processing capabilities
- **React** and **Node.js** communities for excellent documentation
- **MongoDB** for flexible data storage
- **Tailwind CSS** for rapid UI development

## 📞 Support

- **Documentation**: Check the [`docs/`](docs/) directory
- **Issues**: [GitHub Issues](https://github.com/sober-saurabh/mern-music-streaming-app/issues)
- **Discussions**: [GitHub Discussions](https://github.com/sober-saurabh/mern-music-streaming-app/discussions)

---

<div align="center">
  <p>Built with ❤️ using the MERN Stack</p>
  <p>⭐ Star this repository if you found it helpful!</p>
  <p>
    <a href="#top">Back to top</a> •
    <a href="docs/API.md">API Docs</a> •
    <a href="docs/DEPLOYMENT.md">Deploy Guide</a> •
    <a href="docs/CONTRIBUTING.md">Contributing</a>
  </p>
</div>
