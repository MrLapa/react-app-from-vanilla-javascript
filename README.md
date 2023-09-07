# react-app-from-vanilla-javascript
This repository demonstrates how to transform a Vanilla JavaScript application into a React application and sets up the application's entry point.

**Note:** This project initially uses the [Vite](https://vitejs.dev/) web framework to create the Vanilla JavaScript project.

## Installation Instructions

Follow these steps to set up your React environment:

### Step 1: Install React Dependencies

Run the following command to install React and React DOM:

```shell
npm install react react-dom
```

### Step 2: Install and set up the Vite Plugin for React
Install the Vite plugin for React using the following command:

```shell
npm i @vitejs/plugin-react
```

After installing the Vite plugin, set up the `vite.config.js` file with the following code:

```shell
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";

export default defineConfig({
  plugins: [react()],
});
```

### Step 3: Setting up the React Application
Now that you have installed the necessary dependencies, let's set up the React application.

Configure the JavaScript Entry Point
In your existing main.js file, add the following code to set up the React app:

```shell
import React from "react";
import { createRoot } from "react-dom";

createRoot(document.getElementById("root")).render(<h1>Hello World!</h1>);
```

### Step 4: Update the index.html File
In your index.html file, make sure it contains the following lines to load your React application:

```shell
<div id="root"></div>
<script type="module" src="/main.js"></script>
```

### Step 5: Rename the Entry File
Rename the main.js file to main.jsx to indicate that it contains JSX code.

### Start React app
You are now ready to start your React application using Vite. Run the following command:

```shell
npm run dev
```

Congratulations! You have successfully set up your React development environment. Happy coding! 🎉
