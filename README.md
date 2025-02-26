# CI/CD Pipeline with GitHub Actions

## Overview

This project demonstrates how to integrate a CI/CD pipeline using GitHub Actions. The pipeline:
1. Runs Cypress tests when a Pull Request (PR) is made to the `develop` branch.
2. Deploys the app to Render when code is merged into the `main` branch.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   cd your-repository-name

2. **Deploy to Render**:
- Create an account on Render.
- Deploy the app and disable Auto-Deploy in Settings.
- Copy the Deploy Hook URL for GitHub Actions.

3. **Set Up GitHub Actions**:
- Create a develop branch (e.g., git checkout -b develop).
- Set up two GitHub Actions workflows:
    - Test Workflow: Runs Cypress tests on PRs to develop.
    - Deploy Workflow: Deploys to Render when develop is merged into main.

4. **Add GitHub Secrets**:
- Add RENDER_API_KEY and RENDER_DEPLOY_HOOK_URL as GitHub secrets.

5. **Run Locally**:

   ```bash
   npm install
   npm start

Access the app at http://localhost:3000.

## GitHub Actions

- Cypress Tests: Triggered on PRs to develop.
- Deployment: Triggered when merging develop into main.

## Contributing
Feel free to fork the repository and submit pull requests.

## License
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)