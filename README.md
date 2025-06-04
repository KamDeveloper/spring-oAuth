# Authentication Service

Spring Boot application with Google OAuth 2.0 integration.

## Quick Setup

### 1. Google OAuth Configuration

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create OAuth client ID (Web application)
3. Add redirect URI: `http://localhost:8080/login/oauth2/code/google`
4. Copy Client ID and Client Secret

### 2. Environment Variables

```bash
export GOOGLE_CLIENT_ID="your-client-id"
export GOOGLE_CLIENT_SECRET="your-client-secret"
```

### 3. Run Application

```bash
./gradlew bootRun
```

## Access URLs

- **Home**: http://localhost:8080/
- **Login**: http://localhost:8080/login
- **Dashboard**: http://localhost:8080/dashboard
- **User API**: http://localhost:8080/user

## Features

- Google OAuth 2.0 authentication
- Modern responsive UI with Bootstrap 5
- User dashboard with profile information
- JSON API endpoint for user data
- Session management with logout

## Tech Stack

- Spring Boot 3.5.0
- Spring Security OAuth2
- Thymeleaf
- Bootstrap 5
- Java 21 