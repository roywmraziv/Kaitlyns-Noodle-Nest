# Kaitlyn's Noodle Nest

Kaitlyn's Noodle Nest is a full-stack web application designed to showcase a family-owned restaurant's menu, booking system, and general information. This project demonstrates a comprehensive use of modern web development technologies and frameworks, making it an excellent portfolio piece for recruiters to evaluate technical skills.

---

## Features

### 1. **Dynamic Web Pages**
   - The website includes multiple pages such as:
     - **Home Page**: Highlights special offers and provides quick links to the menu and booking system.
     - **About Page**: Shares the story behind the restaurant and its founders.
     - **Menu Page**: Displays categorized menu items (Entrees, Sides, Desserts) with dynamic links to individual menu item details.
     - **Booking Page**: Allows users to make reservations with a form submission system.
     - **Menu Item Details Page**: Provides detailed information about a specific menu item, including its description, price, and an image.

### 2. **Responsive Design**
   - The website is fully responsive, ensuring a seamless user experience across devices of all sizes, from desktops to mobile phones.

### 3. **Interactive Booking System**
   - Users can book a table by filling out a form. The data is validated and stored in the database.

### 4. **Admin Panel**
   - A Django-powered admin interface allows the restaurant owners to manage menu items and bookings efficiently.

### 5. **Static and Media File Management**
   - Static files (CSS, JavaScript, images) are served efficiently using Django's `whitenoise` middleware.
   - Media files are managed with a dedicated `MEDIA_URL` configuration.

---

## Technologies Used

### **Backend**
- **Django Framework (v5.1.6)**:
  - A robust Python-based web framework used to build the backend of the application.
  - Features utilized:
    - URL routing with `django.urls`.
    - Models for database schema definition.
    - Forms for handling user input and validation.
    - Django's ORM for database interactions.
    - Admin interface for managing content.

- **SQLite**:
  - A lightweight database used for development and testing purposes.

- **Gunicorn**:
  - A Python WSGI HTTP server used for deploying the application in production.

### **Frontend**
- **HTML5**:
  - Used for structuring the web pages.
- **CSS3**:
  - Custom styles for the website, including responsive design and animations.
  - Fonts integrated via Google Fonts (`Karla` and `Markazi Text`).
- **Django Templating Engine**:
  - Dynamic rendering of HTML templates with context data passed from views.

### **Static File Management**
- **Whitenoise**:
  - Used for serving static files in production with compression and caching.

### **Reverse Proxy**
- **Nginx**:
  - Configured as a reverse proxy to handle requests and serve static files efficiently.
  - Custom configuration files (`reverse-proxy.conf` and `reverseProxyConfig.json`) are included for managing proxy settings.

### **Deployment**
- **DigitalOcean**:
  - The application is hosted on DigitalOcean's App Platform.
- **Procfile**:
  - Used to define the command for running the application in production.

---

## Code Structure

### **Django App: `restaurant`**
- **Models**:
  - `Booking`: Stores reservation details.
  - `Menu`: Stores menu items with attributes like name, price, description, and category.
- **Views**:
  - Handles requests and renders templates for pages like Home, About, Menu, Booking, and individual menu items.
- **Forms**:
  - `BookingForm`: A Django ModelForm for handling reservation submissions.
- **Templates**:
  - Modular templates with a base layout and partials for the header and footer.
  - Pages include `index.html`, `about.html`, `menu.html`, `book.html`, and `menu_item.html`.
- **Static Files**:
  - Custom CSS styles located in `restaurant/static/css/style.css`.
  - Images and other assets are served from the `restaurant/static/img/` directory.

### **Nginx Configuration**
- Reverse proxy configuration files are included to demonstrate advanced deployment techniques.

---

## Highlights for Recruiters

1. **Full-Stack Development**:
   - Demonstrates proficiency in both backend (Django) and frontend (HTML, CSS) development.

2. **Database Management**:
   - Experience with designing and interacting with relational databases using Django's ORM.

3. **Responsive Design**:
   - Ability to create mobile-friendly and visually appealing web pages.

4. **Deployment and Hosting**:
   - Knowledge of deploying web applications using Gunicorn and Nginx on a cloud platform.

5. **Code Organization**:
   - Clean and modular code structure with reusable components and templates.

6. **Static File Optimization**:
   - Efficient handling of static files for production environments.

---

This project is a testament to my ability to design, develop, and deploy a full-stack web application from scratch. It showcases my technical expertise and attention to detail, making it an excellent addition to my portfolio.