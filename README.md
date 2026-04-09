```
╔════════════════════════════════════════════════════════════════════╗
║                                                                    ║
║        🎬 MOVIE DATABASE APPLICATION - POWERED BY REACT 🎬        ║
║                                                                    ║
║              Search | Discover | Explore | Enjoy Films            ║
║                                                                    ║
╚════════════════════════════════════════════════════════════════════╝
```

# Movie Database Application

A modern, responsive React-based movie search application with a premium Netflix-style interface. Search for movies, view detailed information, and explore a beautiful dark-themed user experience.

## Features

✨ **Modern UI Design**
- Premium black & white minimal aesthetic
- Netflix-inspired card grid layout
- Movie poster background pattern
- Smooth animations and hover effects
- Fully responsive design (mobile, tablet, desktop)

🎬 **Core Functionality**
- Real-time movie search via OMDBAPI
- Detailed movie information popup (title, year, rating, plot, poster)
- Fast, intuitive search interface
- Frosted glass effect search bar

## Tech Stack

- **React** 16.12.0
- **react-scripts** 5.0.1 (upgraded for Node.js v22+ compatibility)
- **axios** - HTTP client for API calls
- **Node.js** v22.18.0+
- **npm** v10.9.0+

## Installation & Setup

1. Clone or navigate to the project directory
2. Install dependencies:
```bash
npm install
```

3. The project includes cross-env for environment variable management:
```bash
npm install cross-env --save-dev
```

## Running the Application

Start the development server:
```bash
npm start
```

The app will open at **http://localhost:3004**

> Note: The app is configured to run on port 3004 to avoid conflicts. The development server includes hot reload—changes to files will automatically refresh the app.

## Environment Configuration

The project uses a `.env` file with the following settings:
- `SKIP_PREFLIGHT_CHECK=true`
- `GENERATE_SOURCEMAP=false`
- `NODE_ENV=development`

## Project Structure

```
react-movie-database/
├── src/
│   ├── App.js         - Main application component
│   ├── index.css      - Styling (Netflix-style design)
│   ├── index.js       - React entry point
│   ├── components/
│   │   ├── Search.js  - Search input component
│   │   ├── Results.js - Results grid container
│   │   ├── Result.js  - Individual movie card
│   │   └── Popup.js   - Movie details modal
│   └── serviceWorker.js
├── public/
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── package.json
└── README.md
```

## API Integration

This app uses the **OMDBAPI** for movie data. The API key is configured in `App.js`.

## Design Features

**Color Scheme:**
- Background: Deep black (#0f0f0f - #1a1a1a)
- Text: Pure white (#ffffff)
- Accents: Subtle grays for secondary elements
- Background Pattern: Movie poster-themed grid with muted colorful stripes

**Component Styling:**
- **Cards:** Sleek black cards with white borders, scale up on hover
- **Search Bar:** Minimal frosted glass effect with smooth focus transitions
- **Modal:** Elegant popup with backdrop blur and smooth animations
- **Typography:** Modern, clean fonts with proper letter-spacing

## Responsive Breakpoints

- **Desktop:** Multicolumn grid (minmax 160px per card)
- **Tablet:** Reduced grid (minmax 120px per card)
- **Mobile:** Compact single-column layout (minmax 100px per card)

## Available Scripts (npm Commands)

**Requirements:** Node.js v22.18.0+ and npm v10.9.0+  
All commands run from the project root directory (`react-movie-database/`)

**Windows Users:** The project uses `cross-env` to automatically set `NODE_OPTIONS=--openssl-legacy-provider` for OpenSSL 3 compatibility with Node.js v22+

### `npm start`

Runs the app in development mode with hot reload enabled.<br />
Opens [http://localhost:3004](http://localhost:3004) in your browser automatically.

The app will reload whenever you make changes to the code. You'll see lint errors and compilation warnings in the console.

**For Windows Users:** The script automatically handles OpenSSL 3 compatibility with Node.js v22+ via the `cross-env` package and `NODE_OPTIONS=--openssl-legacy-provider` flag.

### `npm test`

Launches the test runner in interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production in the `build` folder.<br />
Bundles React in production mode and optimizes for best performance.

The build is minified with hashed filenames for caching. Your app is then ready to be deployed!

### `npm run eject`

**⚠️ Warning: This is a one-way operation. Once you eject, you can't go back!**

Use this command if you need complete control over build configuration. It copies all configuration files and dependencies (Webpack, Babel, ESLint, etc.) into your project, allowing full customization. However, you lose the benefits of centralized Create React App updates.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Troubleshooting

**OpenSSL Error (ERR_OSSL_EVP_UNSUPPORTED):**
If you encounter OpenSSL compatibility issues with Node.js v22+, the project includes the `cross-env` package. The npm scripts should automatically handle the `NODE_OPTIONS=--openssl-legacy-provider` flag.

**Port Already in Use:**
If port 3004 is already in use, you can modify the startup configuration or specify a different port.

## License

This project is open source and available under the MIT License.
