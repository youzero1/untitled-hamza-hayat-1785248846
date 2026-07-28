---
status: pending
title: Build Enterprise-Ready React Application
---

1. **Environment Setup & Configuration**
   - Configure Tailwind CSS v3 in `tailwind.config.js` and `src/styles/global.css`.
   - Setup global styles with `@tailwind` directives.
   - Configure Vite and TypeScript paths (`tsconfig.json`).

2. **Core Infrastructure & Services**
   - Create an Axios instance in `src/lib/api.ts` with interceptors for JWT and error handling.
   - Implement `AuthContext` and `ThemeProvider` in `src/context/` for global state.
   - Setup TanStack Query in `src/main.tsx`.

3. **Atomic UI Component Library**
   - Build reusable components in `src/components/ui/`: `Button`, `Input`, `Card`, `Modal`, `Avatar`, `Loader`.
   - Implement a complex `DataTable` component in `src/components/ui/DataTable` supporting sorting, filtering, and pagination.
   - Build form-specific components using `react-hook-form` and `zod` in `src/components/forms/`.

4. **Layouts & Routing Architecture**
   - Create `MainLayout` and `AuthLayout` in `src/layouts/`.
   - Setup `ProtectedRoute` and `PublicRoute` components in `src/routes/`.
   - Configure `src/routes/index.tsx` with lazy loading for all pages.

5. **Authentication Feature Implementation**
   - Implement login, signup, and forgot password forms in `src/features/auth/`.
   - Create authentication services and hooks (e.g., `useAuth`).

6. **Domain Feature: Book Management**
   - Implement a full CRUD feature for "Books" in `src/features/books/`.
   - Use the reusable `DataTable` to list books.
   - Use `react-hook-form` for adding/editing books.
   - Integrate with TanStack Query for server state management.

7. **Error Handling & Polish**
   - Create a global `ErrorBoundary` in `src/components/common/`.
   - Build 404 and 500 error pages in `src/pages/`.
   - Apply Framer Motion animations for page transitions and modal entries.
   - Ensure responsive design across mobile, tablet, and desktop.
