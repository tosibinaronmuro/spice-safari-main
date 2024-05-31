## Spice Safari main App - Frontend Documentation

This documentation outlines the functionalities and components of the Spice Safari mobile app, built using Next.js 13.

**Technologies Used:**

* Next.js 13 (Frontend Framework)
* React (JavaScript Library for Building User Interfaces)
* Redux Toolkit (State Management Library)
* Tailwind CSS (Utility-First CSS Framework)
* React Toastify (Library for Notifications)

**Project Setup:**

1. **Prerequisites:**
    * Node.js and npm (or yarn) installed on your machine.

2. **Cloning the Repository (if applicable):**
    ```bash
    git clone https://github.com/your-username/spice-safari-app.git
    ```

3. **Installing Dependencies:**
    ```bash
    cd spice-safari-app
    npm install
    ```

4. **Running the Development Server:**
    ```bash
    npm run dev
    ```

    This will start the development server and make the application accessible on your mobile device using a QR code or a local URL depending on your development environment.

**User Interface (UI) Components:**

* **Home:** Displays featured products, categories, and potential promotional offers.
* **Products:** Lists all available products with filtering and sorting options. Users can view product details and add items to their cart.
* **Search:** Allows users to search for products by name or category.
* **Cart:** Shows the list of items added to the cart, with options to edit quantities or remove items. Users can proceed to checkout from here.
* **Checkout:** Guides users through the checkout process, including selecting a delivery address and payment method.
* **Account:** Provides access to user-specific functionalities (requires login):
    * Profile Management: Edit user details (name, email, etc.).
    * Order History: View past orders and their details.
    * Favorites (Wishlist): View and manage favorite products.
    * Logout: Option to log out of the account.

**Data Fetching and State Management:**

* Data fetching is implemented using Next.js data fetching methods (getServerSideProps, getStaticProps, etc.) or external libraries like Axios.
* Redux Toolkit is assumed to be used for managing application state across components.

**Authentication and Authorization:**

* Login and registration functionalities are implemented for user authentication.
* User authentication is required to access account-specific features like favorites, orders, and profile management.
* Authorization logic would determine which functionalities a user can access based on their login status.

**Notifications:**

* React Toastify is used to display notifications to users for actions like adding items to cart, successful orders, etc.

**Styling:**

* Tailwind CSS provides utility classes for building responsive layouts and UI components.
* Additional custom styles might be defined in CSS files for specific design elements.

**Future Considerations:**

* Implement unit tests for critical components using a testing framework like Jest.
* Integrate offline functionality for browsing products or managing wishlist items (if applicable).
* Implement push notifications for order updates or promotions (if applicable).
