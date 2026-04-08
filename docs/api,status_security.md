# GET /api/status
This endpoint returns a JSON response with the version number of the software and uptime, ensuring complete hardening against SQL injections, rate limiting, authentication with JWT, role-based authorization, and comprehensive test coverage.

## Security Measures
- **SQL Injection Prevention:** All database operations use parameter binding to prevent SQL injection attacks.
- **Rate Limiting:** Implement rate-limiting middleware globally to control the request flow for all endpoints including /api/status.
- **Authentication & Authorization:** JWT tokens are required for endpoint requests, and a role-based system enforces permissions at the endpoint level.