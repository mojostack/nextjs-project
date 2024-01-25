# Basic project using Next.js with Supabase Integration

## 1. Setup:

- Create a new Next.js 14 application using the app router.
- Set up a Supabase project (database and authentication).
- Initialize a Git repository for the project and create a repository on GitHub.

## 2. Next.js:

- Keep the UI crisp and minimal. Use NextUI library for UI.
- Create the following pages:
  - Homepage
  - Login Page
  - Sign-up Page
  - Agent Dashboard
  - Owner Dashboard

## 3. Supabase:

- Have 2 tables: Countries and Cities (cities should have a relation with countries table).
- Add the following countries to the Countries table: India, United Kingdom, France.
- Add the following cities to the Cities table: Chennai, Bangalore, Mumbai, Paris, London.
- Enable RLS on Supabase for both tables. Owners can view and delete data. Agents can only view data.

## 4. Frontend Integration:

### Homepage:

- Display a message "Welcome to the app."

### User Roles and Authorization:

- Use email/password-based Supabase auth integration.
- Extend the Supabase Auth integration to handle user roles (Owner and Agent).
- Implement role-based authorization on the frontend. Only owners can access the delete functionality.

### Dashboard Page:

- Create a dashboard page that acts as the main landing page after login.
- Display a welcome message based on the user role (e.g., "Welcome Owner" or "Welcome Agent").
- If the user is not logged in, show an error "Cannot access page."
- For owners, show "Welcome Owner" as a heading. Display a table with two columns - City name and country name.
- Owners can delete data.

### Loading States and Error Handling:

- Implement loading states for data fetching operations.
- Add proper error handling and display error messages to users when there are issues with API calls or data operations.

## 5. GitHub:

- Commit your code regularly as you work on the project.
- Push the final codebase to the GitHub repository.
