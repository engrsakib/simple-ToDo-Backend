# BloodBridge

A comprehensive platform designed for community welfare and fundraising, enabling users to create, manage, and participate in donation campaigns. This project also facilitates lost and found item management, allowing users to post, browse, and recover lost belongings effectively.

## Features for Your Project  

### 🌟 Core Functionalities:
- **User Role Management**:
  - **Admin 🌐**: Full control of the platform, including user management, donation requests, funding, and content publishing.
  - **Donor 🩸**: Ability to register, view donation requests, respond to requests, and manage their own profiles.
  - **Volunteer 🤝**: Permission to create and manage donation requests. Volunteers can update the status of blood donation requests.
  - 💡 *Admins can assign roles (e.g., Volunteer, Admin) or block users directly from the database.*

### 🔒 User Authentication:
- **Registration**:
  - Users can register with their email, name, avatar (via imageBB), blood group, district, upazila, and password. By default, every registered user becomes a "Donor."
  - **Default User Status**: Active.
  - Admins can block/unblock users, which updates their status accordingly.
- **Login**: Secure login with email and password. Social login is not required.
  
### 🔑 Private Dashboard:
- **Profile Management**:
  - Users can view and edit their profile data, except for their email, which remains static.
  - Admins can manage all users, while donors and volunteers manage only their own data.

#### Donor-Specific Features:
- **Recent Donation Requests**: Donors can view their top three recent requests on the dashboard homepage.
- **Full Donation History**: Paginated view of all donation requests with filtering options (`pending`, `in-progress`, `done`, `canceled`).
- **Create Requests**: Donors can submit detailed blood donation requests, including recipient details, location, and donation dates.  
  *Note: Only active donors can create requests.*

#### Admin-Specific Features:
- **Dashboard Statistics**:
  - View total users, total funding, and total donation requests in real-time.
- **User Management**:
  - Block/unblock users, assign roles, and manage user statuses through a detailed table with pagination and filters.
- **Global Request Management**:
  - Manage all blood donation requests, edit statuses, and delete requests.
- **Content Management**:
  - Publish/unpublish blogs, edit and delete content, or add new blogs through a rich text editor.

#### Volunteer-Specific Features:
- **Request Management**:
  - Volunteers can only update the statuses of donation requests (e.g., from "pending" to "in-progress").
- **Content Contribution**:
  - Volunteers can add blogs but cannot publish or delete content.

### 🌐 Public Pages:
- **Home Page**:
  - Includes registration, donor search, contact information, and a responsive footer.
- **Search Donors**:
  - Users can filter donors by blood group, district, and upazila.
- **Donation Requests**:
  - Public view of all pending donation requests, with options to view more details after logging in.
- **Blogs**:
  - Published blogs are accessible publicly, with detailed views for each blog.

### 💳 Payment Integration:
- **Funding Page**:
  - Users can make financial contributions via Stripe integration.
  - Displays total funds and detailed records of donations (e.g., donor name, amount, and date).

### 📅 Additional Features:
- **Pagination**:
  - Implemented across all tables and lists (e.g., user management, donation requests, and funding records).
- **Sorting & Filtering**:
  - Sorting by date, status, or categories to ensure streamlined navigation.
- **JWT Protection**:
  - Secure private APIs and routes using JSON Web Tokens (JWT), stored in the browser’s local storage.

### 🎨 User Experience:
- Fully responsive design for mobile, tablet, and desktop devices.  
- Rich text editing for blog content using **Jodit-react**.  

### 🚀 Challenges Addressed:
- Integration of funding features, JWT authentication, paginated tables, and volunteer/admin-specific permissions ensures scalability and ease of management.






### API Endpoints

#### User Management
1. **Add User**
   - **Method:** `POST /users`
   - **Functionality:** Adds a new user to the database.
   - **Input:** User data (name, email, photo, etc.).

2. **Fetch User by Email**
   - **Method:** `GET /users/:mail`
   - **Functionality:** Fetches user details by email.

#### Lost & Found Campaigns
1. **Create Lost/Found Item Post**
   - **Method:** `POST /items`
   - **Functionality:** Adds a new lost or found item post to the database.

2. **Fetch All Posts**
   - **Method:** `GET /items`
   - **Functionality:** Retrieves all lost and found item posts.

3. **Fetch Post Details**
   - **Method:** `GET /items/:id`
   - **Functionality:** Fetches detailed information about a specific lost or found item post using its ID.

4. **Update Post**
   - **Method:** `PUT /items/:id`
   - **Functionality:** Updates an existing lost or found item post by its ID.

5. **Delete Post**
   - **Method:** `DELETE /items/:id`
   - **Functionality:** Deletes a specific lost or found item post by ID.

#### Recovered Items Management
1. **Mark as Recovered**
   - **Method:** `POST /recovered`
   - **Functionality:** Marks a lost or found item as recovered and stores recovery details (location, date, recovered by).

2. **Fetch All Recovered Items**
   - **Method:** `GET /recovered`
   - **Functionality:** Retrieves all recovered items with relevant details.

### Deployment Guidelines
- Ensure Firebase and MongoDB configurations are secured using environment variables.
- Fully responsive design optimized for mobile, tablet, and desktop.
- Avoid CORS/404/504 errors on production.

## Live Site
[Visit BloodBridge](https://engrsakib-blood-donations-project.netlify.app/)

## GitHub Repositories
- **Server Repository:** [server-side-engrsakib](https://github.com/engrsakib/blood-donor-simple-project-server)
- **Client Repository:** [client-side-engrsakib](https://github.com/engrsakib/blood-donor-simple-project-client-side)

## How to Run the Server
1. Clone the repository:
   ```bash
   git clone https://github.com/engrsakib/blood-donor-simple-project-server
   
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   nodemon index.js
   ```

## How to Run the Client
1. Clone the repository:
   ```bash
   git clone https://github.com/engrsakib/sakib-welfare-champine-client-side.git
   cd sakib-welfare-champine-client-side
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the client:
   ```bash
   npm start
   ```

## Contribution
Contributions are welcome! Feel free to submit issues or pull requests to improve the platform.

