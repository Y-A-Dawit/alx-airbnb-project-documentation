# Airbnb Clone - Backend Requirements

## 1. User Authentication

### Functional Requirements

- **User Registration**  
  - Email/password signup with JWT token generation  
  - OAuth 2.0 via Google/Facebook  
  - Role assignment (guest/host)  

- **User Login**  
  - Email/password authentication  
  - Token refresh mechanism  

### Technical Specifications

**API Endpoints**:

```http
POST /api/auth/register  
Request: { email, password, role }  
Response: { user_id, access_token, refresh_token }

POST /api/auth/login  
Request: { email, password }  
Response: { access_token, user_data }