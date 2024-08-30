# Forkify Recipe App

## Overview

Forkify is a modern recipe application designed to help users search for recipes, view detailed information about individual recipes, bookmark their favorites, and add new recipes. Built with JavaScript modules, this app provides a clean and interactive user experience, leveraging modern JavaScript features and APIs.

## Features

- **Recipe Viewing:** Access detailed information about recipes, including ingredients, cooking time, servings, and images.
- **Search Functionality:** Search for recipes based on keywords, and filter results accordingly.
- **Pagination:** Navigate through search results with easy-to-use pagination controls.
- **Bookmarking:** Save and manage your favorite recipes with the ability to view and delete bookmarks.
- **Recipe Upload:** Add new recipes to the app with a user-friendly form that validates input.

## Installation

To get started with Forkify, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd forkify
   ```

2. **Install Dependencies:**
   Install the necessary dependencies using npm:
   ```bash
   npm install
   ```

3. **Start the Development Server:**
   Launch the development server and open the app in your browser:
   ```bash
   npm start
   ```

4. **Build for Production:**
   Create a production-ready build of the app:
   ```bash
   npm run build
   ```
   The build files will be output to the `./dist` directory.

## Usage

### Development Server

To run the development server, use:
```bash
npm start
```
This command starts Parcel, which will bundle your files and serve the app at `http://localhost:1234`.

### Production Build

To generate a production build, use:
```bash
npm run build
```
This will create a set of optimized files in the `./dist` directory, ready for deployment.

## Code Structure

### `model.js`

Handles the application's state and data management. Key functionalities include:
- **Loading Recipes:** Fetches recipe data from the API and formats it.
- **Search:** Manages search queries and results.
- **Bookmarks:** Adds, deletes, and persists bookmarks.
- **Recipe Upload:** Handles the submission of new recipes.

### `controller.js`

Manages the application logic and user interactions. It controls:
- **Recipe Display:** Updates the UI with recipe details.
- **Search Results:** Renders search results and handles pagination.
- **Bookmarking:** Manages bookmark state and updates the UI accordingly.
- **Recipe Upload:** Handles form submission and updates the app state.

### `package.json`

Contains metadata about the project and defines scripts for development and production:
- **`start:`** Runs the development server using Parcel.
- **`build:`** Builds the project for production.

### Dependencies

- `core-js`: Provides polyfills for modern JavaScript features.
- `fractional`: Utility for handling fractions in recipe ingredients.
- `regenerator-runtime`: Required for async/await support.

### Development Dependencies

- `@parcel/transformer-sass`: Enables Sass support for Parcel.
- `parcel`: Bundler used for development and production builds.

## Configuration

To use the Forkify app, you will need to configure the API URL and API key in `config.js`. Ensure you replace placeholders with your actual API credentials.

## API Details

The app communicates with an external recipe API. Key endpoints include:
- **Recipe Data:** `GET ${API_URL}${id}?key=${KEY}` - Fetches detailed information about a specific recipe.
- **Search Recipes:** `GET ${API_URL}?search=${query}&&key=${KEY}` - Searches for recipes based on a query string.

## Contributing

We welcome contributions to Forkify! If you'd like to contribute, please follow these guidelines:
- Fork the repository and clone it to your local machine.
- Create a new branch for your changes.
- Make your modifications and test thoroughly.
- Submit a pull request describing your changes and why they are beneficial.

## Troubleshooting

If you encounter any issues:
- Ensure all dependencies are installed correctly.
- Check the browser console for errors and verify that the API key and URL are correct.
- Consult the documentation or open an issue on GitHub if you need further assistance.

## Acknowledgments

- **Parcel:** A fast and feature-rich bundler used for this project.
- **API Providers:** The external recipe API used for fetching recipe data.

## License

This project is licensed under the ISC License. See the [LICENSE](./LICENSE) file for details.

## Author

**Umer**
