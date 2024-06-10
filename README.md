# Static Deployer

## Overview
This project can deploy static web-app on AWS S3 with the help of github link

## Setup Instructions

### 1. Setting Up the API Server

1. Navigate to the `api-server` directory:
   ```sh
   cd api-server
   ```
2. Install the necessary dependencies:
   ```sh
   npm install
   ```
3. Start the API server:
    ```sh
   npm start
   ```

### 2. Setting Up the Reverse Proxy
1. Navigate to the `reverse-proxy` directory:
   ```sh
   cd reverse-proxy
   ```
2. Install the necessary dependencies:
   ```sh
   npm install
   ```
3. Start the Reverse Proxy:
    ```sh
   npm start
   ```

### About Project
This Project contains following services and folders:

- `api-server`: HTTP API Server for REST API's
- `build-server`: Docker Image code which clones, builds and pushes the build to S3
- `s3-reverse-proxy`: Reverse Proxy the subdomains and domains to s3 bucket static assets

### Tech stack 
1. Redis 
2. Docker 
3. Express.js
4. AWS (S3, ECR, ECS, IAM)
5. SocketIO
