# Local Doc Server Setup Guide

## Local Setup

1. **Clone the Repository**

2. **Install Dependencies**
    ```bash
    npm install
    ```
3. **Start the Documentation Server**
    ```bash
    npm start
    ```
    The server will start at `http://127.0.0.1:8080`

## Making Changes
1. **Install Redocly CLI**
    ```bash
    npm i -g @redocly/cli@latest
    ```
2. **Modify OpenAPI Files**  
Make required changes to the files located in the `openapi/` directory.
3. **Update dist.json**
    ```bash
    cd docs
    redocly bundle ../openapi/openapi.yaml -o dist.json
    ```
4. **Running the Updated Server**
    ```bash
    npm start
