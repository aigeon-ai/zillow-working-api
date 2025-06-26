# Aigeon AI Zillow Working API

## Project Overview

The **Aigeon AI Zillow Working API** is a Python-based server application designed to interact with the Zillow Working API. This project provides a set of tools to retrieve and manage real estate data from Zillow, offering functionalities such as fetching property details by address, ZPID, or Zillow URL, and performing property searches with various filters. The application leverages the FastMCP framework to streamline API interactions and ensure efficient data retrieval.

## Features Overview

- **Property Lookup by Address**: Retrieve detailed property information using a specific property address.
- **Property Lookup by ZPID**: Access property details using the unique Zillow Property ID (ZPID).
- **Property Lookup by Zillow URL**: Fetch property data directly from a Zillow URL.
- **Autocomplete Suggestions**: Obtain search box autocomplete data from Zillow for enhanced user experience.
- **Advanced Property Search**: Conduct comprehensive property searches with multiple filters, including location, listing status, price range, and more.

## Main Features and Functionality

1. **Property Lookup by Address**:
   - Allows users to input a property address to retrieve its corresponding ZPID and detailed property information.
   - Ensures high accuracy in matching addresses to property data.

2. **Property Lookup by ZPID**:
   - Enables users to fetch property details using the ZPID, a unique identifier found in Zillow URLs.
   - Provides a fallback to address-based lookup if the ZPID is unknown.

3. **Property Lookup by Zillow URL**:
   - Facilitates the retrieval of property information using a direct Zillow URL.
   - Simplifies the process of obtaining property data by leveraging existing Zillow links.

4. **Autocomplete Suggestions**:
   - Offers real-time autocomplete suggestions for search queries, enhancing the user interface and search efficiency.
   - Utilizes Zillow's autocomplete API to provide relevant suggestions based on user input.

5. **Advanced Property Search**:
   - Supports detailed property searches with a wide array of filters, including:
     - Location (address, neighborhood, city, ZIP code)
     - Listing status (For Sale, For Rent, Sold)
     - Price range and monthly payment options
     - Number of bedrooms and bathrooms
     - Home type and space preferences
     - HOA fees and listing types
   - Allows users to sort search results by various criteria, such as price, newest listings, and more.

## Main Functions Description

### `by_property_address(propertyaddress: str) -> dict`
- **Purpose**: Retrieve property details using a specific property address.
- **Input**: A string representing the property address.
- **Output**: A dictionary containing detailed property information.

### `by_zpid(zpid: str) -> dict`
- **Purpose**: Fetch property details using the Zillow Property ID (ZPID).
- **Input**: A string representing the ZPID.
- **Output**: A dictionary containing detailed property information.

### `by_zillow_url(url: str) -> dict`
- **Purpose**: Obtain property data using a direct Zillow URL.
- **Input**: A string representing the Zillow URL.
- **Output**: A dictionary containing detailed property information.

### `autocomplete(query: str) -> dict`
- **Purpose**: Provide autocomplete suggestions for search queries.
- **Input**: A string representing the search query.
- **Output**: A dictionary containing autocomplete suggestions.

### `search_byaddress(...) -> dict`
- **Purpose**: Conduct an advanced property search with multiple filters.
- **Input**: Various parameters including location, listing status, price range, and more.
- **Output**: A dictionary containing search results based on the provided filters.

This project is designed to facilitate seamless interaction with Zillow's real estate data, providing users with powerful tools to access and manage property information efficiently.