# API_creation

## Overview
This project involves two Jupyter notebooks: `client.ipynb` and `server.ipynb`. They are designed to work together in a client-server communication setup, where the client sends requests and the server processes and responds to those requests.

---

## Files

### 1. `client.ipynb`
The `client.ipynb` notebook is responsible for sending HTTP requests to the server. It includes the following features:
- **Access Token Handling**: Reads access tokens from a CSV file.
- **Request Handling**: Sends requests to various endpoints exposed by the server, such as retrieving country counts and age groups of users.
- **Response Processing**: Handles the server's responses and displays the data in the notebook.

### 2. `server.ipynb`
The `server.ipynb` notebook sets up a Flask-based server that listens for incoming requests from the client. It includes several endpoints for:
- **Connectivity Check**: Tests connectivity with the client.
- **Data Processing**: Counts users by nationality and age groups based on data sent by the client.
- **Access Token Validation**: Validates access tokens provided by the client.
- **Error Handling**: Responds appropriately to invalid requests or incorrect endpoints.

---

## Client-Server Interaction
- The client sends HTTP requests, including data and access tokens.
- The server processes these requests, validates the tokens, performs the requested operations (such as counting users by nationality or age), and returns the response to the client.
