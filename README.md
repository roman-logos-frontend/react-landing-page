# 🛍️ Nice Gadgets Store

**Nice Gadgets Store** is a modern online shop where users can browse, view, and add popular gadgets to their **cart** or **favorites**. The application is built with **React** and supports routing, sliders, product categories, filtering, and persistent state using **localStorage**.
The application uses React Context + useReducer for global state management of Cart and Favorites.

## 🚀 Features

# 🏠 Home Page
- Welcome message for users.
- Interactive banner slider using Swiper with autoplay and custom navigation.
- Brand new models section: filters products released in 2022.
- Hot prices section: displays products sorted by highest discount.
- Shop by category section with links to:
  - Mobile Phones
  - Tablets
  - Accessories

# 📁 Product Page
- Each category page (e.g., /phones, /tablets, /accessories) includes:
  - A list of products with images, names, and prices.
  - Navigation to detailed product pages.
  - Buttons to add items to the cart or favorites.

# 📄 Product Detail Page
- Displays product images, color/capacity selection, full specifications.
- Ability to add the selected configuration to the cart or favorites.

# ❤️ Favorites
- Add/remove products from favorites by clicking the heart icon.
- Favorites persist using localStorage.
- Accessible at /favorites.

# ⭐ FavoritesContext
- Stores a list of favorite products in global state.
- Automatically syncs with localStorage to persist favorites between sessions.
- Actions supported:
  - ADD_ITEM — adds a product to the favorites list (if not already present).
  - REMOVE_ITEM — removes a product from the favorites list.
  - LOAD_FAVORITES — loads favorite items from localStorage on app start.

# 🛒 Cart
- Add/remove items to/from the cart.
- Change product quantity.
- View total cost.
- Cart data is also stored in localStorage.
- Accessible at /cart.

# 🛒 CartContext
- Stores cart items in an array, including quantity per product.
- Syncs with localStorage to persist cart data between sessions.
- Actions supported:
  - ADD_ITEM — adds a new item or increases quantity.
  - REMOVE_ITEM — removes an item from the cart.
  - UPDATE_QUANTITY — updates quantity of a specific item.
  - LOAD_CART — initializes state from localStorage.
  - CLEAR_CART — removes all items.

## 🚀 Live Demo

Experience the live website:
👉 [View Demo](https://roman-logos-frontend.github.io/react-landing-page/)

## 🎨 Design Reference

Figma design:
👉 [View Figma](https://www.figma.com/design/FRxncC4lfyhs6og1L6FGEU/Phone-catalog--V2--Rounded-Style-2?node-id=0-1&p=f&t=usbNvLgsqZPAYWNU-0)

## 🛠 Technologies Used

- **HTML5**
- **SCSS (Sass)** – version `1.72.0`
- **Gulp** – task runner for development
- **Stylelint** – for SCSS linting
- **Swiper** - version `11.2.8`
- **React + TypeScript** - version `18.3.1`
- **React Router DOM** - for routing
- **LocalStorage** - for persistent cart & favorites
- **Context API** - for global state management
