# Deployment Improvements (CI Pipeline)

## Overview

I implemented a CI pipeline using GitHub Actions to automate code validation and basic application testing.

## What the CI Pipeline Does

The pipeline runs on:

* Push to `solution/muskan-sikka`
* Pull requests to `main`

### Steps Included

1. **Checkout Code**

   * Pulls the latest repository code

2. **Setup Node.js**

   * Uses Node.js version 18

3. **Install Dependencies**

   * Installs backend dependencies using npm

4. **Linting**

   * Runs ESLint to check code quality

5. **Build Containers**

   * Builds and starts the application using Docker Compose

6. **Health Check**

   * Verifies backend API is running using a curl request

## Why This Improvement Matters

* Ensures code quality through linting
* Detects breaking changes early
* Verifies application runs correctly in a containerized environment
* Automates testing before merging code

## Future Improvements

* Add unit and integration tests
* Add frontend build validation
* Add deployment to cloud platforms (AWS/Vercel)
