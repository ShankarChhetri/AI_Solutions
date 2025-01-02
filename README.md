
# AI Management System

## Overview
This project is a web-based application built with Node.js, Express, MongoDB, and EJS. It features an admin panel, a gallery, resource management, user authentication, and site settings controls. The system is designed to manage solutions, feedbacks, resources, and other functionalities in an AI-related context.

---

## Features
1. **Admin Dashboard**
   - View analytics, manage feedbacks, events, and resources.
   - Change password and manage profile.
   
2. **Gallery Management**
   - Add, update, and delete photos for events.
   - Event booking and timeline updates.

3. **Feedback Management**
   - Approve, delete, and manage user feedback.

4. **Resource Management**
   - Add, update, and delete resources.
   - View and manage portfolio items.

5. **Site Settings**
   - Update logo, timezone, and global site configurations.

6. **Authentication**
   - Admin login, logout, and session-based authentication.

7. **Contact Management**
   - Manage contact form submissions and update user details.

8. **Error Handling**
   - Global error handling for server and application errors.

---

## Requirements
- Node.js
- MongoDB
- dotenv
- express
- mongoose
- bcrypt
- multer
- body-parser
- connect-mongo
- ejs

---

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd <project-folder>
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Create a `.env` file in the root directory and add the following:
   ```
   PORT=3000
   MONGO_URI=mongodb://localhost:27017/AI
   SESSION_SECRET=yourSecretKey
   ```
5. Start the application:
   ```bash
   npm start
   ```
6. Visit `http://localhost:3000` to access the application.

---

## Usage
### Admin Panel
1. Access the admin panel via `/admin/login`.
2. Use the credentials set in the Admin model to log in.
3. Manage dashboard functionalities like events, feedbacks, and resources.

### Feedback and Testimonials
- Users can submit feedback via the home page.
- Admin can approve or delete feedback from the dashboard.

### Resource Management
- Add or delete resources via the admin panel.

---

## Directory Structure
```
├── models/
│   ├── Admin.js
│   ├── Gallery.js
│   ├── Feedback.js
│   ├── Solution.js
│   ├── Resource.js
│   ├── SiteSettings.js
│   ├── Contact.js
├── routes/
│   ├── admin.js
│   ├── feedback.js
│   ├── resources.js
│   ├── chatbot.js
├── views/
│   ├── admin/
│   │   ├── dashboard.ejs
│   │   ├── login.ejs
│   │   ├── change-password.ejs
│   │   ├── site-controls.ejs
│   │   ├── manage-photos.ejs
│   │   ├── manage-resources.ejs
│   │   ├── manage-portfolio.ejs
│   │   ├── manage-contacts.ejs
│   ├── home.ejs
│   ├── contact.ejs
│   ├── solutions.ejs
│   ├── feedbacks.ejs
├── public/
│   ├── images/
│   │   ├── gallery/
│   │   ├── portfolio/
│   │   ├── logo.png
├── app.js
├── package.json
├── .env
```

---

## Troubleshooting
- Ensure MongoDB is running locally on the specified port.
- Check the `.env` file for correct configurations.
- Use `npm install` to ensure all dependencies are installed.

---

## License
This project is open-source and available for modification and use under the MIT License.
