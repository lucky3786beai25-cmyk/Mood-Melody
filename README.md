# 🎵 Mood Melody - Real-Time Mood-Based Music Recommendation Website

## Project Overview
**Mood Melody** is a premium, modern, fully responsive web application that recommends songs and playlists based on the user's current mood in real-time. The platform features advanced animations, glassmorphism UI, voice recognition, and integration with multiple music APIs.

### Key Features
✨ **Real-Time Mood Detection** - Interactive mood selector with 8 different moods
🎤 **Voice Recognition** - Detect mood using speech (Web Speech API)
🎵 **Music API Integration** - Deezer, Last.fm, and Lyrics.ovh APIs
💾 **Local Storage** - Save favorites, mood history, and preferences
🌓 **Dark/Light Mode** - Premium theme switching
📱 **Fully Responsive** - Desktop, tablet, and mobile optimized
✨ **Advanced Animations** - GSAP-style transitions and floating elements
🔐 **User Authentication** - Login/Signup with validation

---

## 🛠️ Tech Stack
- **HTML5** - Semantic markup
- **CSS3** - Glassmorphism, gradients, animations
- **Vanilla JavaScript** - No frameworks
- **APIs** - Deezer, Last.fm, Lyrics.ovh, Web Speech API
- **Local Storage** - Client-side data persistence
- **Responsive Design** - Mobile-first approach

---

## 📁 Project Structure
```
Mood-Melody/
├── index.html                 # Login/Signup Page
├── welcome.html               # Welcome Splash Page
├── home.html                  # Home Page
├── mood-detection.html        # Mood Detection Page (Main Feature)
├── playlist.html              # Playlist Page
├── favorites.html             # Favorites Dashboard
├── about.html                 # About & Contact Page
│
├── css/
│   ├── common.css             # Global styles
│   ├── animations.css         # Advanced animations
│   ├── responsive.css         # Mobile/Tablet styles
│   ├── login.css              # Login page styles
│   ├── home.css               # Home page styles
│   ├── mood.css               # Mood detection styles
│   ├── playlist.css           # Playlist styles
│   ├── favorites.css          # Favorites page styles
│   └── about.css              # About page styles
│
├── js/
│   ├── main.js                # Global functionality
│   ├── auth.js                # Authentication logic
│   ├── api-handler.js         # API integration
│   ├── mood-detector.js       # Mood detection logic
│   ├── music-player.js        # Music player controls
│   ├── storage.js             # Local storage management
│   ├── ui-animations.js       # UI animations
│   └── theme.js               # Dark/Light mode
│
├── assets/
│   ├── images/
│   │   ├── logo.png           # Mood Melody logo
│   │   ├── favicon.ico        # Favicon
│   │   └── placeholder.png    # Placeholder images
│   ├── sounds/
│   │   └── notification.mp3   # Notification sound
│   └── fonts/
│       └── custom-fonts.css   # Custom typography
│
├── api/
│   ├── deezer-config.js       # Deezer API configuration
│   ├── lastfm-config.js       # Last.fm API configuration
│   └── lyrics-config.js       # Lyrics API configuration
│
└── README.md                  # Project documentation
```

---

## 🚀 Getting Started

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/lucky3786beai25-cmyk/Mood-Melody.git
   cd Mood-Melody
   ```

2. Open `index.html` in a modern web browser (Chrome, Firefox, Safari, Edge)

3. No build process or dependencies required - it's vanilla HTML, CSS, and JavaScript!

### First Time Setup
- Create an account or use test credentials
- Allow microphone access for voice mood detection
- Select your preferred theme (Dark/Light mode)
- Explore moods and get personalized recommendations

---

## 📖 7 Pages Explanation

### 1️⃣ LOGIN / SIGNUP PAGE (`index.html`)
**Purpose**: User authentication and registration

**Features**:
- Split-screen UI design
- Animated background particles
- Form validation with JavaScript
- Remember me functionality
- Forgot password UI
- Smooth page transitions
- Error handling and toast notifications

**Technical Implementation**:
```javascript
// Email validation using regex
// Password strength checker
// LocalStorage for remember me
// Form submission handler
```

---

### 2️⃣ WELCOME SPLASH PAGE (`welcome.html`)
**Purpose**: Greet user after login with animated welcome screen

**Features**:
- Dynamic "Welcome to Mood Melody" popup
- Logo scaling animation
- Music waveform animation
- Auto-transition to homepage after 3 seconds
- Optional background music
- Personalized greeting with username

**Technical Implementation**:
```javascript
// Animation timing using setInterval/setTimeout
// CSS keyframe animations
// Audio API for sound effects
// Automatic redirect after delay
```

---

### 3️⃣ HOME PAGE (`home.html`)
**Purpose**: Main landing page with music discovery

**Features**:
- Hero section with slogan: "Feel the Music That Understands You"
- Dynamic search bar with suggestions
- Trending songs section (API fetched)
- Personalized recommendations
- Recently searched moods
- Animated music cards
- Mini music player
- Quick access to mood detection

**Technical Implementation**:
```javascript
// Fetch trending songs from Deezer API
// Search debouncing for smooth search
// Card animations on load
// Local storage for recent moods
// Mini player controls
```

---

### 4️⃣ MOOD DETECTION PAGE (`mood-detection.html`) ⭐ MAIN FEATURE
**Purpose**: Interactive mood selector with AI-powered recommendations

**8 Moods Available**:
1. 😊 **Happy** - Uplifting, energetic tracks
2. 😢 **Sad** - Emotional, soothing songs
3. 😠 **Angry** - Intense, powerful music
4. 😌 **Relaxed** - Calm, ambient sounds
5. 💕 **Romantic** - Love songs and ballads
6. 🧠 **Focused** - Concentration-enhancing tracks
7. ⚡ **Energetic** - High-energy, dance music
8. 💔 **Heartbroken** - Emotional recovery playlist

**Features**:
- Animated emoji for each mood
- Dynamic background color change
- Mood intensity slider (1-10)
- Voice mood input (speech recognition)
- Text mood input
- Real-time playlist generation
- Personalized recommendations text
- Mood history tracking
- Save mood for later

**Technical Implementation**:
```javascript
// Web Speech API for voice recognition
// Deezer API for mood-based song fetching
// CSS transitions for background changes
// LocalStorage for mood history
// Last.fm API for recommendations
// Dynamic text generation based on mood
```

---

### 5️⃣ PLAYLIST PAGE (`playlist.html`)
**Purpose**: Display and manage playlists with song controls

**Features**:
- Dynamic playlist cards
- Song thumbnails and metadata
- Song name, artist, duration
- Play/Pause button
- Save to favorites button
- Like/Dislike functionality
- Playlist filtering and sorting
- Music player integration
- Share playlist option
- Add to queue feature

**Technical Implementation**:
```javascript
// Fetch playlists from Deezer API
// Track likes/dislikes in localStorage
// Music player event handling
// Dynamic DOM manipulation
// Responsive grid layout
// Filter and sort functionality
```

---

### 6️⃣ FAVORITES DASHBOARD (`favorites.html`)
**Purpose**: User's personal music library and profile

**Features**:
- Saved favorite songs
- Mood history timeline
- Favorite playlists
- Recently played tracks
- User profile section
- Editable username
- Profile picture upload
- Statistics (songs saved, hours listened)
- Export favorites
- Clear history option

**Technical Implementation**:
```javascript
// LocalStorage management for favorites
// File upload for profile picture
// User data management
// Timeline visualization
// Delete/Remove functionality
// Data export to JSON
// Statistics calculation
```

---

### 7️⃣ ABOUT + CONTACT PAGE (`about.html`)
**Purpose**: Project information and user feedback

**Features**:
- Project overview
- Why Mood Melody is unique
- Technologies used with icons
- Contact form
- Feedback system
- Social media links
- FAQ section with accordion
- Developer information
- License information
- Newsletter signup

**Technical Implementation**:
```javascript
// Contact form validation
// Email sending simulation
// Accordion functionality
// Form submission handling
// Social media link integration
// Newsletter subscription
// Error/Success notifications
```

---

## 🎨 Design & UI Details

### Color Palette
**Dark Theme**:
- Primary: #1a1a2e (Deep Black)
- Secondary: #9d4edd (Purple)
- Accent: #00d9ff (Neon Blue)
- Background: #0f0f1e

**Light Theme**:
- Primary: #ffffff (White)
- Secondary: #c77dff (Soft Purple)
- Accent: #00a8e8 (Light Blue)
- Background: #f8f9fa

### Key Design Elements
1. **Glassmorphism** - Frosted glass effect on cards
2. **Gradients** - Smooth color transitions
3. **Animations** - Floating music notes, waveforms
4. **Typography** - Modern fonts (Poppins, Inter)
5. **Shadows** - Subtle depth effects
6. **Hover Effects** - Interactive feedback
7. **Loading Skeletons** - Professional loading states

---

## 🔌 API Integration Guide

### 1. Deezer API
**Purpose**: Fetch songs, albums, artist information

**Endpoint**: `https://api.deezer.com/`

**Key Methods**:
```javascript
// Get song by ID
GET /song/{id}

// Search songs
GET /search?q={query}

// Get artist details
GET /artist/{id}

// Get playlist
GET /playlist/{id}
```

**Example Usage**:
```javascript
const fetchSongs = async (mood) => {
  const response = await fetch(`https://api.deezer.com/search?q=${mood}&limit=20`);
  const data = await response.json();
  return data.data;
};
```

---

### 2. Last.fm API
**Purpose**: Mood-based recommendations and track information

**API Key**: Get from https://www.last.fm/api

**Key Methods**:
```javascript
// Get similar tracks
GET ?method=track.getsimilar&name={track}&artist={artist}

// Get top tracks
GET ?method=geo.gettoptracks&country={country}

// Get track info
GET ?method=track.getinfo&name={track}&artist={artist}
```

---

### 3. Lyrics.ovh API
**Purpose**: Fetch song lyrics

**Endpoint**: `https://api.lyrics.ovh/v1/`

**Example**:
```javascript
const getLyrics = async (artist, song) => {
  const response = await fetch(
    `https://api.lyrics.ovh/v1/${artist}/${song}`
  );
  const data = await response.json();
  return data.lyrics;
};
```

---

### 4. Web Speech API
**Purpose**: Voice mood recognition

**Browser Support**: Chrome, Firefox, Edge, Safari

**Implementation**:
```javascript
const recognition = new webkitSpeechRecognition();
recognition.onresult = (event) => {
  const transcript = event.results[0][0].transcript;
  detectMood(transcript);
};
```

---

## 🎯 Advanced Features Explained

### 1. Real-Time API Music Fetching
- Asynchronous API calls with error handling
- Caching mechanism for faster loading
- Pagination for large results
- Rate limiting awareness

### 2. Voice Recognition Mood Input
- Web Speech API integration
- Mood keyword detection in speech
- Confidence scoring
- Fallback to text input

### 3. Dynamic Background Changing
- CSS transitions for smooth changes
- Mood-specific color schemes
- Intensity-based brightness adjustment
- Animated gradient backgrounds

### 4. Personalized Recommendation Engine
- Mood history analysis
- User preference tracking
- Similar mood recommendations
- Trending songs filtering

### 5. Local Storage Management
```javascript
// Save favorites
localStorage.setItem('favorites', JSON.stringify(favorites));

// Save mood history
localStorage.setItem('moodHistory', JSON.stringify(history));

// Save theme preference
localStorage.setItem('theme', 'dark');
```

### 6. Music Player Controls
- Play/Pause
- Next/Previous
- Progress bar
- Volume control
- Playlist queue
- Shuffle & Repeat

### 7. Loading Skeletons
- Smooth content loading
- Placeholder elements
- Professional appearance
- Better UX

### 8. Toast Notifications
- Success messages
- Error alerts
- Info notifications
- Auto-dismiss
- Stack handling

### 9. Search Suggestions
- Autocomplete functionality
- Recent searches
- Popular moods
- Song/Artist suggestions

### 10. Error Handling
- Try-catch blocks
- Fallback UI
- User-friendly messages
- Console logging for debugging

---

## 🎬 Animation Details

### CSS Animations
1. **Fade In/Out** - Content transitions
2. **Slide** - Navigation effects
3. **Bounce** - Interactive feedback
4. **Float** - Floating music notes
5. **Pulse** - Loading indicators
6. **Rotate** - Spinning loaders
7. **Glow** - Neon effects
8. **Blur** - Background blur on modals

### JavaScript Animations
1. **Keyframe Control** - Smooth transitions
2. **Event-Based** - Interaction feedback
3. **RequestAnimationFrame** - Smooth 60fps animations
4. **CSS Transitions** - Property changes

---

## 📱 Responsive Design

### Breakpoints
- **Desktop**: 1200px and above
- **Tablet**: 768px to 1199px
- **Mobile**: Below 768px

### Mobile Optimizations
- Touch-friendly buttons (min 48px)
- Simplified navigation (hamburger menu)
- Vertical layout
- Optimized font sizes
- Reduced animations
- Fast loading (lazy loading images)

---

## 🔐 Security Considerations

1. **Form Validation** - Client-side and best practices
2. **Local Storage** - Don't store sensitive data
3. **API Keys** - Use environment variables (in production)
4. **HTTPS** - Required for voice recognition
5. **XSS Prevention** - Sanitize user input
6. **CSRF Protection** - Token-based forms

---

## 📊 Viva Explanation Points

### Project Architecture
- Explain 7-page structure
- API integration strategy
- Data flow diagram
- Component interaction

### Key Technologies
- Vanilla JavaScript benefits
- CSS3 modern features
- Web APIs usage
- LocalStorage advantages

### Advanced Features
- Voice recognition implementation
- Real-time mood detection
- Dynamic UI changes
- Recommendation algorithm

### User Experience
- Smooth animations
- Responsive design
- Accessibility features
- Error handling

### Code Quality
- Well-commented code
- Modular structure
- Best practices
- Clean code principles

---

## 🚀 Future Scope & Improvements

### Phase 2 - Backend Integration
- User database (Firebase/Node.js)
- Server-side authentication
- Cloud storage for playlists
- Real-time notifications

### Phase 3 - Advanced AI
- Machine learning for mood detection
- Sentiment analysis
- Neural network recommendations
- Behavioral patterns

### Phase 4 - Social Features
- User profiles
- Share playlists
- Follow friends
- Collaborative playlists
- Comments and reviews

### Phase 5 - Mobile App
- React Native version
- iOS/Android apps
- Push notifications
- Offline mode

### Phase 6 - Premium Features
- Ad-free experience
- Unlimited downloads
- High-quality audio
- Custom playlists
- Priority support

### Additional Improvements
- Spotify API integration
- YouTube Music integration
- Podcast recommendations
- Concert recommendations
- Artist collaboration features
- Mood prediction based on time/date
- Integration with fitness apps
- Ambient sound mixing
- Custom mood creation
- Community playlists

---

## 🎓 How to Present This Project

### Project Summary (2 min)
"Mood Melody is a real-time mood-based music recommendation website that uses mood detection to suggest personalized playlists. It features 7 interconnected pages with advanced animations, API integrations, and a beautiful glassmorphism design."

### Technical Highlights (3 min)
- HTML5 semantic markup
- CSS3 advanced animations and gradients
- Vanilla JavaScript with no frameworks
- Multiple API integrations (Deezer, Last.fm, Lyrics.ovh)
- Web Speech API for voice recognition
- LocalStorage for persistence
- Fully responsive design

### Features Demo (3 min)
1. Show login and welcome animation
2. Navigate through mood detection
3. Show playlist generation
4. Demonstrate voice recognition
5. Show theme switching
6. Display favorites dashboard

### Code Quality (2 min)
- Well-structured folder organization
- Clean, commented code
- Modular JavaScript files
- Separated CSS concerns
- Error handling throughout
- Best practices followed

---

## 📝 License
MIT License - Feel free to use and modify

## 👨‍💻 Developer
Created with ❤️ by lucky3786beai25-cmyk

## 🙏 Acknowledgments
- Deezer API for music data
- Last.fm for recommendations
- Web Speech API for voice recognition
- Inspiration from Spotify, Apple Music, Netflix

---

**Happy Coding! 🎵✨**
