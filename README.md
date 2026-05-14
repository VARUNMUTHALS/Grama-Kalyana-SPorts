# Grama Kalyana Sports

A professional local sports tournament management application for Cricket, Kabaddi, and Volleyball with live scoring capabilities.

## 🏏 Features

### Core Features
- **Tournament Management**: Create and manage tournaments for multiple sports
- **Team Management**: Add teams and players with detailed profiles
- **Live Scoring**: Real-time score updates with professional scoreboard interface
- **Public Live View**: Fans can watch live scores remotely
- **Player Statistics**: Track career statistics, man of the match awards, and performance history

### Sports Supported
- 🏏 **Cricket**: Full cricket scoring with runs, wickets, overs, and statistics
- 🤼 **Kabaddi**: Kabaddi scoring with raid points, tackle points, and player tracking
- 🏐 **Volleyball**: Volleyball scoring with sets, points, and match statistics

### Technical Features
- **Real-time Updates**: Firebase Realtime Database for live score synchronization
- **Authentication**: Firebase Authentication for secure user management
- **Cloud Storage**: Firebase Storage for team logos and player photos
- **Offline Support**: Offline mode for viewing downloaded matches
- **Professional UI**: Bold sports interface with high contrast colors and large typography

## 🎨 Design System

### Color Scheme
- **Primary**: Neon Orange (#FF6B35)
- **Background**: Matte Black (#1A1A1A)
- **Text**: White (#FFFFFF)
- **Accent**: Neon Green, Neon Blue, Neon Red

### Typography
- Large scoreboard fonts for outdoor readability
- High contrast text for visibility
- Bold sports-themed styling

## 🏗️ Architecture

### MVVM Architecture
- **Model**: Data classes for Tournament, Team, Player, Match, LiveScore
- **View**: Jetpack Compose UI with Material 3 components
- **ViewModel**: Business logic and state management
- **Repository**: Data access layer with Firebase integration

### Package Structure
```
com.gramakalyana.sports
├── data/           # Data sources and repositories
├── ui/             # UI components and screens
│   ├── components/ # Reusable UI components
│   ├── screens/    # App screens
│   └── theme/      # Theme and styling
├── viewmodel/      # ViewModels
├── repository/     # Repository implementations
├── firebase/       # Firebase configuration
├── models/         # Data models
├── navigation/     # Navigation setup
└── utils/          # Utility classes and extensions
```

## 🚀 Getting Started

### Prerequisites
- Android Studio Arctic Fox or later
- Kotlin 1.9.0+
- Android SDK 24+ (Android 7.0)
- Firebase project setup

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd grama-kalyana-sports
   ```

2. **Firebase Setup**
   - Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Authentication, Realtime Database, and Storage
   - Download `google-services.json` and place it in `app/` directory
   - Update Firebase configuration in `firebase/FirebaseConfig.kt`

3. **Build and Run**
   - Open the project in Android Studio
   - Sync Gradle dependencies
   - Run the app on an emulator or device

## 📱 App Structure

### Main Screens
- **Home**: Dashboard with quick actions and featured sports
- **Tournaments**: List and manage tournaments
- **Live Scores**: View live matches and scores
- **Statistics**: Player and team statistics
- **Settings**: App preferences and configuration

### Key Components
- **Scoreboard Components**: Professional scoreboards for each sport
- **Scorer Controls**: Large, touch-friendly controls for live scoring
- **Navigation**: Bottom navigation with drawer support
- **Authentication**: Login and registration flows

## 🔧 Configuration

### Firebase Configuration
Update the following in `firebase/FirebaseConfig.kt`:
- Database URLs
- Storage paths
- Authentication methods

### Theme Customization
Modify colors and styles in:
- `ui/theme/Color.kt`
- `ui/theme/Type.kt`
- `res/values/colors.xml`
- `res/values/themes.xml`

## 📊 Data Models

### Core Models
- **Tournament**: Tournament details, format, and status
- **Team**: Team information, players, and statistics
- **Player**: Player profiles and career statistics
- **Match**: Match details and scores
- **LiveScore**: Real-time scoring data

### Sport-Specific Models
- **CricketScore**: Runs, wickets, overs, and cricket statistics
- **KabaddiScore**: Raid points, tackle points, and kabaddi statistics
- **VolleyballScore**: Sets, points, and volleyball statistics

## 🎯 Usage

### Creating a Tournament
1. Navigate to Tournaments → Create Tournament
2. Enter tournament details (name, sport, dates, venue)
3. Add participating teams
4. Create match schedule

### Live Scoring
1. Go to Live Scores → Select match
2. Use scorer controls to update scores
3. Scores update in real-time for all viewers
4. Public viewers can watch live scores

### Managing Teams and Players
1. Add teams with logos and details
2. Add players with photos and jersey numbers
3. Track player statistics across tournaments

## 🛠️ Development

### Building the App
```bash
./gradlew assembleDebug
```

### Running Tests
```bash
./gradlew test
```

### Code Style
- Follow Kotlin coding conventions
- Use meaningful variable and function names
- Add comments for complex logic
- Use Material 3 design guidelines

## 📦 Dependencies

### Core Dependencies
- **Jetpack Compose**: Modern UI toolkit
- **Navigation Compose**: Navigation component
- **Material 3**: Design system
- **Firebase**: Backend services
- **Hilt**: Dependency injection
- **Coroutines**: Asynchronous programming

### UI Dependencies
- **Accompanist**: Additional Compose utilities
- **Coil**: Image loading
- **Material Icons**: Icon library

## 🔒 Security

- Firebase Authentication for user management
- Firebase Security Rules for data protection
- Input validation for all user inputs
- Secure storage for sensitive data

## 🌐 Network

- Firebase Realtime Database for real-time updates
- Firebase Storage for file uploads
- Offline support with data synchronization
- Error handling and retry mechanisms

## 📈 Performance

- Lazy loading for large lists
- Image caching and optimization
- Efficient state management
- Memory leak prevention

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📞 Support

For support and questions:
- Create an issue in the repository
- Contact the development team
- Check the documentation

## 🔄 Updates

### Version 1.0.0
- Initial release with core features
- Support for Cricket, Kabaddi, and Volleyball
- Live scoring capabilities
- Tournament management
- Player statistics

### Planned Features
- Video streaming for live matches
- Advanced analytics dashboard
- Multi-language support
- Wear OS companion app
- Web dashboard for tournament organizers

---

**Grama Kalyana Sports** - Professional Tournament Management Made Simple 🏆
