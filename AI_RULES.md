# AI Rules and Project Guidelines

This document outlines the technology stack and specific rules for developing and modifying this application.

## Tech Stack Overview

1.  **Frontend Framework:** React with TypeScript.
2.  **Build Tool:** Vite.
3.  **Routing:** React Router (`react-router-dom`).
4.  **Styling:** Tailwind CSS, used exclusively for all component styling.
5.  **UI Components:** shadcn/ui (built on Radix UI).
6.  **Icons:** Lucide React.
7.  **State Management (Data Fetching):** TanStack Query (used for setup, ready for API integration).
8.  **Design System:** Custom Bio Site Design System defined in `src/index.css` using Tailwind layers and CSS variables.

## Library Usage Rules

*   **Components:** Always use components from `src/components/ui/` (shadcn/ui) when available. If a custom component is needed, place it in `src/components/`.
*   **Styling:** All styling must be implemented using Tailwind CSS classes. Avoid inline styles unless absolutely necessary for dynamic CSS variables (like colors or background images derived from user configuration).
*   **Icons:** Use icons imported from `lucide-react`.
*   **Routing:** Maintain all primary routes within `src/App.tsx`. Use `react-router-dom` components (`Link`, `useNavigate`, etc.) for navigation.
*   **File Structure:**
    *   Pages go into `src/pages/`.
    *   Reusable components go into `src/components/`.
    *   Utility functions go into `src/utils/`.
    *   Hooks go into `src/hooks/`.
    *   Type definitions go into `src/types/`.
*   **Editor Configuration:** The core logic for managing the editable configuration should reside in `src/context/EditorContext.tsx` and the types in `src/types/editor.ts`.