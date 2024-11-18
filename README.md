# 🛒 Commerce - Online Auction Platform  

**Commerce** is a dynamic web application for online auctions, allowing users to list items, place bids, leave comments, and manage watchlists. Built with Django, this platform integrates robust back-end functionality with a clean front-end design, providing a seamless auction experience.  

---

## 🔍 What Does This Project Do?  

This platform enables users to:  
- **Create Auction Listings**: Post items for bidding with a title, description, image, and starting bid. 📤  
- **Bid on Listings**: Place competitive bids and track the highest bid in real-time. 💰  
- **Comment on Listings**: Engage in discussions by leaving comments on auction pages. 💬  
- **Manage Watchlists**: Save items of interest to a personal watchlist for easy access. 👀  
- **Close Listings**: End auctions and determine the highest bidder as the winner. ✅  

---

## 🛠️ Technologies Used  

### 1. **Django Framework**  
- **Model-View-Template (MVT) Architecture**: Ensures a clean separation of logic, data, and presentation.  
- **ORM (Object-Relational Mapping)**: Simplifies database interactions for managing users, listings, bids, and comments.  

### 2. **Bootstrap**  
- Enhances the front-end with a responsive, modern design.  
- Provides reusable components for forms, navigation bars, and modals.  

### 3. **SQLite**  
- Lightweight database for storing user data, auction listings, bids, and comments.  

### 4. **HTML, CSS, JavaScript**  
- **HTML**: Defines the structure of web pages.  
- **CSS**: Styles pages for an intuitive user experience.  
- **JavaScript**: Adds interactivity, such as dynamic updates and form validation.  

---

## 🔧 How It Works  

### 1. Auction Listings  
- Users create auction listings with the following attributes:  
  - Title, description, and starting bid.  
  - Optional image URL for visual representation.  
  - Category for better organization.  

### 2. Bidding System  
- Listings display the current highest bid and allow users to place new bids.  
- Bid validation ensures new bids are higher than the current maximum.  

### 3. Watchlist  
- Users can add or remove items from their watchlist.  
- Watchlist items are stored per user and accessible via a dedicated page.  

### 4. Comments  
- Users can post comments on active listings.  
- Comments are displayed in chronological order below the listing details.  

### 5. Closing Auctions  
- Listing creators can close auctions at any time.  
- When closed, the highest bidder is marked as the winner, and no further bids are accepted.  

---

## 📊 Database Models  

### 1. **User**  
- Stores user authentication details using Django's built-in User model.  

### 2. **Listing**  
- Fields: `title`, `description`, `starting_bid`, `current_price`, `image_url`, `category`, `is_active`, `creator`.  
- Relationships: Connected to `User` as the creator and bidders via bids.  

### 3. **Bid**  
- Fields: `amount`, `bidder`, `listing`.  
- Tracks all bids placed on each listing.  

### 4. **Comment**  
- Fields: `content`, `commenter`, `listing`.  
- Stores user-generated comments for each listing.  

### 5. **Watchlist**  
- Many-to-Many relationship between users and listings.  
- Tracks items users have saved to their watchlists.  

---

## 🎯 Applications  

This project showcases:  
- **E-Commerce Development**: Demonstrates how to build a scalable auction platform.  
- **Full-Stack Development**: Combines Django back-end with front-end technologies like Bootstrap and JavaScript.  
- **User Interactivity**: Implements features like bidding, commenting, and watchlist management for an engaging experience.  

---

## 🌟 Why Use This Project?  

- **Scalability**: Easily extendable to add new features, such as email notifications or payment integration.  
- **Educational**: Learn how to implement core e-commerce functionalities using Django.  
- **Practical**: Adapt the platform for other use cases, like marketplace apps or classified listings.  

---  

Feel free to explore and customize this project to suit your needs. Happy coding! 🚀  
