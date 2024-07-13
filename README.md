# TEAM-UI API DOCUMENTATION AND ER DESIGN

## TEAM MEMBERS
- https://github.com/idowuseyi || SlackID: IdosTech
- https://github.com/Cyber9jaDev || SlackID: Cyber9ja
- https://github.com/kobiowuquadri || SlackID: DevQuat
- https://github.com/sirlawglobal || SlackID: akanjilawrence
- https://github.com/dejosemario || SlackID: josemaria

## LINK TO HOSTED API DOCUMENTATION
[API-doc](https://idowuseyi.github.io/hng_Team_UI/)

## LINK TO ER DESIGN
[ER-design](https://app.eraser.io/workspace/AH1e47I3vJF432HRmHAD?origin=share)

## Full-featured Application API

This repository contains the API design and Entity-Relationship (ER) design for a full-featured application designed by TEAM-UI. The application includes authentication, messaging, payments, user and organization management, and more.

### Table of Contents

- [Overview](#overview)
- [API Design](#api-design)
- [ER Design](#er-design)
- [Database Schema](#database-schema)
- [Endpoints](#endpoints)
- [License](#license)

### Overview

This project includes the design for a comprehensive API that supports various functionalities such as user authentication (including social and magic link), messaging, payments, user and organization management, and more.

### Getting Started

## API Design

The API is designed using the OpenAPI 3.0.3 specification. The detailed API documentation is available in this [link](https://idowuseyi.github.io/hng_Team_UI/) file in this repository.

## ER Design

The Entity-Relationship design for this project is defined using the eraser.io tool. The ER design file is available in this [link](https://app.eraser.io/workspace/AH1e47I3vJF432HRmHAD?elements=B_vLReOhcVOH3l-eaV0qww).

### Database Schema

#### Tables

- `users`
- `organizations`
- `user_organizations`
- `social_auth`
- `magic_links`
- `messages`
- `email_templates`
- `payments`
- `charts`
- `content`
- `notifications`
- `blog_posts`
- `invite_links`
- `settings`

#### Relationships

- Users can belong to multiple organizations.
- Organizations can have multiple users.
- Social authentication and magic link tables are linked to users.
- Messages, notifications, payments, and settings are linked to users.

### Endpoints

Here is a summary of the main endpoints. For detailed information, please refer to the `openapi.yaml` file.

#### Authentication

- `POST /auth/register`
- `POST /auth/login`
- `POST /auth/logout`
- `POST /auth/social`
- `POST /auth/magic-link`
- `POST /auth/change-password`

#### Messaging

- `POST /messaging/email`
- `GET /messaging/templates`

#### Payments

- `POST /payments/stripe`
- `POST /payments/flutterwave`
- `POST /payments/lemonsqueezy`

#### Users

- `POST /users`
- `GET /users`
- `GET /users/{id}`
- `PUT /users/{id}`
- `DELETE /users/{id}`

#### Organizations

- `POST /organizations`
- `GET /organizations`
- `GET /organizations/{id}`

#### Other Endpoints

- `GET /charts`
- `GET /content/edit`
- `POST /content/edit`
- `GET /notifications`
- `GET /blog`
- `GET /invite/link`
- `GET /settings/language-region`
- `PUT /settings/language-region`
- `GET /email-templates`
- `POST /email-templates`

### License

This project is licensed under the MIT License.
