# crypto-portfolio-management
This web tool for synthesizing and visualizing realtime cryptocurrency trends

## Project structure
- **Project folder structure**: Reflects the logical components of your project, including the frontend, the backend, the tests, the assets.

  ```
  crypto-tracker/
  ├── frontend/             # contains the frontend code and assets
  │   ├── src/              # contains the source code for the frontend
  │   │   ├── components/   # contains the reusable UI components
  │   │   ├── pages/        # contains the main pages of the app
  │   │   ├── utils/        # contains the helper functions and constants
  │   │   └── index.js      # the entry point of the frontend app
  │   ├── public/           # contains the static files for the frontend
  │   │   ├── images/       # contains the images for the app
  │   │   ├── styles/       # contains the CSS files for the app
  │   │   └── index.html    # the HTML file for the app
  │   └── package.json      # contains the dependencies and scripts for the frontend
  ├── backend/              # contains the backend code and assets
  │   ├── src/              # contains the source code for the backend
  │   │   ├── controllers/  # contains the functions that handle the API requests
  │   │   ├── models/       # contains the schemas and models for the database
  │   │   ├── services/     # contains the functions that interact with external APIs
  │   │   ├── routes/       # contains the routes for the API endpoints
  │   │   ├── config/       # contains the configuration files for the backend
  │   │   └── index.js      # the entry point of the backend app
  │   ├── tests/            # contains the tests for the backend
  │   └── package.json      # contains the dependencies and scripts for the backend
  └── README.md             # contains the documentation and instructions for the project
  ```

- **Separate business logic and API routes**: Separate the business logic and the API routes in the backend code, so that code is modular, testable, and reusable. The business logic is the code that implements the core functionality of your app, such as fetching, storing, and analyzing the cryptocurrency data. The API routes are the code that defines the endpoints that the frontend can call to access the data. 
- 
  ```
  backend/
  ├── src/
  │   ├── controllers/      # contains the functions that handle the API requests
  │   │   ├── crypto.js     # contains the functions for the crypto-related endpoints
  │   │   └── user.js       # contains the functions for the user-related endpoints
  │   ├── models/           # contains the schemas and models for the database
  │   │   ├── crypto.js     # contains the schema and model for the crypto collection
  │   │   └── user.js       # contains the schema and model for the user collection
  │   ├── services/         # contains the functions that interact with external APIs
  │   │   ├── coingecko.js  # contains the functions that use the CoinGecko API
  │   │   └── cryptocompare.js # contains the functions that use the CryptoCompare API
  │   ├── routes/           # contains the routes for the API endpoints
  │   │   ├── crypto.js     # contains the routes for the crypto-related endpoints
  │   │   └── user.js       # contains the routes for the user-related endpoints
  │   ├── config/           # contains the configuration files for the backend
  │   │   ├── db.js         # contains the code for connecting to the database
  │   │   └── env.js
