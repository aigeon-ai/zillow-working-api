# Aigeon AI Zillow Working API

## Project Description

The **Aigeon AI Zillow Working API** is a Python-based server application designed to interact with the Zillow API through RapidAPI. This application provides a set of tools to access and retrieve real estate data from Zillow, enabling users to search for properties by various criteria such as property address, ZPID, Zillow URL, and more. It also supports advanced search functionalities, including autocomplete suggestions and detailed property listings based on user-defined filters.

## Features Overview

- **Property Search by Address**: Retrieve property details using a specific address.
- **Property Search by ZPID**: Access property information using Zillow's unique property identifier (ZPID).
- **Property Search by Zillow URL**: Fetch property details directly from a Zillow URL.
- **Autocomplete Suggestions**: Provide search box autocomplete data for better user experience.
- **Advanced Property Search**: Perform comprehensive property searches with multiple filtering options such as location, listing status, price range, and more.

## Main Features and Functionality

1. **By Property Address**: 
   - Allows users to input a property address and retrieve its corresponding ZPID and detailed property information with high accuracy.

2. **By ZPID**:
   - Enables users to fetch detailed property data using the Zillow Property ID (ZPID). This is useful for users who have the ZPID from a Zillow URL.

3. **By Zillow URL**:
   - Users can input a Zillow URL to obtain property details directly, simplifying the process of accessing property information.

4. **Autocomplete**:
   - Provides suggestions for search queries, enhancing user experience by offering relevant autocomplete options based on partial input.

5. **Search By Address**:
   - A sophisticated search tool that allows users to search for properties using various criteria such as location, listing status (For Sale, For Rent, Sold), price range, number of bedrooms, and more. This feature supports pagination and sorting to refine search results.

## API Endpoints / Main Functions Description

### 1. `by_property_address(propertyaddress: str) -> dict`
- **Description**: Retrieves property details using a given property address.
- **Input**: A string representing the property address (e.g., "3 W Forest Dr, Rochester, NY 14624").
- **Output**: A dictionary containing detailed property information.

### 2. `by_zpid(zpid: str) -> dict`
- **Description**: Fetches property details using the Zillow Property ID (ZPID).
- **Input**: A string representing the ZPID (e.g., "30907787").
- **Output**: A dictionary with property details.

### 3. `by_zillow_url(url: str) -> dict`
- **Description**: Obtains property information from a Zillow URL.
- **Input**: A string representing the Zillow URL (e.g., "https://www.zillow.com/homedetails/3-W-Forest-Dr-Rochester-NY-14624/30907787_zpid/").
- **Output**: A dictionary containing property details.

### 4. `autocomplete(query: str) -> dict`
- **Description**: Provides autocomplete suggestions for search queries.
- **Input**: A string representing the search query.
- **Output**: A dictionary with autocomplete suggestions.

### 5. `search_byaddress(...) -> dict`
- **Description**: Performs an advanced search for properties based on multiple criteria.
- **Inputs**: 
  - `location`: Address, neighborhood, city, or ZIP code.
  - `listingStatus`: Type of property data (For Sale, For Rent, Sold).
  - `page`: Pagination for results.
  - `sortOrder`: Sorting preference for search results.
  - Additional filters such as `listPriceRange`, `monthlyPayment`, `bed_min`, `bed_max`, etc.
- **Output**: A dictionary with search results containing property listings.

This application leverages the power of the Zillow API to provide comprehensive real estate data, making it a valuable tool for developers and users interested in accessing property information programmatically.