# Angular-first-app

This project is a tutorial application for learning Angular, built as part of the "Tour of Heroes" tutorial provided by the Angular team. The application helps manage a list of heroes, demonstrating core Angular concepts and practices. This repository was created as a crash course in Angular development.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Features](#features)
- [Running the Application](#running-the-application)
- [Running the JSON Server](#running-the-json-server)
- [Building the Application](#building-the-application)
- [Further Reading](#further-reading)
- [License](#license)

## Prerequisites

To run and develop this project, you'll need the following installed on your machine:

- [Node.js](https://nodejs.org/) (version 14.x or higher)
- [npm](https://www.npmjs.com/) (version 6.x or higher)
- [Angular CLI](https://cli.angular.io/) (version 12.x or higher)
- [json-server](https://www.npmjs.com/package/json-server)

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/enshikuku/angular-first-app.git
   cd angular-first-app
   ```

2. **Install the dependencies**:
   ```bash
   npm install
   ```

3. **Run the JSON server**:
   ```bash
   npm install -g json-server
   json-server --watch db.json
   ```

4. **Run the application**:
   ```bash
   ng serve
   ```

5. **Open your browser** and navigate to `http://localhost:4200/`.

## Project Structure

```plaintext
src/
├── app/
│   ├── hero-detail/
│   ├── heroes/
│   ├── messages/
│   ├── app-routing.module.ts
│   ├── app.component.ts
│   ├── app.module.ts
│   └── ...
├── assets/
├── environments/
├── db.json
├── index.html
├── main.ts
├── styles.css
└── ...
```

- **app/**: Contains the main application code and components.
- **assets/**: Contains static assets like images.
- **environments/**: Contains environment-specific configuration files.
- **db.json**: Mock database file for `json-server`.
- **index.html**: The main HTML file.
- **main.ts**: The main entry point for the application.
- **styles.css**: Global styles for the application.

## Features

- **Hero Management**: Add, edit, and delete heroes.
- **Hero Search**: Search heroes by name.
- **Navigation**: Navigate between different views (dashboard, hero details, etc.).
- **Messages**: Display messages to the user.
- **HTTP Integration**: Fetch data from a mock server using `json-server`.

## Running the Application

To run the application locally, use the following command:

```bash
ng serve
```

Then, open your browser and navigate to `http://localhost:4200/`.

## Running the JSON Server

To run the JSON server, use the following command:

```bash
json-server --watch db.json
```

This will start a mock REST API server at `http://localhost:3000/`. Ensure the server is running before starting the Angular application.

## Building the Application

To build the application for production, use the following command:

```bash
ng build
```

The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Further Reading

- [Angular Documentation](https://angular.io/docs)
- [Tour of Heroes Tutorial](https://angular.io/tutorial)
- [Angular CLI](https://cli.angular.io/)
- [json-server](https://www.npmjs.com/package/json-server)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.