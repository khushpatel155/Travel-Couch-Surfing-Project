### README for Travel & Couch Surfing Project

---

# **Couch Surfing & Room Renting Platform**

This project is a full-stack MERN (MongoDB, Express, React, Node.js) web application inspired by platforms like CouchSurfing. It enables users to host travelers by offering rooms for free or at minimal cost. It includes a wide array of features and is designed to be scalable, secure, and user-friendly.

---

## **Features**

### **User Features**
1. **Room Listings**  
   - Users can add rooms with detailed descriptions, images, and pricing.
   - Rooms appear as cards or on an interactive map with geolocation.

2. **Interactive Map**  
   - Rooms displayed on a map using MapBox with geolocate control.
   - Reverse geocoding to convert coordinates to readable addresses.

3. **Image Upload**  
   - Drag-and-drop image upload with Firebase integration.
   - Carousel-style image sliders for room galleries.

4. **Search & Filter**  
   - Search rooms by city or address.
   - Filter rooms by price range or other criteria.

5. **Authentication**  
   - Google One Tap Login integration.
   - Custom authentication using JWT tokens with local storage session management.

6. **Profile Management**  
   - Upload avatar pictures and update user information.

7. **Real-Time Validation**  
   - Validate user inputs for room details like title, price, and description.

---

### **Admin Features**
1. **Admin Dashboard Panel**  
   - Role-based access control (RBAC) with admin, editor, and normal user roles.
   - Admins can manage users, rooms, and access privileges.
   - Editors can manage rooms but not users.

2. **Data Management**  
   - Manage users via an interactive DataGrid (sorting, editing, filtering).
   - View, update, delete rooms, and remove associated Firebase images.

3. **Statistics & Charts**  
   - Pie chart for room price categories.
   - Area chart comparing user registrations and room listings over time.

4. **Access Control**  
   - Restricted access to admin panel and dashboard.
   - Unauthorized users receive "Forbidden Access" messages.

---

### **Technical Highlights**
1. **Frontend**
   - **React.js**: For creating a responsive and interactive UI.
   - **Material UI (MUI5)**: Modern components for design and styling.
   - **MapBox**: Interactive maps with clustering for room locations.

2. **Backend**
   - **Node.js** & **Express.js**: API development and middleware integration.
   - **MongoDB** & **Mongoose**: Storing and managing user and room data.

3. **Security**
   - JWT-based authentication and role validation.
   - Session expiration management for token-based access control.

4. **File Storage**
   - Firebase for storing and managing user-uploaded images.

5. **Deployment**
   - Frontend hosted on Netlify.
   - Backend hosted on Render (free alternative to Heroku).

---

### **Special Features**
- **Role-Based Access Control (RBAC):**  
   Secure and granular control of system resources based on user roles.
   - **Admin:** Full access to manage users, rooms, and privileges.
   - **Editor:** Limited access to manage rooms.
   - **Normal User:** Can only manage their own data.

- **Real-Time Validation:**  
   Client-side and server-side checks to ensure data integrity.

- **Interactive Map Features:**  
   Geolocation, clustering, and reverse geocoding for precise room location management.

---

## **How to Run the Project**
1. Clone the repository.
2. Install dependencies:
   ```bash
   npm install
   cd client && npm install
   cd ..
   ```
3. Set up environment variables :

# Server Configuration
PORT=5000  # The port on which the server will run

# Database Configuration
MONGO_CONNECT=your_mongodb_connection_string  # Replace with your MongoDB connection URI

# Client Configuration
CLIENT_URL=http://localhost:3000  # URL of the frontend client application

4. Start the backend and frontend servers:
   ```bash
   npm run server
   cd client && npm start
   ```
5. Access the application at `http://localhost:3000`.

---

## **Technologies Used**
- **Frontend:** React.js, Material UI (MUI5), MapBox, Firebase
- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Authentication:** JWT, Google One Tap Login
- **Charts:** reCharts, DataGrid (MUI)
- **Hosting:** Render, Netlify

---

This project offers significant potential for real-world applications, including:
- CouchSurfing platforms
- Real estate and room rental marketplaces
- Location-based services and apps

---

Feel free to explore and contribute!#
