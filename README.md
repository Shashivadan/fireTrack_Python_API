markdown
# Predict Forest API Documentation

This API predicts forest fire likelihood based on temperature, oxygen levels, and humidity.

## Usage

### Endpoint

```
https://firetrack-python-api.onrender.com/predict_forest
```

### Request Parameters

- `temperature`: The temperature in Celsius.
- `oxygen`: The oxygen level in percentage.
- `humidity`: The humidity level in percentage.

### Example Request

```
GET /predict_forest?temperature=25&oxygen=18&humidity=60
```

### Example Response

```
{
  "temperature": 25,
  "oxygen": 18,
  "humidity": 60,
  "prediction": "Low"
}
```

### Response Parameters

- `temperature`: The temperature value from the request.
- `oxygen`: The oxygen value from the request.
- `humidity`: The humidity value from the request.
- `prediction`: The predicted fire likelihood categorized as "Low", "Medium", or "High".

## Setup

1. Clone the repository:

```bash
git clone <repository_url>
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the server:

```bash
python app.py
```

## Dependencies

- Python 3.x
- Fastapi
- scikit-learn (for prediction model)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

Replace `<repository_url>` with the actual URL of your repository. This README provides comprehensive documentation on how to use the API, set it up, its dependencies, and its license.
