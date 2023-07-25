## Virtual environment setup
`py -0p`: List Python versions on your computer </br>
`py -3.11 -m venv venv`: Make a virtual environment with Python version 3.11 </br>

## How to run the Dockerfile locally
`docker build -t rest-apis-flask-python .`: Builds Docker image </br>
`docker run -d -p 5000:5000 rest-apis-flask-python`: Run the container </br>
`docker run -dp 5000:5000 -w /app -v "/c/Alv/python-flask-course:/app" IMAGE_NAME sh -c "flask run --host 0.0.0.0"`: Hot reloading with volume </br>

## DB migration
`flask db init`: Creates migrations/ folder to track changes to our database </br>
`flask db migrate`: Create migration file including difference between models in code and database </br>
`flask db upgrade`: Go from current migration to the latest one </br>