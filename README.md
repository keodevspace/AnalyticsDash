# Analytics Dashboard

This repository showcases a full-stack application designed to collect, process, and visualize data from a backend system. It serves as a dashboard, demonstrating skills in data analysis, reporting, and building interactive user interfaces.

## About the Project

This project was developed to highlight my abilities in:

* **Data Analysis & ETL:** Implementing a custom ETL (Extract, Transform, Load) process to transform raw data into a structured format for analysis.
* **Database Query Optimization:** Designing a database schema and creating complex SQL queries (views, stored procedures) to efficiently generate reports.
* **Backend API Development:** Building a robust and performant RESTful API with ASP.NET Core to serve data to the frontend.
* **Frontend Visualization:** Creating a dynamic and interactive dashboard using Angular to present data in a clear, graphical format.
* **Full-Stack Development:** Demonstrating proficiency in integrating a backend API with a frontend application.

## Key Technologies

* **Backend:** ASP.NET Core with C#
* **Frontend:** Angular
* **Database:** SQL Server
* **Data Visualization:** Chart.js

## Project Structure

The solution is divided into two main projects:

* **`Analytics.Api`**: The backend API. It contains the ETL logic, which periodically fetches data from the source database, processes it, and stores the results in the `Analytics` database. It also provides a set of endpoints for the frontend to consume.
* **`Analytics.Frontend`**: The Angular application. This project is the user interface, which fetches data from the `Analytics.Api` and displays it in various charts and tables.

## Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

* [.NET SDK 8.0 or later](https://dotnet.microsoft.com/download)
* [Node.js and npm](https://nodejs.org/en/download/)
* [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/keodevspace/AnalyticsDashboard.git](https://github.com/keodevspace/AnalyticsDashboard.git)
    cd AnalyticsDashboard
    ```

2.  **Database Configuration**
    * Set up your `Analytics` database in SQL Server.
    * Update the connection string in `appsettings.json` in the `Analytics.Api` project.

3.  **Run the Backend**
    ```bash
    # In the Analytics.Api directory
    dotnet run
    ```
    The API will run, and the ETL process will begin.

4.  **Run the Frontend**
    ```bash
    # In the Analytics.Frontend directory
    npm install
    ng serve
    ```
    The Angular app will now be running.

### How to Use

The dashboard will be available at `http://localhost:4200` (or the port specified by Angular CLI). The charts and tables will populate with data fetched from your backend API.

## What I've Learned

* Designing a data pipeline from source to visualization.
* Writing complex SQL queries and optimizing a database for reporting.
* Creating a cohesive full-stack application from the ground up, highlighting both backend and frontend skills.
* Demonstrating the value of data analysis in a real-world scenario.
