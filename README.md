# halcon-construction-system
A web application for internal order tracking and management for Halcon Construction Materials Distributor.


# Halcon Construction Materials Distribution System

A full-stack web application to automate the internal order tracking and management processes for Halcon.

## Features

*   **Customer Portal:** Public page to check order status with invoice number.
*   **Admin Dashboard:** Secure dashboard for company personnel.
*   **Role-Based Access Control (RBAC):** Different functionalities for Sales, Purchasing, Warehouse, and Route departments.
*   **Order Lifecycle Management:** Track orders through "Ordered", "In Process", "In Route", and "Delivered" statuses.
*   **Photo Evidence:** Route personnel can upload photos for loading and delivery proof.
*   **Soft Delete & Restoration:** Orders can be archived and restored from a separate list.

## Tech Stack

*   **Backend:** [Node.js with Express] / [Python with Django] / [PHP with Laravel]
*   **Frontend:** [React] / [Vue.js] / [Plain HTML/CSS/JS]
*   **Database:** PostgreSQL
*   **File Storage:** Local storage (can be extended to AWS S3)

## Prerequisites

*   Node.js ^18.0.0 / Python ^3.10
*   PostgreSQL ^13
*   npm / yarn / pip

## Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/halcon-construction-system.git
    cd halcon-construction-system
    ```

2.  **Setup Backend:**
    ```bash
    cd backend
    npm install
    # Create a .env file based on .env.example and configure your database credentials.
    npm run migrate  # To run database migrations
    npm run seed     # To seed the default admin user and roles
    npm run dev      # To start the development server
    ```

3.  **Setup Frontend:**
    ```bash
    cd ../frontend
    npm install
    npm run dev      # To start the Vite/React dev server
    ```
4.  Open `http://localhost:3000` to view the admin app and `http://localhost:3000/track` for the public tracking page.

## Database Schema

See the ER Diagram in the `/docs` directory for a detailed view of the database structure.

## Testing

```bash
# Run backend tests
cd backend && npm test

# Run frontend tests
cd frontend && npm test
