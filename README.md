# Zenn UI

## Angular App

## Setup

<details open>
<summary>
Pre-requisites
</summary> <br />
To be able to start development on Zenn, make sure that you have the following prerequisites installed:

###

- Required Node.js version: [14.23.1]
- Required Docker version: [26.0.0]
- Required Git version: [2.31.1]


### Backend configuration

To use local backend with this application, follow these instructions:

<a href="https://github.com/We-Make-Footballers/wmf-admin/tree/master/Source/Api" target="_blank">WMF-Admin</a>
<a href="https://github.com/We-Make-Footballers/parentarea-api" target="_blank">Parentarea-Api</a>
</details>

---

1. **Clone the Repository**: 
   ```bash
   git clone <repository-url>
   ```

2. **Instal dependencies**:

    ```bash
   npm install
   ```
    
**Husky Setup:** Husky will be installed automatically along with the other dependencies. Husky helps to set up Git hooks easily in your project.

---

## Environment Configuration
This project uses environment variables to manage configurations. Follow these steps to set up your environment:

1. **Create `.env` file:**

  ```bash
  touch .env
  ```
2. **Copy `.env.dist` to `.env`**
    
  ```bash
  cp .env.dist .env
  ```

3. **Update Environment Variables:**

Open the `.env` file and update the variables according to your environment.

---
## Development Server
Run `npm run start` for a dev server. Navigate to http://localhost:`{ PORT }`/. The app will automatically reload if you change any of the source files.

---
## Build
Run `npm run build` to build the project. The build artifacts will be stored in the dist/ directory. By default build the application with `--prod` flag.

---
## Running Tests
This project uses <a href="https://www.cypress.io/" target="_blank">`Cypress`</a> for end-to-end testing. To run the tests use:

- **Run tests with with UI up**
  ```bash
  npm run e2e
  ```

- **Run tests only with the console**
  ```bash
  npm run test:ui
  ```

---
