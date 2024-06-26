# Fast React Pizza

Welcome to the Fast React Pizza project! This is a web application for ordering pizza, built using React, Redux, and various other modern web technologies. The app allows users to browse a menu, add items to a cart, place orders, and track the status of their orders.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
  - [Components](#components)
  - [Redux](#redux)
  - [Services](#services)
  - [Utilities](#utilities)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)

## Project Overview

Fast React Pizza is a mock pizza delivery application that allows users to:

- Browse a menu of available pizzas.
- Add pizzas to their cart.
- Place an order with their selected pizzas.
- View and update their order status.

## Features

- **User Authentication**: Users can enter their name to start ordering.
- **Menu Browsing**: View a list of available pizzas.
- **Order Management**: Add pizzas to the cart and place an order.
- **Order Tracking**: View order status and estimated delivery time.
- **Priority Ordering**: Users can mark their orders as a priority.

## Tech Stack

- **Frontend**: React, React Router, Redux, Tailwind CSS
- **Backend**: Mocked with a static API
- **State Management**: Redux Toolkit
- **Utilities**: Geolocation API for fetching user location

## Technologies Used

### Frontend

- **[React](https://reactjs.org/)**: A JavaScript library for building user interfaces.
- **[React Router](https://reactrouter.com/)**: A standard library for routing in React applications.
- **[Redux](https://redux.js.org/)**: A predictable state container for JavaScript apps.
- **[Redux Toolkit](https://redux-toolkit.js.org/)**: The official, recommended way to write Redux logic.
- **[Tailwind CSS](https://tailwindcss.com/)**: A utility-first CSS framework for rapidly building custom designs.

### Development Tools

- **[Vite](https://vitejs.dev/)**: A fast build tool and development server.
- **[ESLint](https://eslint.org/)**: A tool for identifying and fixing linting errors in JavaScript code.
- **[Prettier](https://prettier.io/)**: A code formatter to ensure consistent code style.

### APIs and Libraries

- **[Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API)**: For fetching the user's location.
- **Mock API**: For simulating backend endpoints.

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (version 14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/osama206/fast-react-pizza.git
   cd fast-react-pizza
   ```

2. Install dependencies:
   ```sh
   npm install
   # or
   yarn install
   ```

### Running the Application

To start the development server, run:
```sh
npm run dev
# or
yarn dev
```

The application will be available at `http://localhost:5173`.

## Project Structure

Here's an overview of the project structure:

### Components

- **Header**: Application header with navigation.
- **Loader**: Loading spinner.
- **Button**: Reusable button component.
- **LinkButton**: Button that navigates to different routes.
- **CreateUser**: Form for entering the username.
- **Username**: Displays the current username.
- **Order**: Detailed order view.
- **OrderItem**: Displays individual items in an order.
- **SearchOrder**: Form to search for an order by ID.
- **UpdateOrder**: Form to update the order priority.
- **CartOverview**: Displays a summary of the items in the cart.

### Redux

- **userSlice**: Manages user-related state, including username and address.
- **cartSlice**: Manages the shopping cart state.
- **store.js**: Configures the Redux store.

### Services

- **apiRestaurant**: Functions for interacting with the restaurant's API.
- **apiGeocoding**: Functions for fetching user addresses based on geolocation.

### Utilities

- **helpers.js**: Utility functions for formatting currency, dates, and calculating delivery times.

## API Endpoints

The following API endpoints are used in the project (note: these are mocked for the purpose of this project):

- **Menu**: `GET /menu`
- **Order**: `GET /order/:id`
- **Create Order**: `POST /order`
- **Update Order**: `PATCH /order/:id`

## Contributing

We welcome contributions! If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some amazing feature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

---
