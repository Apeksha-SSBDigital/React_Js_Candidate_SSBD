# React_Js_Candidate_SSBD
PROJECT DESCRIPTION:
Develop a simple e-commerce application using React.js and API integration, with a focus on core functionalities like displaying products, adding them to a cart, and managing cart items. The application will also use React Router for navigation between pages.
You are free to use any libraries, extensions, or tools that suit your development process.
The final solution should be pushed to a GitHub repository. You need to fork the repository provided in this document, complete the task, and submit your work by 12:00 PM (Noon) on Thursday, 23rd January.

REQUIREMENTS:
1.	Product List Page:
•	Purpose: Display all available products fetched from an external API. 
1.	Product Card: Each product will be displayed as a card containing: 
	Product image.
	Product name.
	Price.
	"Add to Cart" button.
2.	Product Listing: A grid or list layout showcasing multiple product cards.
•	Functionality: 
o	Fetch the list of products from an API.
o	Display the products dynamically based on the fetched data.
o	When the user clicks "Add to Cart," the product is added to the cart, and a notification (e.g., toast or message) confirms the action.

2.	Cart Functionality:
•	Purpose: Enable users to manage their selected items. 
1.	Cart Summary Section: 
	Displays the total number of items in the cart.
	Shows the total price of the items in the cart.
	Updates dynamically as items are added or removed.
2.	Cart Data Management: 
	Use a state management or local state to handle cart data.
•	Functionality: 
o	Clicking "Add to Cart" adds the item to the cart and updates: 
	The quantity of the item (if it’s already in the cart).
	The total price.
o	Real-time updates of the cart summary without refreshing the page.

3.	Cart Page:
•	Purpose: Display detailed information about items in the cart and provide editing options. 
1.	Cart Item List: 
	Each item will display: 
	Product name.
	Price (unit price and total price based on quantity).
	Quantity selector (with "+" and "-" buttons to increase or decrease quantity).
2.	Dynamic Updates: 
	As the quantity of items changes, the total price of the cart updates automatically.
3.	A "Remove" button for each item allows users to remove it from the cart.
•	Functionality: 
o	Validate that the quantity does not drop below 1.
o	Dynamically calculate the total price for each item and the cart total.
4.	API Integration:
•		Purpose: Fetch product data from an external API and use it to populate the product list.
•	Implementation: 
o	Fetch data (e.g., product name, price, image URL) on the Product List page load.
o	Handle loading and error states gracefully (e.g., show a spinner or error message).
•	API Response Example:
API for products list
API - https://fakestoreapi.com/products?limit=30
TYPE- GET
EXPECTED RESPONSE - [
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


5.	Navigation:
•		Purpose: Provide a smooth navigation experience between the Product List page and the Cart page.
•	Implementation: 
o	Use React Router to create two main routes: 
1.	/products for the Product List page.
2.	/cart for the Cart page.
o	Include a navigation bar or links that allow users to switch between these pages.
o	Highlight the active page in the navigation bar.

Expected Application Flow
1.	Home/Product List Page: 
o	User visits the page and sees a list of products.
o	Products are displayed dynamically based on API data.
o	User clicks "Add to Cart," and the item is added to the cart. The cart summary updates in real time.
2.	Cart Page: 
o	User navigates to the Cart page via button.
o	All items in the cart are displayed with their name, price, and quantity.
o	User can adjust quantities or remove items.
o	The total price and item count update dynamically.
3.	Navigation: 
o	Users can switch between the Product List and Cart pages seamlessly.
o	Cart updates persist across navigation.

DELIVERABLES:
1.	Code Structure:
o	A well-structured React project that includes the following:
•	Components: Reusable UI elements to build the interface.
•	Pages: Specific views for routes.
•	Services: Handle API calls and business logic.
•	 Context: Manage global state.
•	 Models: Define common data structures.
•	 Routes: Define navigation paths.
•	 Styles: Scoped or global CSS for consistent design.
•	 Utils: Helper functions for logic.

2.	GitHub Repository:
o	Fork the repository shared in this document.
o	Push your final code to your forked repository.
o	Share the link to your repository with us by 12 PM on Thursday, 23rd January.
o	Repository Link - Github Link

TOOLS & TECHNOLOGIES:
•	React.js: Use React for frontend development with reusable components.
•	Axios: Integrate APIs to fetch product data dynamically.
•	React Router: Enable navigation between Product List and Cart pages.
•	Toast Notifications: Display user-friendly alerts for actions like adding items to the cart.
•	State Management: Use React Context API or local state for managing cart data.
