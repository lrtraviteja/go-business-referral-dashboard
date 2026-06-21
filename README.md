# Referral Dashboard

## Features
- Secure user authentication using JWT cookies.
- Protected referral dashboard.
- Real-time fetching of referral overview and service metrics.
- Referral table with client-side pagination, search, and sorting.
- Referral details page.
- Clean, responsive, and accessible UI.

## Tech Stack
- **Framework**: React with Vite
- **Routing**: react-router-dom
- **Auth**: js-cookie
- **Styling**: Plain CSS with modern variables
- **Testing**: Vitest, React Testing Library

## Getting Started

1. Clone the repository and navigate to the root directory.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```

## Available Scripts

- `npm run dev`: Starts the local development server.
- `npm run build`: Builds the app for production to the `dist` folder.
- `npm test`: Runs the Vitest test suite.
- `npm run smoke:api`: Runs the optional live backend smoke test (not part of the default test command).

## API Integration

The app uses `fetch` for API calls to the provided backend. The auth token is stored securely in a `jwt_token` cookie and is attached as a `Bearer` token to authenticated requests automatically. 

## Testing

Run unit tests via `npm test`.

## Optional Live API Smoke Test

To verify the live backend contract without spinning up a browser:
```bash
npm run smoke:api
```
*Note: Do not commit `.env` or any JWT tokens. The smoke test logs in securely and runs dynamically without saving tokens.*

## Deployment

This app can be deployed easily to **Vercel** or **Netlify**:

1. Push your code to GitHub.
2. Import the project in Vercel/Netlify.
3. The framework will be automatically detected as Vite.
4. **Build command**: `npm run build`
5. **Output directory**: `dist`
6. Deploy!
