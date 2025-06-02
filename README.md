# CI/CD Assignment 1 - Calculator Application

## Technology Used
- Python 3.9
- Docker
- GitHub Actions
- Pytest for testing

## Project Structure
```
.
├── src/
│   └── calculator.py
├── tests/
│   └── test_calculator.py
├── Dockerfile
├── requirements.txt
└── README.md
```

## Implementation Steps

1. Created a basic calculator application in Python
2. Implemented test cases using unittest
3. Created Dockerfile for containerization
4. Set up GitHub Actions workflow for CI pipeline

## CI Pipeline Implementation

The CI pipeline is implemented using GitHub Actions and consists of the following stages:

1. **Build Stage**
   - Sets up Python environment
   - Installs dependencies from requirements.txt

2. **Test Stage**
   - Runs unit tests using pytest
   - Generates test coverage report

3. **Container Stage**
   - Builds Docker image
   - Runs container
   - Verifies container functionality
   - Stops container

## How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run tests:
   ```bash
   python -m pytest tests/
   ```
4. Build and run Docker container:
   ```bash
   docker build -t calculator-app .
   docker run calculator-app
   ```

## Test Cases
The application includes the following test cases:
1. Addition operations
2. Subtraction operations
3. Multiplication operations
4. Division operations
5. Division by zero error handling 