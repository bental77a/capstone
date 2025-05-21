# Connect & Play

## 🏆 Project Vision

SportsMeet was born from a simple frustration - trying to organize pickup games through cluttered community apps with excessive content. Our platform strips away the noise, focusing solely on connecting sports enthusiasts for real-world games and events.

## ✨ Key Features

- **Live Event Tracking**: Events automatically become inactive after their scheduled end time
- **Streamlined Experience**: Clean UI focused exclusively on sports meetups
- **Secure Authentication**: Complete password reset functionality via email
- **Location Intelligence**: Google Maps Places API integration for accurate meetup coordination
- **Mobile Responsive**: Fully functional across all device sizes

## 🛠️ Technical Architecture

### Backend (Django)
- **User Model**: Extended from Django's AbstractUser
- **Events Model**: Comprehensive event management with many-to-many user relationships
- **Email Integration**: Yahoo SMTP server for reliable communication
- **Form Validation**: Custom Django widgets for enhanced input validation

### Frontend
- Dynamic content loading with JavaScript
- Responsive design with custom CSS
- Interactive map integration

## 📁 Project Structure

```
capstone/
├── .env                  # Environment variables (API keys, email credentials)
├── settings.py           # Project configuration (timezone, media storage, etc.)
├── urls.py               # Project-level URL routing
├── media/images/         # User-uploaded media storage
├── sports/               # Main application directory
│   ├── static/
│   │   ├── scripts.js    # Core frontend functionality
│   │   └── styles.css    # Application styling
│   ├── templates/
│   │   ├── registration/ # Authentication templates
│   │   └── sports/       # Main application templates
│   ├── admin.py          # Admin panel configuration
│   ├── models.py         # Database schema
│   ├── urls.py           # Application-level URL routing
│   └── views.py          # Request handling logic
└── db.sqlite3            # SQLite database
```

## 📊 JavaScript Functionality

- Current/future event display
- Past event archives
- Detailed event view
- User attendance management
- Event creation/cancellation flows
- Location autocomplete via Google API
- CSRF-protected operations

## 🚀 Getting Started

1. **Prerequisites**
   - Python 3.x
   - pip

2. **Installation**
   ```bash
   # Clone repository
   git clone <repository-url>
   cd capstone
   
   # Set up virtual environment
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   
   # Install dependencies
   pip install -r requirements.txt
   
   # Run migrations
   python manage.py migrate
   
   # Start development server
   python manage.py runserver
   ```

3. **Access the application**
   - Open your browser and navigate to http://127.0.0.1:8000/

## 🌟 What Sets This Project Apart

This project distinguishes itself from typical CRUD applications by focusing on real-time community connection for physical activities. The integration of temporal event management, location services, and streamlined user experience creates a purposeful platform that solves a genuine need for sports enthusiasts looking to organize games without unnecessary complexity.
