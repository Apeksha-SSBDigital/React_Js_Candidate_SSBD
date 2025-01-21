Project Description
Objective:  
Develop a simple e-commerce application using React.js and API integration, focusing on core functionalities such as displaying products, adding them to a cart, and managing cart items. The application will utilize React Router for navigation between pages.

You may use any libraries, extensions, or tools that suit your development process.  
The final solution must be pushed to a GitHub repository by 12:00 PM (Noon) on Thursday, 23rd January.

 Requirements

 1. Product List Page
- Purpose: Display all available products fetched from an external API.
- Key Features:
  1. Product Card: Each product must include:
     - Product image.
     - Product name.
     - Price.
     - "Add to Cart" button.
  2. Product Listing:
     - Showcase multiple product cards in a grid or list layout.
- Functionality:
  - Fetch the product list from the provided API dynamically.
  - Display the fetched products on the page.
  - Clicking "Add to Cart" should:
    - Add the product to the cart.
    - Display a confirmation notification (e.g., toast).

 2. Cart Functionality
- Purpose: Enable users to manage selected items.
- Key Features:
  1. Cart Summary Section:
     - Display the total number of items in the cart.
     - Show the total price of all cart items.
     - Update dynamically as items are added or removed.
  2. Cart Data Management:
     - Use React Context API or local state for handling cart data.
- Functionality:
  - Clicking "Add to Cart" should:
    - Update the quantity of the product in the cart (if already added).
    - Recalculate the total price dynamically.
  - Provide real-time updates without page refresh.

 3. Cart Page
- Purpose: Display detailed information about items in the cart and provide editing options.
- Key Features:
  1. Cart Item List:
     - Each cart item must display:
       - Product name.
       - Price (unit price and total price based on quantity).
       - Quantity selector (with "+" and "-" buttons to adjust quantity).
  2. Dynamic Updates:
     - Adjust the total price dynamically as the quantity changes.
  3. Remove Button:
     - Allow users to remove items from the cart.
- Functionality:
  - Validate that quantity does not drop below 1.
  - Dynamically calculate the total price for individual items and the overall cart.

 4. API Integration
- Purpose: Fetch product data from an external API and use it to populate the product list.
- Implementation:
  - Fetch product data from:  
    API: `https://fakestoreapi.com/products?limit=30`  
    Method: `GET`
  - Handle loading and error states gracefully (e.g., show a spinner or error message).

Expected API Response:
json
[
  {
    "id": 1,
    "title": "Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",
    "price": 109.95,
    "description": "Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday",
    "category": "men's clothing",
    "image": "https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg",
    "rating": {
      "rate": 3.9,
      "count": 120
    }
  }
]

 5. Navigation
- Purpose: Provide seamless navigation between the Product List and Cart pages.
- Implementation:
  - Use React Router to create two main routes:
    1. `/products` for the Product List page.
    2. `/cart` for the Cart page.
  - Include a navigation bar or links for switching between pages.
  - Highlight the active page in the navigation bar for better user experience.

 Expected Application Flow
1. Home/Product List Page:
   - Display a list of products dynamically fetched from the API.
   - Clicking "Add to Cart" adds the product to the cart and updates the cart summary in real time.
2. Cart Page:
   - Display all cart items with their name, price, and quantity.
   - Allow users to adjust quantities or remove items.
   - Update the total price and item count dynamically.
3. Navigation:
   - Users can switch between the Product List and Cart pages seamlessly.
   - Cart updates persist across navigation.

 Deliverables

 1. Code Structure
- A well-organized React project, including:
  - Components: Reusable UI elements for building the interface.
  - Pages: Specific views for each route.
  - Services: Handle API calls and business logic.
  - Context: Manage global state efficiently.
  - Models: Define common data structures.
  - Routes: Define navigation paths using React Router.
  - Styles: Use scoped or global CSS for consistent design.
  - Utils: Include helper functions for reusable logic.

 2. GitHub Repository
- Fork the provided repository and push the final code to your forked repository.
- Ensure meaningful commit messages reflecting development progress.
- Share the repository link by 12:00 PM (Noon) on Thursday, 23rd January.

 Tools & Technologies
- React.js: Frontend development framework with reusable components.
- Axios: For integrating APIs and fetching product data dynamically.
- React Router: To enable smooth navigation between pages.
- Toast Notifications: For user-friendly alerts (e.g., adding items to the cart).
- State Management: React Context API or local state for managing cart data.
