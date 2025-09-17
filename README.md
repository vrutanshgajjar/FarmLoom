FarmLoom

FarmLoom is a web platform designed for wholesale crop trading, connecting farmers and consumers seamlessly. The project is still under development but aims to provide a reliable marketplace with rich features for both sellers and buyers.

Architecture

(Add your architecture diagram here when available)

Features

Dual Interfaces: FarmLoom provides separate interfaces for consumers and farmers, with authentication (SignUp/SignIn) and email verification.

Farmer Side

Sales Analytics: Integrated charts and graphs to help farmers track their sales performance.

Product Management: Farmers can add, edit, and delete crops with details such as images, stock, location (map-based), and minimum order quantity.

Order Dashboard: A centralized dashboard where farmers can manage incoming orders and view customer locations on a map.

FAQ Section: Farmers can answer common questions, which are displayed publicly for consumers.

Consumer Side

Simple Browsing Experience: Consumers can explore categories and products easily from the homepage.

Product Dashboard: Detailed product pages include stock availability, pricing, and order restrictions.

Reviews & Ratings: Consumers can leave feedback on products, ensuring transparency.

Direct Contact Form: A built-in form allows consumers to send inquiries directly to farmers. Resolved queries appear in the FAQ section.

Cart & Checkout: Consumers can add products to their cart, manage quantities, and securely place orders.

Real-Time Updates (WebSocket): Planned feature for live stock updates without refreshing the page (works in local environment, not on free hosting like Vercel).

Technologies Used

MongoDB

NodeJS

ExpressJS

ReactJS

Redux

CSS (or Tailwind, if you plan to add it later)

WebSocket (socket.io)

Cloudinary (for image storage)

Leaflet (map integration)

Recharts (data visualization)

Installation

To run FarmLoom locally, ensure you have NodeJS and MongoDB installed.

Clone the repository

git clone <repository-url>
cd FarmLoom


Frontend Setup

Navigate to the client folder.

Create a .env file in client root with:

VITE_FARMLOOM_API = "http://localhost:8080/"


Run the frontend:

cd client
npm install
npm run dev


Backend Setup

Navigate to the server folder.

Create a .env file in server root with:

MONGO_DB_URL = {your mongodb url}
JWT_SECRET = {jwt secret}
CLOUDINARY_CLOUD_NAME = {cloudinary cloud name}
CLOUDINARY_API_KEY = {cloudinary api key}
CLOUDINARY_API_SECRET = {cloudinary api secret}


Run the backend:

cd server
npm install
nodemon

Contribution

FarmLoom is open to contributions. Feel free to fork the repository, raise issues, or submit pull requests to help improve the platform.
