# Number Classification API

This is a Python-based API that classifies a given number and returns interesting mathematical properties along with a fun fact.

## Features
- Classifies a number based on its properties (prime, perfect, Armstrong, odd/even).
- Fetches a fun fact about the number from the Numbers API.
- Returns responses in JSON format.

## API Endpoint
- **Endpoint**: `GET /api/classify-number?number=<number>`
- **Example Request**: `GET /api/classify-number?number=200`
- **Example Response**:
  ```json
    {
        "digit_sum": 2,
        "fun_fact": "200 is the smallest number which can not be made prime by changing one of its digits.",
        "is_perfect": false,
        "is_prime": false,
        "number": 200,
        "properties": [
            "even"
        ]
    }
  ```

## Requirements
- Python 3.7 or higher
- Flask
- requests
- flask-cors

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/mumiaktech/NumberClassificationAPI.git
   cd NumberClassificationAPI
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Running the API
1. Start the Flask development server:
   ```bash
   python app.py
   ```
2. The API will be available at `http://127.0.0.1:5000`.

## Deployment
Deploy the API to a platform like [Render](https://render.com/), [Heroku](https://www.heroku.com/), or [PythonAnywhere](https://www.pythonanywhere.com/).

## Testing
Use tools like [Postman](https://www.postman.com/) or `curl` to test the API:
```bash
curl "https://number-classification-api-p0fs.onrender.com/api/classify-number?number=200"
```
