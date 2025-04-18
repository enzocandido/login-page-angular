# Login Page Application

A modern and responsive authentication application built with Angular. This application provides a secure and user-friendly login and signup system that can be easily integrated into any project requiring authentication.

## Features

- **User Authentication**: Secure login functionality with form validation
- **User Registration**: New user signup with validation
- **Responsive Design**: Works flawlessly on desktop and mobile devices
- **Toast Notifications**: Real-time feedback for user actions using ngx-toastr
- **Form Validation**: Client-side validation for all input fields
- **Component-Based Architecture**: Modular design with reusable components

## Tech Stack

- **Angular** (v19.2.x) - Front-end framework
- **TypeScript** - Programming language
- **Angular Forms** - For form handling and validation
- **Angular Router** - For navigation between pages
- **ngx-toastr** - For toast notifications
- **SCSS** - For styling components

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v18.x or higher)
- npm (v9.x or higher)
- Angular CLI (`npm install -g @angular/cli`)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/enzocandido/login-page-angular.git
   cd login-page-angular
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm start
   ```

4. Open your browser and navigate to `http://localhost:4200/`

## Project Structure

```
src/
├── app/
│   ├── components/             # Shared/reusable components
│   │   ├── default-login-layout/
│   │   └── primary-input/
│   ├── pages/                  # Application pages
│   │   ├── login/              # Login page component
│   │   └── signup/             # Signup page component
│   ├── services/               # Services for business logic
│   │   └── login.service.ts    # Authentication service
│   ├── types/                  # TypeScript types/interfaces
│   └── app.routes.ts           # Application routing
├── styles/                     # Global styles
└── index.html                  # Main HTML file
```

## Usage

### Login

Navigate to `/login` to access the login page. Enter your email and password to authenticate.

### Sign Up

Navigate to `/signup` to create a new account. Fill in the required information and submit the form.

## API Endpoints

The application communicates with a backend server for authentication. The endpoints used are:

- **POST /login**: Authenticates a user and returns a JWT token
- **POST /signup**: Registers a new user

## Configuration

To configure the application for your environment:

1. Update API endpoints in `login.service.ts` to point to your backend server
2. Customize validation rules in form controls as needed
3. Modify toast notification messages to match your requirements

## Building for Production

To build the application for production:

```bash
npm run build
```

The build artifacts will be stored in the `dist/` directory.

## Extending the Application

### Adding New Pages

1. Create a new component: `ng generate component pages/your-page-name`
2. Add a route in `app.routes.ts`
3. Link to the new page from existing components

### Adding New Form Fields

1. Update the form interface and FormGroup in the component
2. Add the new form controls in the HTML template
3. Implement validation as needed

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
