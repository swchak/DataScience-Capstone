# SpaceX Launch Data Science Analysis

A comprehensive data science capstone project that collects, analyzes, and visualizes SpaceX launch data with machine learning predictions for launch success. This project demonstrates end-to-end data science workflows including data collection, exploratory data analysis, SQL querying, geospatial analysis, and predictive modeling.

## Table of Contents

- [What the Project Does](#what-the-project-does)
- [Why It's Useful](#why-its-useful)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Usage](#usage)
- [Getting Help](#getting-help)
- [Contributing](#contributing)

## What the Project Does

This capstone project provides an end-to-end analysis of SpaceX launch missions, including:

- **Data Collection**: Gathering SpaceX launch data via REST APIs and web scraping
- **Data Wrangling**: Cleaning, transforming, and preparing data for analysis
- **Exploratory Data Analysis (EDA)**: Statistical analysis and visualization of launch patterns
- **SQL Analytics**: Database queries for launch site analysis and success metrics
- **Geospatial Analysis**: Mapping launch sites and analyzing location-based factors
- **Machine Learning**: Predictive models for launch success classification
- **Interactive Dashboard**: Plotly Dash application for exploring launch records and correlations

## Why It's Useful

This project is valuable for:

- **Learning Data Science Workflows**: See a complete example of how to approach a real-world data science problem from start to finish
- **SpaceX Launch Insights**: Understand factors affecting rocket launch success, payload capacity, and site performance
- **Interactive Visualization**: Explore launch data through an interactive web dashboard
- **Predictive Analytics**: Leverage machine learning models to predict launch outcomes
- **Reference Implementation**: Use as a template for similar data science capstone projects

## Getting Started

### Prerequisites

- Python 3.7+
- pip or conda package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/swchak/DataScience-Capstone.git
cd DataScience-Capstone
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install pandas dash plotly jupyter scikit-learn requests beautifulsoup4 sqlite3
```

### Quick Start

#### Running the Interactive Dashboard

To launch the SpaceX Dashboard web application:

```bash
python spacex-dash-app.py
```

The dashboard will be available at `http://127.0.0.1:8050/` and allows you to:
- Filter launch records by site
- View success/failure pie charts
- Explore payload vs. success correlations
- Adjust payload ranges with interactive sliders

#### Exploring the Analysis Notebooks

Open any of the Jupyter notebooks to explore different aspects of the analysis:

```bash
jupyter notebook
```

Key notebooks:
- `jupyter-labs-spacex-data-collection-api.ipynb` - Data collection via SpaceX API
- `jupyter-labs-webscraping.ipynb` - Web scraping launch data
- `labs-jupyter-spacex-Data wrangling.ipynb` - Data cleaning and preparation
- `jupyter-labs-eda-sql-coursera_sqllite.ipynb` - SQL queries and database analysis
- `lab_jupyter_launch_site_location.ipynb` - Geospatial analysis of launch sites
- `edadataviz.ipynb` - Exploratory data visualization
- `SpaceX_Machine Learning Prediction_Part_5.ipynb` - Machine learning model training and evaluation

## Project Structure

```
├── jupyter-labs-spacex-data-collection-api.ipynb  # REST API data collection
├── jupyter-labs-webscraping.ipynb                  # Web scraping implementation
├── labs-jupyter-spacex-Data wrangling.ipynb        # Data cleaning & transformation
├── jupyter-labs-eda-sql-coursera_sqllite.ipynb     # SQL analytics
├── lab_jupyter_launch_site_location.ipynb          # Geospatial analysis
├── edadataviz.ipynb                                # Exploratory visualization
├── SpaceX_Machine Learning Prediction_Part_5.ipynb # ML predictions
├── spacex-dash-app.py                              # Interactive Dash dashboard
├── dataset_part_1.csv                              # Processed launch data (part 1)
├── dataset_part_2.csv                              # Processed launch data (part 2)
├── dataset_part_3.csv                              # Processed launch data (part 3)
├── spacex_launch_dash.csv                          # Dashboard data source
├── spacex_web_scraped.csv                          # Web scraped data
├── my_data1.db                                     # SQLite database
├── ds-capstone-findings-report.pdf                 # Full analysis report
└── README.md                                        # This file
```

## Key Features

- **Multi-source Data Integration**: Combines API-based data, web scraping, and CSV sources
- **SQL Database Analysis**: SQLite-based querying for efficient data exploration
- **Interactive Dashboard**: Real-time filtering and visualization with Plotly Dash
- **Machine Learning Models**: Scikit-learn powered predictions for launch success
- **Comprehensive Analysis**: Statistical summaries, visualizations, and geospatial mapping
- **Reproducible Workflows**: Jupyter notebooks documenting every step

## Usage

### Data Sources

The project uses three main data sources:

1. **SpaceX REST API** - Official SpaceX API endpoint for launch records
2. **Web Scraping** - Wikipedia and other public sources for additional data
3. **CSV Files** - Pre-processed data for quick analysis

### Dashboard Features

The Dash application provides:

- **Site Dropdown**: Filter data by specific launch site or view all sites
- **Success Pie Chart**: Visualize success/failure rates by site
- **Payload Range Slider**: Filter launches by payload mass (0-10,000 kg)
- **Correlation Scatter Plot**: Explore relationships between payload and launch success

### Example: Dashboard Analysis

```python
# The dashboard automatically filters and updates visualizations
# Select a launch site to see site-specific success rates
# Adjust the payload slider to analyze payload impact on success
# Color coding shows different booster version categories
```

## Getting Help

### Documentation

- **Full Analysis Report**: See `ds-capstone-findings-report.pdf` for comprehensive findings
- **Jupyter Notebooks**: Each notebook contains markdown documentation and code comments
- **Code Comments**: Inline comments throughout explain key logic and decisions

### Common Issues

For troubleshooting and common questions:
- Check the Jupyter notebooks for data preprocessing steps
- Review the dashboard code in `spacex-dash-app.py` for implementation details
- Examine the CSV files to understand data structure and content

### Data Information

- **Payload Mass**: Measured in kilograms (kg)
- **Launch Class**: Binary outcome (1 = Success, 0 = Failure)
- **Booster Version Category**: Different rocket model versions
- **Launch Site**: SpaceX facility location

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

### Areas for Contribution

- Additional machine learning models and experiments
- Enhanced dashboard visualizations
- Extended geospatial analysis
- Performance optimizations for large datasets
- Documentation improvements
- New data sources or collection methods

## Author

Created as a data science capstone project by Swetha Chakravarthy

## License

This project is open source. Please check the LICENSE file for details.