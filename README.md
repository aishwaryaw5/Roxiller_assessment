# Roxiller_assessment
#Frontend

This frontend project is designed to interact with backend APIs for managing and analyzing product transactions. It provides a user interface with a table and charts based on data fetched from the backend.

Usage

To use the frontend application, follow these instructions:

Ensure the backend API is deployed and accessible.
Clone the frontend repository to your local machine.
Install the necessary dependencies using the package manager of your choice (e.g., npm or yarn)
Features

Transactions Table
Select Month Dropdown

Displays options from January to December.
Defaults to March.
Allows selecting a different month to display transactions.
Transactions List

Utilizes the transactions listing API to list transactions in a table.
Displays transactions of the selected month irrespective of the year using the API.
Search transaction box filters transactions based on title/description/price using the API.
Clears the search box to display the initial list of transactions for the selected month using the API.
Next and Previous buttons load the next and previous page data from the API.
Transactions Statistics
Displays total sale amount, total sold items, and total not sold items for the selected month.
Fetches data from the created API to populate the statistics box.
Transactions Bar Chart
Displays a bar chart showing the price range and the number of items in that range for the selected month.
Applies the selected month from the dropdown (above the table) to fetch data from the API.
Enjoy using the product transaction management system!

#Backend 


This project aims to implement a backend system to manage and analyze product transactions. The backend interacts with a third-party API to fetch product transaction data and provides various APIs for listing transactions, generating statistics, and creating charts based on the fetched data.

API Endpoints

Initialize Database
Endpoint: /api/initDatabase
Method: GET
Description: Initializes the database by fetching JSON data from the third-party API and seeding the database with the received data.
List All Transactions
Endpoint: /api/transactions
Method: GET
Description: Lists all transactions based on the provided search parameters and pagination.
Query Parameters:
month (required): The month to filter transactions.
search (optional): Search text to match against product title/description/price.
page (optional): Page number for pagination (default: 1).
perPage (optional): Number of records per page (default: 10).
Statistics
Endpoint: /api/statistics
Method: GET
Description: Provides statistics for the selected month.
Query Parameters:
month (required): The month to retrieve statistics.
Bar Chart
Endpoint: /api/bar-chart
Method: GET
Description: Generates data for a bar chart, showing the price range and the number of items in each range for the selected month.
Query Parameters:
month (required): The month to generate the bar chart.
Pie Chart
Endpoint: /api/pie-chart
Method: GET
Description: Generates data for a pie chart, showing unique categories and the number of items from each category for the selected month.
Query Parameters:
month (required): The month to generate the pie chart.
Combined Data
Endpoint: /api/combined-data
Method: GET
Description: Fetches data from all the above APIs and combines the responses.
How to Use

To interact with the APIs, make HTTP requests to the specified endpoints with the required parameters. Ensure that the month parameter is provided in all relevant requests.

Feel free to explore and analyze the product transactions using the provided APIs. If you have any questions or issues, please refer to the documentation or contact the project maintainers.
