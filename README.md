# HealthHub - Your Complete Health and Wellness Platform

HealthHub is a comprehensive health management platform that helps users track their fitness, nutrition, and overall wellness goals. The application provides personalized diet recommendations, calorie tracking, and health management features through a modern, user-friendly interface.

## Features

- **User Management**: Secure authentication and personalized user profiles
- **Health Management**: Track and monitor your health metrics
- **Diet Recommendations**: Get personalized diet plans based on your health goals
- **Calorie Tracking**: Monitor your daily calorie intake and burnt calories
- **Nutrition Recommendations**: Receive tailored nutrition advice
- **Interactive Dashboard**: Visualize your health progress with intuitive charts and metrics

## Technology Stack

### Frontend
- React.js (v18)
- Material-UI (MUI) for component styling
- TailwindCSS for custom styling
- React Router for navigation
- Axios for API communication
- Framer Motion for animations
- React Toastify for notifications
- React Gauge Chart for data visualization

### Backend (Microservices Architecture)
- API Gateway
- Eureka Server for service discovery
- Multiple specialized microservices:
  - User Management Service
  - Health Management Service
  - Diet Recommendation Service
  - Calories Burnt Service
  - Nutrition Recommendation Service

## 📁 Project Structure

```
HealthHub/
├── frontend/
│   ├── src/                    # Source code directory
│   │   ├── components/         # React components
│   │   ├── pages/             # Page components
│   │   ├── assests/           # Assests functions
│   │   ├── App.js             # Main App component
│   │   └── index.css
|   |   └── index.js
|   |   └── App.css
│   ├── public/                 # Public assets
│   ├── package.json           # Frontend dependencies and scripts
│   ├── package-lock.json      # Locked versions of dependencies
│   └── tailwind.config.js     # Tailwind CSS configuration
└── backend/
    ├── API-Gateway/           # API Gateway Service
    │   ├── src/
    │   └── pom.xml
    ├── EurekaServer/          # Service Discovery
    │   ├── src/
    │   └── pom.xml
    ├── User-Management-Service/
    ├── Health-Management-Service/
    ├── Diet-Recommendation-Service/
    ├── Calories-Burnt-Service/
    └── Nutrition-Rec/
```

##  Configuration Files

### Frontend Configuration
1. **package.json**
   - Defines project dependencies
   - Scripts for development, building, and testing
   - Project metadata

2. **package-lock.json**
   - Locks dependency versions for consistent installations
   - Ensures same versions across team members

3. **tailwind.config.js**
   - Tailwind CSS customization
   - Theme configuration
   - Custom utility classes

4. **.env** (create this file)
   ```
   REACT_APP_API_URL=http://localhost:8080
   ```

### Backend Configuration
1. **pom.xml** (in each service)
   - Maven dependencies
   - Build configuration
   - Project properties

2. **application.properties/yml** (in each service)
   - Service configuration
   - Database connections
   - Server ports

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Java (v11 or higher)
- Maven
- npm or yarn

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create `.env` file with necessary environment variables

4. Start the development server:
   ```bash
   npm start
   ```

### Backend Setup
1. Start the Eureka Server:
   ```bash
   cd backend/EurekaServer
   mvn spring-boot:run
   ```

2. Start the API Gateway:
   ```bash
   cd backend/API-Gateway
   mvn spring-boot:run
   ```

3. Start individual microservices (repeat for each service):
   ```bash
   cd backend/<service-name>
   mvn spring-boot:run
   ```

## Testing

### Frontend Testing
```bash
cd frontend
npm test
```

### Backend Testing
```bash
cd backend/<service-name>
mvn test
```

## Building for Production

### Frontend Build
```bash
cd frontend
npm run build
```

### Backend Build
```bash
cd backend/<service-name>
mvn clean package
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- Harika Gummadi

## Acknowledgments

- Thanks to all contributors who have helped shape HealthHub
- Special thanks to the open-source community for the amazing tools and libraries 
