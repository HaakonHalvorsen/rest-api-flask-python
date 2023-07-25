## Virtual environment setup
`py -0p`: List Python versions on your computer
`py -3.11 -m venv venv`: Make a virtual environment with Python version 3.11

## Docker setup
`docker build -t rest-apis-flask-python .`: Builds Docker image
`docker run -d -p 5000:5000 rest-apis-flask-python`: Run the container
`docker run -dp 5000:5000 -w /app -v "/c/Alv/python-flask-course:/app" rest-apis-flask-python`: Hot reloading with volume 

## DB migration
`flask db init`: Creates migrations/ folder to track changes to our database
`flask db migrate`: Create migration file including difference between models in code and database
`flask db upgrade`: Go from current migration to the latest one