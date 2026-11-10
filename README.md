# Nexlevr Internship – Beginner Task 1: Public API Integration

**Organization:** [Nexlevr](https://github.com/Nexlevr)  
**Internship Track:** Beginner  
**Task:** 1 of 3 – Call a Public API  
**API:** Open Food Facts  
**Tool:** Postman  
**Status:** Completed

## About the Internship

This project is part of the Nexlevr internship program, which includes Beginner, Intermediate, and Advanced task tracks.

This repository documents my work on the Beginner-level task, focusing on REST API fundamentals, API testing, and documentation using Postman.

## Project Overview

The objective was to connect to a free public API useful for business applications, make real API requests using Postman, document every request and response, and publish the collection.

For this task, I selected the **Open Food Facts API**, a public product catalogue that provides information about food products worldwide.

## Objectives

- Understand and interact with a REST API.
- Configure HTTP requests, query parameters, and headers.
- Retrieve and analyze JSON responses.
- Document API requests and actual response examples.
- Implement automated tests using Postman.
- Publish a reusable API collection.

## API Information

| Property | Details |
|---|---|
| API | Open Food Facts |
| Base URL | `https://world.openfoodfacts.org` |
| Authentication | Not required |
| Response format | JSON |
| HTTP methods used | GET |

**Official Documentation:** https://openfoodfacts.github.io/openfoodfacts-server/api/

## Implemented API Requests

### 1. Get Product by Barcode

**Method:** GET

**Endpoint:** `/api/v2/product/{barcode}.json`

**Example barcode:** `6132500711033`

Retrieves product information using its barcode.

**Business Use Case:** Retailers can use barcode lookups to retrieve product names, brands, quantities, and other product information.

### 2. Search Products

**Method:** GET

**Endpoint:** `/cgi/search.pl`

**Query Parameters:**
- `search_terms`: Product keyword to search for.
- `json`: Set to `1` to request a JSON response.
- `page_size`: Maximum number of products returned.

**Example search:** Nutella

**Business Use Case:** E-commerce applications can search product catalogues and display matching products to customers.

### 3. Get Products by Category

**Method:** GET

**Endpoint:** `/api/v2/search`

**Query Parameters:**
- `categories_tags_en`: Category used to filter products (e.g., `beverages`).
- `page_size`: Maximum number of products returned.
- `fields`: Specifies which product attributes to retrieve.

**Header:**
- `User-Agent`: Identifies the application making the API request.

**Business Use Case:** Retailers can filter and organize products by category to improve catalogue management and product discovery.

## Testing and Documentation

The Postman collection includes:

- Documented endpoints and HTTP methods.
- Configured query parameters and request headers.
- Actual API response examples.
- Automated tests to validate HTTP status codes and response structure.

## Postman Collection

**Published Documentation:** https://documenter.getpostman.com/view/58962353/2sBYHYveEP

**Exported Collection:** `open-food-facts.postman_collection.json`

## Technologies and Tools

- Postman
- REST API
- HTTP
- JSON
- JavaScript (Postman Tests)
- Open Food Facts API

---

**Nexlevr Internship – Beginner Track | Task 1 of 3**
