# Country & Capital API

This is a straightforward API developed with Python and Flask, designed to provide the country name for a corresponding capital city.

---

## Project Overview

This service has a single purpose: to accept a capital city's name and return the country it belongs to. The repository holds all the necessary code for this microservice.

---

## Required Software

Before you begin, ensure you have the following installed:
* Python (version 3.8 or newer)
* The pip package installer

---

## Instructions for Local Setup

To get a copy of this project running on your own machine, please follow these steps.

1.  **Get the code:**
    ```bash
    git clone [https://github.com/your-username/country-capital-api.git](https://github.com/your-username/country-capital-api.git)
    cd country-capital-api
    ```

2.  **Set up a virtual environment (best practice):**
    ```bash
    # On macOS/Linux
    python3 -m venv .venv
    source .venv/bin/activate

    # On Windows
    python -m venv .venv
    .\.venv\Scripts\activate
    ```

3.  **Install project dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch the server:**
    This API is served by Uvicorn. Use this command to start it:
    ```bash
    uvicorn main:app --reload
    ```
    You can now access the API at `http://127.0.0.1:8000`.

---

## Using the API

We host a live instance of this service for internal organizational use.

**Service Endpoint:** `https://example.com/country-capital/`

To use it, send a GET request and include the city as a query parameter.

**cURL Example:**
```bash
curl "[https://example.com/country-capital/?city=Tokyo](https://example.com/country-capital/?city=Tokyo)"

Sample Response:

JSON

{
  "city": "Tokyo",
  "country": "Japan"
}