# 🌍 TravelBandhu

TravelBandhu is a full-stack travel and accommodation web application that allows users to explore travel destinations, discover property listings, create and manage their own listings, and share reviews.

The project is designed to provide a simple and user-friendly platform for travelers to find suitable stays and share their experiences.

## ✨ Features

* 🏠 Browse and explore property listings
* 🔍 View detailed information about listings
* ➕ Create new property listings
* ✏️ Edit your own listings
* 🗑️ Delete your own listings
* ⭐ Add reviews to listings
* 🗑️ Delete reviews
* 🔐 User authentication and authorization
* 👤 Listing ownership and authorization
* 🖼️ Image upload and cloud storage
* 🔔 Flash messages for user feedback
* 📱 Responsive user interface
* 🗺️ Location-based property information

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap
* EJS
* EJS-Mate

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### Authentication & Security

* Passport.js
* Passport-Local
* Express Session
* Connect-Mongo
* Connect-Flash

### Image Management

* Cloudinary
* Multer
* Multer-Storage-Cloudinary

### Other Tools

* Method-Override
* Dotenv
* Nodemon

## 📂 Project Structure

```text
TravelBandhu/
│
├── controllers/
│
├── models/
│
├── routes/
│
├── views/
│   ├── includes/
│   ├── layouts/
│   ├── listings/
│   ├── users/
│   └── reviews/
│
├── public/
│   ├── css/
│   └── js/
│
├── utils/
│
├── app.js
├── middleware.js
├── schema.js
├── package.json
├── package-lock.json
└── README.md
```

## 🚀 Getting Started

Follow these steps to run TravelBandhu locally.

### 1. Clone the Repository

```bash
git clone https://github.com/dhiruuuu7766/TravelBandhu.git
```

### 2. Navigate to the Project

```bash
cd TravelBandhu
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory:

```env
ATLASDB_URL=your_mongodb_connection_string
SECRET=your_session_secret

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET=your_cloudinary_api_secret
```

> ⚠️ Never commit your `.env` file to GitHub. Keep your database and Cloudinary credentials private.

### 5. Start the Application

Using Node.js:

```bash
node app.js
```

Or using Nodemon during development:

```bash
nodemon app.js
```

The application will be available at:

```text
http://localhost:3000
```

## 🔐 Authentication

TravelBandhu uses **Passport.js** for user authentication.

Users can:

* Register an account
* Log in and log out
* Create property listings
* Edit their own listings
* Delete their own listings
* Add reviews
* Manage their reviews

Authorization middleware ensures that users can only modify resources they are authorized to manage.

## 🏠 Listings

Users can create property listings with information such as:

* Title
* Description
* Location
* Country
* Price
* Image

Users can also edit or delete listings they own.

## 🖼️ Image Upload

TravelBandhu uses **Cloudinary** for image storage.

The image upload workflow uses:

```text
User
  ↓
Multer
  ↓
Cloudinary
  ↓
Image URL
  ↓
MongoDB
```

Listing image information is stored along with the listing data in MongoDB.

## ⭐ Reviews

Authenticated users can add reviews to property listings.

Each review contains:

* Rating
* Comment
* User reference
* Listing reference

Users can also delete reviews according to the application's authorization rules.

## 🗄️ Database

TravelBandhu uses **MongoDB** with **Mongoose** for database management.

Main data models include:

* User
* Listing
* Review

Relationships between users, listings, and reviews are managed using MongoDB references.

## 🔒 Security

The project includes several security practices:

* Authentication using Passport.js
* Authorization middleware
* Session-based authentication
* Environment variables for sensitive credentials
* Protected routes
* User ownership validation

## 📸 Screenshots

Add project screenshots here to showcase the application.

```text
Coming Soon
```

## 🔮 Future Improvements

Some planned improvements include:

* 🗺️ Interactive maps
* 🔎 Advanced search and filtering
* ❤️ Wishlist functionality
* 📅 Property booking system
* 💳 Online payment integration
* 📧 Email notifications
* ⭐ Improved rating system
* 📱 Enhanced mobile experience
* ☁️ Production deployment

## 🎯 Learning Outcomes

Through this project, I practiced and improved my understanding of:

* RESTful API development
* Express.js
* MongoDB and Mongoose
* Authentication and authorization
* MVC architecture
* CRUD operations
* Middleware
* Session management
* Image upload and cloud storage
* EJS templating
* Database relationships
* Git and GitHub

## 👨‍💻 Author

### Dhiraj Kumar Ram

**B.Tech CSE Student | Full Stack / MERN Developer**

* GitHub: https://github.com/dhiruuuu7766
* LinkedIn: https://linkedin.com/in/dhiraj-kumarr

## 📄 License

This project was developed for learning and portfolio purposes.

---

⭐ If you found this project useful, consider giving it a star!
