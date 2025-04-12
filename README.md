# Fuel Quality Analysis Project

## Project Overview
This project analyzes historical fuel quality data from Costa Rican service stations to develop predictive models that can automatically classify gasoline types and estimate octane numbers based on physical fuel characteristics. The goal is to create a more efficient and cost-effective method for fuel quality assessment compared to traditional laboratory testing.

## Business Problem

Fuel quality monitoring is essential for regulatory compliance and consumer protection in Costa Rica, where approximately 3.78 billion liters of fuel were consumed in 2023 alone. However, current methods face significant challenges:

- Traditional octane testing requires specialized laboratory equipment and expensive motor tests
- The regulatory authority (ARESEP) has limited resources to conduct widespread testing
- In 2023, 13 service stations failed to meet quality standards, highlighting the need for better monitoring

This project aims to develop predictive models that can:
1. Estimate octane numbers using easily measurable physical characteristics
2. Automatically classify fuels as regular or superior gasoline
3. Reduce economic costs associated with laboratory testing
4. Enable more stations to be evaluated in less time
5. Facilitate early identification of non-compliant stations

## Data Description

The dataset comes from ARESEP (Public Services Regulatory Authority of Costa Rica) and contains:
- 23,139 records spanning from 2013 to 2024
- 23 columns including fuel physical properties and quality measurements
- Three main fuel types: Gasolina Superior (Premium), Gasolina Regular, and Diésel
- Physical measurements such as:
  - Distillation curve parameters (10%, 50%, 90%, initial and final points)
  - Density, viscosity, and vapor pressure
  - Aromatics, sulfur, benzene, and olefin content
  - Octane number and cetane index

The data is complemented by inspection results indicating compliance with quality standards.

## Methodology

The project follows a comprehensive data science workflow:

1. **Data Acquisition and Integration**
   - Combining multiple CSV files from different time periods
   - Processing inspection results and quality measurements separately
   - Merging datasets using station codes and visit dates

2. **Data Cleaning and Preprocessing**
   - Converting date formats
   - Handling duplicates with different inspection results
   - Creating target variables for compliance by fuel type
   - Using regular expressions to extract non-compliance information

3. **Feature Engineering**
   - Transforming categorical variables
   - Analyzing relationships between physical properties and octane number
   - Preparing data for classification and regression models

4. **Model Development**
   - Implementing classification models to distinguish between fuel types
   - Building regression models to estimate octane numbers
   - Evaluating model performance using appropriate metrics

## Technologies Used

- **Python**: Primary programming language
- **Pandas & NumPy**: Data manipulation and numerical operations
- **Scikit-learn**: Machine learning model implementation and evaluation
- **Matplotlib & Seaborn**: Data visualization
- **PyTorch**: Neural network development
- **Regular Expressions**: Text processing for compliance information

## Skills Demonstrated

This project showcases several key data science competencies:

- **Data Integration**: Combining multiple datasets from different sources
- **Data Cleaning**: Handling duplicates, missing values, and inconsistent formats
- **Exploratory Data Analysis**: Understanding distributions and relationships
- **Feature Engineering**: Creating relevant features for modeling
- **Predictive Modeling**: Implementing classification and regression techniques
- **Domain Knowledge Application**: Applying understanding of fuel properties in analysis
- **Process Automation**: Creating reproducible workflows for ongoing analysis

## Potential Impact

The models developed in this project could significantly improve fuel quality monitoring in Costa Rica by:
- Reducing the cost and time required for testing
- Expanding testing coverage to more service stations
- Providing early warning of potential quality issues
- Creating a replicable, data-driven methodology for future monitoring

This approach demonstrates how data science can transform regulatory processes, making them more efficient while maintaining or improving their effectiveness.
