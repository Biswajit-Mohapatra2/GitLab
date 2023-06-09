# GitLab

# Python Flask - Demo Web Application CI/CD with GitLab

This is a simple Python Flask web application. The app provides system information and a realtime monitoring screen with dials showing CPU, memory, IO and process information.

The app has been designed with cloud native demos & containers in mind, in order to provide a real working application for deployment, something more than "hello-world" but with the minimum of pre-reqs. It is not intended as a complete example of a fully functioning architecture or complex software design.

## ScreenShot

![gitlab-cicd](https://user-content.gitlab-static.net/6f581c4c2e4c645ab4523bd3661204bcddf53979/68747470733a2f2f757365722d696d616765732e67697468756275736572636f6e74656e742e636f6d2f31343938323933362f33303533333137312d64623137666363632d396334662d313165372d383836322d6562386331343866656465612e706e67)

This repository contains the source code and configuration for implementing Continuous Integration and Continuous Deployment (CI/CD) using GitLab.

## Overview

The purpose of this project is to automate the build, test, and deployment process for our application using GitLab CI/CD. By leveraging the GitLab CI/CD pipeline, we can ensure that our code is continuously built, tested, and deployed in a controlled and consistent manner.

## Project Structure

```
├── .gitlab-ci.yml # GitLab CI/CD pipeline configuration
├── src/ # Source code directory
│ ├── app/ # Application source code
│ └── tests/ # Unit and integration tests
├── scripts/ # Scripts for build, test, and deployment
└── docs/ # Project documentation
```

## GitLab CI/CD Pipeline

The `.gitlab-ci.yml` file at the root of this repository defines the GitLab CI/CD pipeline configuration. The pipeline is responsible for executing the following stages:

1. **Build**: Compiles the source code and generates build artifacts.
2. **Test**: Runs unit and integration tests to ensure code quality and correctness.
3. **Deploy**: Deploys the application to a staging or production environment.

Each stage may consist of multiple jobs that are executed sequentially or in parallel, depending on the configuration. The pipeline configuration can be customized to meet specific project requirements.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository: `git clone <repository-url>`
2. Navigate to the project directory: `cd <project-directory>`
3. Configure the GitLab CI/CD pipeline by modifying the `.gitlab-ci.yml` file.
4. Customize the build, test, and deployment scripts in the `scripts/` directory to fit your project's needs.
5. Update the source code in the `src/` directory with your application code.
6. Commit and push your changes to trigger the GitLab CI/CD pipeline.
