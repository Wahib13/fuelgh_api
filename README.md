### Description
A RESTful web service for reliable information on Ghana's fuel situation. Built with Python + FastAPI

### Project Motivation
Almost all consumer products have a way consumers can compare prices and buy what suits their budget. I believe there is the need to create an authoritative source that tracks the prices of crude oil products and help consumers make an informed decision when buying diesel/petrol.

### How It works, Data Sources
The current data source is from the National Petroleum Authority website: http://www.npa.gov.gh/. The homepage is analyzed to extract the URL for the latest pricing data. This is in an Excel sheet format that is then read using openpyxl and loaded into a database.
<br>
You can access the live service at http://fuelgh.com/docs

### Setup Instructions
There are no pre-setup instructions/installation required. The application comes with docker-compose files and runs within containers
1. Make a copy of .env.example and rename it to .env. You may update the default values to suit your environment
2. Execute within the project directory:
```
docker-compose up
```
This will build the Docker image and run the app using Uvicorn

### Using The Service
After going through the setup instructions you should be able to access it locally on http://localhost:8000/docs/
