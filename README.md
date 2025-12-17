# Notes App (Auth-Protected)

A minimal notes application with Auth0 authentication. Users can log in and manage personal notes stored in localStorage.

## Setup Instructions

1. **Create an Auth0 Account**
   - Go to [auth0.com](https://auth0.com) and sign up
   - Create a new tenant

2. **Create an Application**
   - In Auth0 Dashboard, go to Applications
   - Click "Create Application"
   - Choose "Single Page Web Applications"
   - Select "Vanilla JS"

3. **Configure Application Settings**
   - Set Allowed Callback URLs: `http://localhost:3000`
   - Set Allowed Logout URLs: `http://localhost:3000`
   - Set Allowed Web Origins: `http://localhost:3000`

4. **Update Configuration**
   - Replace `YOUR_AUTH0_DOMAIN` in `index.html` with your Auth0 domain
   - Replace `YOUR_CLIENT_ID` in `index.html` with your application's Client ID

5. **Run the Application**
   ```bash
   # Serve the files (you can use any local server)
   npx serve .
   # Or use Python
   python -m http.server 3000
   ```

## Key Features

- Auth0 login/logout
- Create and view personal notes
- Notes visible only after login
- Notes stored per user in localStorage
- Delete notes functionality
