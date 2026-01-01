# Conga Notification Service

[![Build Status](https://github.com/testorg08/notification-service/workflows/CI/badge.svg)](https://github.com/testorg08/notification-service/actions)

Email, SMS, and in-app notification service for the Conga Platform.

## 🏗️ Architecture

- **Site Group**: CSG1 (Platform Layer)
- **Sync Wave**: 2 (Depends on SSG1 services)
- **Dependencies**: auth-service, user-service
- **Infrastructure**: PostgreSQL, RabbitMQ, S3

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/v1/notifications/send` | Send notification |
| GET | `/api/v1/notifications/templates` | List templates |
| POST | `/api/v1/notifications/templates` | Create template |
| GET | `/api/v1/notifications/history` | Notification history |

## 🌍 Environments

- **Development**: https://notifications-dev.conga.com
- **Staging**: https://notifications-staging.conga.com
- **Production**: https://notifications.conga.com

**Part of the Conga Platform** | **Site Group CSG1** | **Sync Wave 2**