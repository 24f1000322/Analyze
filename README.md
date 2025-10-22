# Sales Performance Dashboard

This project provides a complete, functional single-page web application (SPA) to visualize sales data. It leverages a Python script to process raw sales data, a GitHub Actions workflow to automate data processing and deployment, and a simple HTML/CSS/JavaScript frontend to display the results.

## Project Summary

The core idea is to process sales data from an Excel file (`data.xlsx`), generate a `result.json` file containing key performance indicators (KPIs), and then publish this JSON file via GitHub Pages. A single-page application (`index.html`) then fetches this `result.json` and presents the sales analytics in an intuitive and professional dashboard.

**Key Features:**

*   **Automated Data Processing**: `execute.py` processes sales data to calculate total sales by product line, average unit price, total revenue by city, and identifies top performers.
*   **CI/CD Pipeline**: A GitHub Actions workflow (`ci.yml`) lints the Python code using `ruff`, executes `execute.py`, and publishes the generated `result.json` and `index.html` to GitHub Pages.
*   **Interactive Dashboard**: `index.html` provides a responsive dashboard using Bootstrap 5, fetching data from the published `result.json` and displaying it in tables and summary cards.
*   **Clean Architecture**: Separation of concerns between data processing (Python), deployment automation (GitHub Actions), and frontend visualization (HTML/CSS/JS).

## Setup Instructions

To set up and run this project locally or understand its components, follow these steps:

### Prerequisites

*   Python 3.11+
*   `pip` (Python package installer)
*   `git` (for cloning the repository)

### Local Environment Setup

1.  **Clone the Repository**: