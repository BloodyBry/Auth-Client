# Auth Client — SPA & Social Login

## 📌 Project Overview

Auth Client is a Single Page Application (SPA) built to consume a Laravel REST API and provide a complete authentication system.

The application supports:

- Classic authentication (register / login with token)
- Profile management
- Secure logout
- Account deletion
- Social login using OAuth2 (Google + GitHub)

This project is part of a frontend mission at **NexaAuth**, a startup specialized in identity solutions for SMEs.

---

# ⚙️ Tech Stack

## Frontend

- Framework: **React.js**
- State Management: **Zustand**
- HTTP Client: **Axios**
- Styling: **Tailwind CSS**
- Routing: **React Router**

## Backend

- Laravel API (existing)
- Authentication: **Laravel Sanctum**
- Social Login: **Laravel Socialite**

---

# 🎯 Why React?

React was chosen because:

- Simple and fast to set up
- Large ecosystem
- Perfect for building SPAs
- Easy state management with Zustand
- Clean separation between UI and logic

---

# 🚀 Features

## 🔐 Classic Authentication

- Register (POST /api/register)
- Login (POST /api/login)
- Logout (POST /api/logout)
- Token stored securely
- Route protection (private routes)

---

## 👤 Profile Management

- View profile (GET /api/me)
- Update profile (PUT /api/me)
- Change password (PUT /api/me/password)

⚠️ Password change is disabled for OAuth users

---

## 🔗 Social Login (OAuth2)

- Login with Google
- Login with GitHub

Flow:

1. Redirect to provider
2. User authenticates
3. Callback returns token
4. User redirected to `/profile`

---

## 🔒 Protected Routes

- `/profile` is protected
- Redirect to `/login` if not authenticated

---

## ❌ Error Handling

- API errors displayed clearly
- No raw stack traces
- Friendly messages

---

## 📱 UX Features

- Loading indicators
- Responsive design
- Clean UI
- 404 page for unknown routes

---

# 🧩 User Stories Covered

| ID | Description |
|----|------------|
| US-01 | User can register |
| US-02 | User can login |
| US-03 | User can view/update profile |
| US-04 | User can change password |
| US-05 | User can logout |
| US-06 | Login with Google |
| US-07 | Login with GitHub |
| US-08 | Route protection |
| US-09 | Delete account |

---