# Netflix Clone - Modern Streaming Platform

A modern Netflix clone built with React, TypeScript, and Material UI that replicates the core functionality and user interface of Netflix.

<div align="center">
  <a href="http://netflix-clone-with-tmdb-using-react-mui.vercel.app/">
    <img src="./public/assets/netflix-logo.png" alt="Logo" width="100" height="32">
  </a>

  <p align="center">
    <a href="https://netflix-clone-react-typescript.vercel.app/">View Demo</a>
    ·
    <a href="https://github.com/cyber-cl/Netflix_Clone/issues">Report Bug</a>
    ·
    <a href="https://github.com/cyber-cl/Netflix_Clone/issues">Request Feature</a>
  </p>
</div>

## Features

- Browse movies and TV shows by genre, popularity, and more
- View detailed information about movies and TV shows
- Watch trailers and previews
- Responsive design for all devices
- Infinite scrolling for content discovery
- Custom video player with YouTube integration

## Technologies Used

- **Frontend Framework**: React with TypeScript
- **UI Library**: Material UI (MUI)
- **State Management**: Redux Toolkit with RTK Query
- **Routing**: React Router v6
- **Animation**: Framer Motion
- **Video Player**: Video.js with YouTube integration
- **Carousel/Slider**: React Slick
- **Build Tool**: Vite

## Screenshots

<div align="center">
  <img src="./public/assets/home-page.png" alt="Home Page" width="100%" height="100%">
  <p align="center">Home Page</p>
  
  <img src="./public/assets/mini-portal.png" alt="Mini Portal" width="100%" height="100%">
  <p align="center">Mini Portal</p>
  
  <img src="./public/assets/detail-modal.png" alt="Detail Modal" width="100%" height="100%">
  <p align="center">Detail Modal</p>
  
  <img src="./public/assets/grid-genre.png" alt="Grid Genre" width="100%" height="100%">
  <p align="center">Grid Genre Page</p>
  
  <img src="./public/assets/watch.png" alt="Watch Page" width="100%" height="100%">
  <p align="center">Watch Page with custom control bar</p>
</div>

## Getting Started

### Prerequisites

- Node.js 16.x or higher
- TMDB API key (create one at [themoviedb.org](https://www.themoviedb.org/))

### Installation

1. Clone the repository
```bash
git clone https://github.com/cyber-cl/Netflix_Clone.git
cd Netflix_Clone
```

2. Install dependencies
```bash
npm install
```

3. Create a .env file in the root directory with your TMDB API key
```
VITE_APP_TMDB_V3_API_KEY=your_api_key_here
VITE_APP_API_ENDPOINT_URL=https://api.themoviedb.org/3
```

4. Start the development server
```bash
npm run dev
```

## Docker Deployment

```bash
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t netflix-clone .
docker run --name netflix-clone-website --rm -d -p 80:80 netflix-clone
```

## Kubernetes Deployment

1. Update the deployment.yml and service.yml files with your configuration
2. Apply the Kubernetes manifests
```bash
kubectl apply -f deployment.yml
kubectl apply -f service.yml
```

## Key Implementation Details

- **React Router v6**: Using the new lazy loading and data loader features
- **Portal Implementation**: For modal dialogs and video previews
- **Forwarding Refs**: Making components reusable
- **Higher Order Components**: For shared functionality
- **Custom MUI Theme**: Tailored to match Netflix's design
- **RTK Query**: For efficient API data fetching and caching
- **Infinite Scrolling**: Using Intersection Observer API
- **Custom Carousel**: Built with react-slick

## Future Improvements

- Add user authentication and profiles
- Implement watchlist and favorites functionality
- Add search functionality
- Improve performance with code splitting and lazy loading
- Add unit and integration tests
- Implement accessibility features

## License

MIT License - see LICENSE file for details

## Acknowledgments

- [TMDB](https://www.themoviedb.org/) for providing the movie and TV show data
- Netflix for the inspiration