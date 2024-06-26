README.md
markdown
Copy code
# Agriculture Analytics

This project is a simple React application that performs data analysis on an agriculture dataset and displays the results in tables. It uses TypeScript, React, and Mantine v7 for table rendering. The dataset is provided in JSON format.

## Features

- Fetches and processes agriculture data.
- Displays yearly aggregation of crop production.
- Displays average yield and cultivation area of crops between 1950-2020.

## Project Structure

agriculture-analytics/
├── public/
│ ├── agriculture_data.json # Dataset file
│ ├── index.html
│ └── ...
├── src/
│ ├── data/
│ │ └── dataAnalysis.ts # Data fetching and processing functions
│ ├── App.tsx # Main application component
│ ├── index.tsx # Entry point of the application
│ └── ...
├── .gitignore
├── package.json
├── README.md # Project documentation
├── tsconfig.json # TypeScript configuration
├── yarn.lock
└── ...

less
Copy code

## Getting Started

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/en/) (version 14.x or higher)
- [Yarn](https://yarnpkg.com/) (version 1.x or higher)

### Installation

1. **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd agriculture-analytics
    ```

2. **Install dependencies using Yarn:**

    ```bash
    yarn install
    ```

3. **Ensure the dataset is placed correctly:**

    The dataset file `agriculture_data.json` should be in the `public` directory. The structure should look like this:

    ```
    public/
    ├── agriculture_data.json
    ├── index.html
    └── ...
    ```

### Running the Application

To start the development server and run the application:

```bash
yarn start
This will start the application and open it in your default web browser. If it doesn't open automatically, navigate to http://localhost:3000 in your browser.

Data Analysis Functions
fetchData(url: string): Promise<CropData[]>

Fetches the dataset from the given URL.

aggregateData(data: CropData[]): { yearlyAggregation: YearlyAggregation[], cropAggregationArray: CropAggregation[] }

Processes the dataset to create two types of aggregations:

Yearly aggregation of crops with maximum and minimum production.
Average yield and cultivation area for each crop from 1950-2020.
Components
App.tsx

Main component that handles fetching and displaying data in tables.

Screenshots
Include screenshots of the final rendered tables in your README for clarity.

Example:



Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
