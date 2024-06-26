# React-csv-upload

A basic web app built with Node.js and React that uses Express for handling uploads, NeDB for storing data, and csv-parse to process CSV files.

## Installation

### Prerequisites

Check if you have the right versions of node and npm as listed in package.json.

### Installation

- Clone the repository.
- Navigate to the project directory.
- Install the required dependencies:

    ```bash
    npm install
    ```

## Node.js Backend

1. Navigate to the node files.
2. Run the command:

    ```bash
    node index.js
    ```

    This will start the server which will listen on port 3000 for requests.

## React.js Frontend

1. Navigate to the React files.
2. Run the command:
 
    ```bash
    npm start
    ```

    This will start the React application. Open your web browser and navigate to `http://localhost:3001` to view the application.

### Using the React Frontend

-   **Upload a CSV File**: Click the "Upload CSV" button to select and upload a file. 
    
-   **Search Users**: Enter a search term in the input field and click on the "Search" button to retrieve users based on the entered criteria.
    
### Node.js Backend Interaction

-   **Delete All Data**: To clear all data from the database, you can use the following curl command to send a DELETE request to the backend, as this functionality is managed directly via API:

    ```bash
    Invoke-WebRequest -Uri http://localhost:3000/api/files -Method DELETE
    ```
    
## Testing

To run the automated tests, follow these steps:

1. Make sure the server is running.
2. Open a terminal or command prompt.
3. Navigate to the project directory.
4. Run the following command to execute the tests for `Api.test.js`:

    ```bash
    npm test Api.test.js
    ```

5. Run the following command to execute the tests for `App.test.js`:

    ```bash
    npm test App.test.js
    ```