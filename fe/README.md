# Chat-X Frontend

This is the **Angular frontend** for the Chat-X project. It provides the user interface and communicates with the Django REST Framework (DRF) backend.

## Folder Structure

- `src/app/` – main Angular app files
- `src/assets/` – static assets like images
- `src/environments/` – environment configuration (API URLs, etc.)

## Prerequisites

- Node.js (v18+ recommended)
- npm (or Yarn)
- Angular CLI (`npm install -g @angular/cli`)

## Setup & Installation

1. Navigate to the frontend folder:

```bash
cd fe
Install dependencies:

bash
Copy code
npm install
Run the development server:

bash
Copy code
ng serve
The app will be available at http://localhost:4200.

Building for Production
bash
Copy code
ng build --prod
The output will be in the dist/ folder.

You can configure Django to serve these files or deploy them separately on a static hosting service.

Configuration
Update API endpoints in src/environments/environment.ts (for development) and environment.prod.ts (for production) to point to your Django backend.

Contributing
Make sure to run npm install after pulling new changes.

Follow Angular best practices when adding components or services.

License
MIT License

yaml