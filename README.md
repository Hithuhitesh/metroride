# 🚴‍♂️ Bike Rental Management System

A comprehensive Android application for bike rental management with admin panel, real-time tracking, and payment integration.

## 📱 **Screenshots**

| Login Screen | Admin Dashboard | Bike List | Booking History |
|--------------|----------------|-----------|-----------------|
| ![Login](screenshots/login.png) | ![Admin](screenshots/admin.png) | ![Bikes](screenshots/bikes.png) | ![Bookings](screenshots/bookings.png) |

## ✨ **Features**

### **User Features:**
- 🔐 **Secure Authentication** - Email/password login with validation
- 🚴‍♂️ **Browse Bikes** - View available bikes by location and type
- 📅 **Book Bikes** - Hourly and daily rental options
- 💳 **Payment Integration** - Secure payment processing
- 📍 **Location Services** - GPS-based bike location tracking
- 📊 **Booking History** - View past and current bookings
- ⭐ **Rating System** - Rate bikes and services

### **Admin Features:**
- 👥 **User Management** - View and manage all users
- 🚴‍♂️ **Bike Management** - Add, edit, delete bikes
- 📊 **Analytics Dashboard** - Revenue, bookings, user statistics
- 📍 **Location Management** - Manage bike pickup locations
- 💰 **Revenue Tracking** - Daily, weekly, monthly reports
- 🔧 **System Settings** - Configure pricing, locations, features

## 🛠️ **Technology Stack**

- **Frontend:** Android (Kotlin)
- **Backend:** PHP with MySQL
- **Database:** MySQL
- **API:** RESTful API
- **Authentication:** JWT tokens
- **Payment:** Razorpay integration
- **Maps:** Google Maps API
- **Architecture:** MVVM pattern

## 📋 **Prerequisites**

- Android Studio Arctic Fox or later
- Android SDK 21+ (Android 5.0)
- PHP 7.4+
- MySQL 5.7+
- XAMPP/WAMP for local development

## 🚀 **Installation**

### **1. Clone Repository**
```bash
git clone https://github.com/YOUR_USERNAME/bike-rental-android-app.git
cd bike-rental-android-app
```

### **2. Database Setup**
1. Start XAMPP/WAMP
2. Import `database/bike_rental.sql` to MySQL
3. Update database credentials in `app/src/main/java/com/example/bikerental/Config.kt`

### **3. Backend Setup**
1. Copy backend files to `htdocs/myproject/`
2. Update database connection in `api/db.php`
3. Configure Google Maps API key

### **4. Android Setup**
1. Open project in Android Studio
2. Sync Gradle files
3. Update API endpoints in `Config.kt`
4. Add Google Maps API key to `google_maps_api.xml`
5. Build and run the project

## 📁 **Project Structure**

```
app/
├── src/main/
│   ├── java/com/example/bikerental/
│   │   ├── activities/          # All activity classes
│   │   ├── adapters/           # RecyclerView adapters
│   │   ├── models/             # Data models
│   │   ├── utils/              # Utility classes
│   │   └── Config.kt           # API configuration
│   ├── res/
│   │   ├── layout/             # XML layouts
│   │   ├── drawable/           # Images and icons
│   │   ├── values/             # Strings, colors, styles
│   │   └── mipmap/             # App icons
│   └── AndroidManifest.xml
├── build.gradle.kts            # App-level dependencies
└── proguard-rules.pro

backend/
├── api/                        # PHP API endpoints
├── database/                   # SQL files
└── uploads/                    # File uploads
```

## 🔧 **Configuration**

### **API Configuration**
Update `Config.kt` with your server details:
```kotlin
object Config {
    const val BASE_URL = "http://your-domain.com/myproject/api/"
    const val GOOGLE_MAPS_API_KEY = "your-maps-api-key"
}
```

### **Database Configuration**
Update `api/db.php`:
```php
$host = 'localhost';
$dbname = 'bikerental';
$username = 'root';
$password = '';
```

## 📊 **Database Schema**

### **Main Tables:**
- `users` - User accounts and profiles
- `admins` - Admin user management
- `bikes` - Bike inventory and details
- `bookings` - Rental transactions
- `locations` - Pickup/drop locations
- `payments` - Payment records

## 🔐 **Authentication**

- **JWT Token-based** authentication
- **Password hashing** with bcrypt
- **Session management** for admin panel
- **Role-based access** control

## 💳 **Payment Integration**

- **Razorpay** payment gateway
- **Multiple payment methods** (UPI, cards, net banking)
- **Secure transaction** processing
- **Payment verification** and confirmation

## 📍 **Location Services**

- **Google Maps** integration
- **GPS tracking** for bike locations
- **Geofencing** for pickup/drop zones
- **Route optimization** for delivery

## 🎨 **UI/UX Features**

- **Material Design** components
- **Dark/Light theme** support
- **Responsive layouts** for different screen sizes
- **Smooth animations** and transitions
- **Intuitive navigation** with bottom navigation

## 📱 **Screens**

### **User Screens:**
1. **Splash Screen** - App loading and branding
2. **Login/Register** - Authentication
3. **Home** - Featured bikes and quick actions
4. **Bike List** - Browse available bikes
5. **Bike Details** - View bike information and book
6. **Booking** - Select dates and payment
7. **My Bookings** - View booking history
8. **Profile** - User account management

### **Admin Screens:**
1. **Admin Login** - Admin authentication
2. **Dashboard** - Analytics and overview
3. **User Management** - Manage users
4. **Bike Management** - Manage bike inventory
5. **Booking Management** - View all bookings
6. **Analytics** - Revenue and usage reports
7. **Settings** - System configuration

## 🚀 **Getting Started**

1. **Clone the repository**
2. **Set up the database** using provided SQL files
3. **Configure API endpoints** in the Android app
4. **Add Google Maps API key**
5. **Build and run** the application

## 📈 **Future Enhancements**

- [ ] **Push notifications** for booking updates
- [ ] **Real-time chat** support
- [ ] **Bike maintenance** tracking
- [ ] **Loyalty program** for frequent users
- [ ] **Multi-language** support
- [ ] **Offline mode** for basic functionality

## 🤝 **Contributing**

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 **Developer**

**Pavan Kumar**  
Computer Science Student  
Email: pavan@example.com

## 🏫 **College Project**

This project was developed as part of the Computer Science curriculum for college verification and assessment.

---

**Built with ❤️ for better bike rental management**

