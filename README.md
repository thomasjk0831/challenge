## Overview
Below are the steps and choices made to configure this project for production.

## Getting Started

### Prerequisites

- Node.js v18 or higher
- npm or yarn

### Install Dependencies

To install the necessary dependencies, run:

npm install

### Environment Config

Ensure sensitive information is not hard-coded but stored in env variables:

npm i dotenv

add .env file to store variables such as Ports, Urls, etc

### Add tests

Setup Jest for unit tests:

npm jest --init

to test run:

npm run test

### Error Handling
handle errors gracefully and ensure that the application can restart in case of crash

implementation: 
handle errors where the directory does not match any routes.
handle all other types of errors using a custom middleware
use a process manager like PM2 to ensure app restarts in case of unhandled error

### Quality of life

Setup nodemon and eslint for easier and more effcient development

### Security

use library such as fastify-helmet to set HTTP security headers.

### Continuous Integration

Setup CI to avoid version conflicts and to automate the process of testing and building.





