# Restaurant Explorer — Client

A React and TypeScript app for discovering Toronto restaurants. Browse by cuisine, price, occasion, and distance, explore directions, and share community recommendations.

## Stack

React, TypeScript, Material UI, Axios, and Google Maps Embed API.

## Local development

Requires Node.js and npm.

```sh
npm ci
```

Create a `.env.local` file:

```dotenv
REACT_APP_API_BASE_URL=http://localhost:8000/api/v1
# Optional: enables embedded directions
REACT_APP_GOOGLE_MAPS_API_KEY=your_google_maps_key
```

Start the [API server](https://github.com/thomas-m1/restaurant_recommender_server), then run:

```sh
npm start
```

The app runs on port 3000. Build a production bundle with `npm run build`.

The default directions origin is Toronto City Hall. Users can enter a custom starting location. Restaurant distances are calculated by the batch importer.

## Related repositories

- [API server](https://github.com/thomas-m1/restaurant_recommender_server)
- [Batch importer](https://github.com/thomas-m1/restaurant_recommender_batch)
