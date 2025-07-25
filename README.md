# Project Manager

This is a simple project management tool built with TypeScript that allows you to manage your projects in "Active" and "Finished" categories. It features a drag-and-drop interface to move projects between these two states.

[Link to Live Demo](https://natata08.github.io/drag-and-drop-ts/)

## Features

- Create new projects with a title, description, and number of people.
- View projects in two separate lists: Active and Finished.
- Drag and drop projects from the Active list to the Finished list.
- Built with modern web technologies and a clean, component-based architecture.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (which includes npm) must be installed on your system.

### Installation

1.  Clone the repository or download the source code.
2.  Navigate to the project directory:
    ```bash
    cd drag-and-drop-ts
    ```
3.  Install the dependencies:
    ```bash
    npm install
    ```

### Running the Application

To start the development server, run the following command:

```bash
npm run dev
```

This will open the application in your default web browser.

## Technologies Used

- **TypeScript**: For type-safe JavaScript development.
- **Vite**: As the build tool and development server.
- **HTML5 & CSS3**: For the structure and styling of the application.

## TypeScript Features Used

This project demonstrates a variety of TypeScript features, including:

- **Classes and Object-Oriented Programming (OOP)**: The application is built with a clear, component-based architecture using classes for components, state, and models.
- **Inheritance**: The `ProjectList` and `ProjectInput` components extend a generic `Component` base class to reduce code duplication.
- **Abstract Classes**: The `Component` class is an `abstract` class, defining a contract that other components must follow.
- **Generics**: The base `Component` class uses generics (`<T extends HTMLElement, U extends HTMLElement>`) to provide strongly-typed access to DOM elements.
- **Interfaces**: The `DragTarget` interface is implemented by the `ProjectList` class to ensure it correctly handles drag-and-drop events.
- **Decorators**: A custom `@autobind` decorator is used to automatically bind the `this` context for event handler methods.
- **Enums**: The `ProjectStatus` enum is used to clearly define the possible states of a project (e.g., `Active` or `Finished`).
