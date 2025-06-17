# Nxt Watch 🎥

**🌐 Live Demo**: [https://charanwatch.ccbp.tech/](https://charanwatch.ccbp.tech/)

A modern video streaming platform built with React.js, featuring user authentication, video browsing, and personalized video management with both light and dark themes.

## 🌟 Features

### 🔐 Authentication
- Secure login system with JWT token authentication
- Protected routes for authenticated users
- Automatic redirection based on authentication status
- Show/hide password functionality

### 🏠 Video Browsing
- **Home Route**: Browse all videos with search functionality
- **Trending Route**: Discover trending videos
- **Gaming Route**: Explore gaming content
- **Video Details**: Watch videos with React Player integration

### 💾 Personal Features
- **Saved Videos**: Save and manage your favorite videos
- Like/Dislike functionality for videos
- Persistent saved videos across sessions

### 🎨 Theming
- **Light Theme**: Clean, bright interface
- **Dark Theme**: Modern, eye-friendly dark mode
- Theme persistence across all routes

### 📱 Responsive Design
- Mobile-first approach
- Responsive layouts for all screen sizes:
  - Extra Small (< 576px)
  - Small (≥ 576px)
  - Medium (≥ 768px)
  - Large (≥ 992px)
  - Extra Large (≥ 1200px)

## 🚀 Live Demo

### 📹 Application Demo Videos

#### **✅ Success Flow Demo**
<div align="center">
  
  **Main Application Features**
  
  <video width="80%" controls>
    <source src="https://assets.ccbp.in/frontend/content/react-js/nxt-watch-output-v0.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  
  *Showcases: Login → Home → Video Search → Trending → Gaming → Video Details → Save Functionality*
  
</div>

#### **❌ Error Handling Demo**
<div align="center">
  
  **Failure Scenarios & Error States**
  
  <video width="80%" controls>
    <source src="https://assets.ccbp.in/frontend/content/react-js/nxt-watch-failure-output-v0.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  
  *Demonstrates: Login Errors → API Failures → Network Issues → Retry Functionality*
  
</div>

### 🎬 Alternative Demo Links
> **Note:** If videos don't display in your README viewer, click the links below:

| Demo Type | Direct Link | Description |
|-----------|-------------|-------------|
| 🎯 **Success Flow** | [▶️ Watch Demo](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-output-v0.mp4) | Complete app walkthrough |
| ⚠️ **Error Handling** | [▶️ Watch Demo](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-failure-output-v0.mp4) | Error states & recovery |

### 🖼️ Screenshots Preview

<details>
<summary>📱 Click to view app screenshots</summary>

#### Light Theme
| Home | Trending | Gaming |
|------|----------|---------|
| ![Home Light](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-home-success-light-theme-lg-output-v0.png) | ![Trending Light](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-trending-success-light-theme-lg-output-v0.png) | ![Gaming Light](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-gaming-success-light-theme-lg-output-v0.png) |

#### Dark Theme
| Home | Trending | Gaming |
|------|----------|---------|
| ![Home Dark](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-home-success-dark-theme-lg-output-v0.png) | ![Trending Dark](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-trending-success-dark-theme-lg-output-v0.png) | ![Gaming Dark](https://assets.ccbp.in/frontend/content/react-js/nxt-watch-gaming-success-dark-theme-lg-output-v0.png) |

</details>

## 🛠️ Built With

- **React.js** - Frontend framework
- **React Router** - Navigation and routing
- **Styled Components** - Component styling
- **React Player** - Video playback
- **React Popup** - Modal dialogs
- **Date-fns** - Date formatting
- **React Loader Spinner** - Loading states
- **React Icons** - Icon components
- **JWT** - Authentication tokens

## 📋 Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

## ⚡ Quick Start

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/nxt-watch.git

# Navigate to project directory
cd nxt-watch

# Install dependencies
npm install

# Start the development server
npm start
```

The application will open in your browser at `http://localhost:3000`

### Login Credentials

```
Username: rahul
Password: rahul@2021
```

## 🗂️ Project Structure

```
src/
├── components/
│   ├── Header/
│   ├── Sidebar/
│   ├── VideoCard/
│   ├── VideoPlayer/
│   ├── Login/
│   ├── Home/
│   ├── Trending/
│   ├── Gaming/
│   ├── SavedVideos/
│   ├── VideoItemDetails/
│   ├── NotFound/
│   └── ProtectedRoute/
├── context/
│   └── ThemeContext.js
├── App.js
└── index.js
```

## 🎯 Routes

| Route | Component | Description |
|-------|-----------|-------------|
| `/` | Home | Browse all videos with search |
| `/login` | Login | User authentication |
| `/trending` | Trending | Trending videos |
| `/gaming` | Gaming | Gaming content |
| `/saved-videos` | SavedVideos | User's saved videos |
| `/videos/:id` | VideoItemDetails | Individual video player |
| `/not-found` | NotFound | 404 error page |

## 🔌 API Integration

### Authentication
- **POST** `/login` - User authentication
- Returns JWT token for protected routes

### Video Data
- **GET** `/videos/all` - Home videos with search
- **GET** `/videos/trending` - Trending videos
- **GET** `/videos/gaming` - Gaming videos
- **GET** `/videos/:id` - Individual video details

All API requests include JWT token authentication for protected content.

## ✨ Key Functionalities

### Video Management
- Search videos on home page
- Browse categorized content (Trending, Gaming)
- Save/unsave videos to personal collection
- Like/dislike videos with state management

### User Experience
- Smooth loading states with spinners
- Error handling with retry functionality
- Responsive video player
- Intuitive navigation with sidebar
- Theme toggle in header

### State Management
- Theme context for global theme state
- Video interaction states (like, dislike, saved)
- Authentication state management
- Search and filter states

## 🎨 Design System

### Color Palette

#### Light Theme
- Background: `#f9f9f9`
- Cards: `#ffffff`
- Text Primary: `#231f20`
- Text Secondary: `#64748b`

#### Dark Theme
- Background: `#0f0f0f`
- Cards: `#181818`
- Text Primary: `#ffffff`
- Text Secondary: `#94a3b8`

#### Interactive Elements
- Primary Blue: `#3b82f6`
- Active State: `#2563eb`
- Error Red: `#ff0000`

### Typography
- Font Family: Roboto
- Responsive font sizes
- Proper contrast ratios for accessibility

## 🧪 Testing

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Generate coverage report
npm run test:coverage
```

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🚀 Deployment

### Build for Production

```bash
npm run build
```

This creates an optimized production build in the `build` folder.

### Environment Variables

Create a `.env` file in the root directory:

```env
REACT_APP_API_BASE_URL=https://apis.ccbp.in
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow React best practices
- Use functional components with hooks
- Implement proper error boundaries
- Write meaningful commit messages
- Ensure responsive design
- Test on multiple screen sizes



## 🙏 Acknowledgments

- Design inspiration from modern video platforms
- Icons provided by React Icons
- Video content from CCBP APIs
- React community for excellent tooling

## 📞 Support

For support and questions:
- Create an issue in the repository
- Contact: yedidacharan931@gmail.com

## 🔄 Version History

- **v1.0.0** - Initial release with core functionality
- **v1.1.0** - Added dark theme support
- **v1.2.0** - Enhanced responsive design
- **v1.3.0** - Performance optimizations

---

**Made with ❤️ using React.js**
