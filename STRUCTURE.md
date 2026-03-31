# Folder Structure Documentation

## 📁 Project Organization

This document explains the folder structure and file organization of the RecyConnect project.

## Root Directory Structure

```
RecyConnect/
├── css/                 # Stylesheets for all pages
├── js/                  # JavaScript functionality
├── data/                # Application data storage
├── uploads/             # User uploaded files
├── includes/            # Reusable HTML components
├── *.html              # HTML pages
├── server.js           # Main Express server
├── package.json        # Node.js dependencies
├── .gitignore          # Git ignore rules
├── LICENSE             # MIT License
└── README.md           # Project documentation
```

## 📂 Detailed Breakdown

### `/css/` - Stylesheets
Contains CSS files organized by functionality:

- **`style.css`** - Main global styles and responsive design
- **`navbar.css`** - Navigation component styles
- **`dashboard.css`** - General dashboard styling
- **`donor-dashboard.css`** - Donor-specific dashboard styles
- **`farmer-dashboard.css`** - Farmer-specific dashboard styles
- **`upcycler-dashboard.css`** - Upcycler-specific dashboard styles
- **`chat.css`** & **`chat-new.css`** - Chat interface styling
- **`food-surplus.css`** - Food surplus page styles
- **`agricultural-waste.css`** - Agricultural waste page styles
- **`upcycling.css`** - Upcycling marketplace styles
- **`ai-recommendations.css`** - AI recommendations interface
- **`map.css`** & **`map-interactive.css`** - Map component styles
- **`admin.css`** - Admin panel styling
- **`impact.css`** - Impact and analytics styling
- **`home.css`** - Homepage specific styles

### `/js/` - JavaScript Files
Contains JavaScript functionality organized by feature:

- **`main.js`** - Global JavaScript functions and utilities
- **`auth.js`** - Authentication and user management
- **`dashboard.js`** - General dashboard functionality
- **`donor-dashboard.js`** - Donor dashboard specific logic
- **`farmer-dashboard.js`** - Farmer dashboard specific logic
- **`upcycler-dashboard.js`** - Upcycler dashboard specific logic
- **`chat.js`** - Real-time chat functionality
- **`food-surplus.js`** & **`food-surplus-fixed.js`** - Food surplus management
- **`agricultural-waste.js`** - Agricultural waste handling
- **`ai-recommendations.js`** - AI-powered recommendations
- **`map-leaflet.js`** & **`map-interactive.js`** - Map functionality
- **`resources.js`** - Resource management utilities
- **`admin-users.js`** - Admin user management
- **`include-html.js`** - HTML component inclusion utility

### `/data/` - Data Storage
Application data files:
- **`surplus.json`** - Food surplus items database
- Additional JSON files for other data types

### `/uploads/` - File Uploads
User-uploaded content:
- Images for surplus items
- Product photos
- Profile pictures
- *Note: Directory is tracked by git, but contents are ignored*

### `/includes/` - Reusable Components
Shared HTML components:
- Navigation bars
- Footers
- Common UI elements

## 📄 HTML Pages

### Main Pages
- **`index.html`** - Homepage and landing page
- **`about.html`** - About us and mission
- **`contact.html`** - Contact form and information
- **`how-it-works.html`** - Platform explanation

### Feature Pages
- **`dashboard.html`** - Main user dashboard
- **`donor-dashboard.html`** - Donor-specific dashboard
- **`farmer-dashboard.html`** - Farmer-specific dashboard
- **`upcycler-dashboard.html`** - Upcycler-specific dashboard
- **`admin-users.html`** - Admin user management

### Functional Pages
- **`post-surplus.html`** - Form to post surplus items
- **`food-surplus.html`** - Browse food surplus
- **`agricultural-waste.html`** - Agricultural waste marketplace
- **`upcycling.html`** - Upcycling marketplace
- **`ai-recommendations.html`** - AI recommendations interface

### Interactive Pages
- **`chat.html`** - Real-time chat interface
- **`map.html`** - Basic map view
- **`map-interactive.html`** - Interactive map with features

## 🔧 Server Configuration

### `server.js` - Main Express Server
- **Port**: 3000 (configurable via PORT environment variable)
- **Static files**: Served from root directory
- **File uploads**: Handled via Multer, stored in `/uploads`
- **Data storage**: JSON files in `/data` directory
- **API endpoints**: `/api/surplus` for CRUD operations

### Key Features
- Express.js framework
- Multer for file uploads
- Body parser for request handling
- Static file serving
- SPA routing support
- Error handling and logging

## 🌐 Multi-Language Support

The project supports both English and Arabic:
- HTML pages use appropriate language attributes
- CSS includes RTL support for Arabic
- JavaScript handles language switching
- Server responses include Arabic messages

## 📱 Responsive Design

All CSS files include:
- Mobile-first approach
- Breakpoint-based media queries
- Flexible grid layouts
- Touch-friendly interfaces

## 🔒 Security Considerations

- File upload validation (images only, 2MB max)
- Input sanitization
- CORS protection ready
- Environment-based configuration

## 🚀 Development Workflow

1. **Development**: Use `npm run dev` for auto-restart
2. **Production**: Use `npm start` for optimized serving
3. **Testing**: Add test files in appropriate directories
4. **Build**: Minify CSS/JS for production deployment

## 📊 API Structure

### Current Endpoints
- `GET /api/surplus` - Retrieve all surplus items
- `POST /api/surplus` - Create new surplus item

### Planned Endpoints
- User authentication endpoints
- Chat messaging endpoints
- Map data endpoints
- Analytics endpoints

## 🔄 File Naming Conventions

- **CSS**: Use kebab-case (e.g., `donor-dashboard.css`)
- **JavaScript**: Use kebab-case (e.g., `food-surplus.js`)
- **HTML**: Use kebab-case (e.g., `agricultural-waste.html`)
- **Components**: Prefix with purpose (e.g., `navbar.css`)

## 🎯 Best Practices

- Keep CSS modular and component-based
- Use semantic HTML5 elements
- Implement progressive enhancement
- Follow accessibility guidelines
- Optimize images and assets
- Use proper error handling

---

This structure ensures maintainability, scalability, and ease of development for the RecyConnect platform.
