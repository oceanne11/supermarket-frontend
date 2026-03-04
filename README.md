Frontend — supermarket-frontend
Project Structure
supermarket-frontend/
├── auth.html      # Login & Register page
├── index.html     # Products manager page
└── README.md

Setup
No installation needed. Just:
•	Make sure the backend is running at http://localhost:5000
•	Open auth.html in your browser
•	Register or login, then you will be redirected to index.html

Pages
auth.html — Login & Register
•	Tab-based layout switching between Login and Register
•	Role selection on register: Customer, Manager, Admin
•	JWT token saved to localStorage on success
•	Auto-redirects to index.html after login
•	Toast notifications for success and error states

index.html — Products Manager
•	Loads all products on page load via GET /api/products
•	Product cards show image, name, category, price, stock, and status badge
•	Category filter buttons and live search
•	Slide-in sidebar form for Add and Edit (Admin/Manager only)
•	Image upload with preview
•	Delete with confirmation modal
•	Toast notifications after every API action
•	Edit/Delete buttons only visible to Admin and Manager

Color Palette 
Name	Hex Code	Usage
Orange	#EC6426	Primary buttons, accents, price text
Green	#2B573A	Navigation bar, sidebar header, badges
Cream	#FDE3CF	Page background, light surfaces
Brown	#632713	Text, delete actions, headings
Light Green	#72AC43	In Stock badge
Yellow	#F8A91F	Category highlights
Pink	#E4A5CA	Category accents

JavaScript Functions
Function	Description
loadProducts()	Fetches all products from API and renders them
createProduct(formData)	POST request to create a new product
updateProduct(id, formData)	PUT request to update an existing product
deleteProduct(id)	DELETE request to remove a product
renderProducts(products)	Renders product cards to the grid
openSidebar()	Opens the add product form sidebar
openEditForm(id)	Opens the edit form pre-filled with product data
filterCategory(cat)	Filters products by category
searchProducts(query)	Live search through loaded products
showToast(msg, type)	Shows success or error notification
initAuth()	Loads user from localStorage and sets up UI
logout()	Clears token and redirects to auth.html


📤 Submission Checklist
Item	Status
Backend pushed to GitHub (supermarket-backend)	✅
Frontend pushed to GitHub (supermarket-frontend)	✅
.env not committed to GitHub	✅
node_modules not committed	✅
postman_collection.json in root	✅
Screenshots in /screenshots folder	✅
README.md in both repos	✅
Figma share link in README	[https://www.figma.com/proto/pOM2FgK2S5HglvZsXTtz4w/Untitled?node-id=0-1&t=euI3zrHCiBUnCtJt-1]

🎨 Figma Design
Figma Share Link: [ https://www.figma.com/proto/pOM2FgK2S5HglvZsXTtz4w/Untitled?node-id=0-1&t=euI3zrHCiBUnCtJt-1 ]

