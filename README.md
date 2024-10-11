# Car Recommendation System API

This project is a FastAPI-based web service that provides car recommendations based on a machine learning model. The system takes input data and predicts the best car options using a pre-trained model.

## Project Structure

- **app.py**: Main FastAPI application. This file contains the API routes and logic for serving predictions.
- **car-recommender.joblib**: A pre-trained machine learning model used to make car recommendations.
- **CarPrediction.ipynb**: Jupyter notebook containing exploratory data analysis and model training details.
- **cars.csv**: Dataset used for training the recommendation model.
- **CarUser.py**: Script responsible for handling user-related features, such as managing user inputs.
- **requirements.txt**: Contains all the dependencies required to run the project.
- **Fast_API/**: Project directory with additional code or configuration files.

## Requirements
To install the necessary dependencies, run

pip install -r requirements.txt 

## Running the Application

uvicorn app:app --reload 

Once the server is running, you can access the API documentation at **http://127.0.0.1:8000/docs** or **http://127.0.0.1:8000/redoc**.
Running the Application
To start the FastAPI server, run the following command:

## Car Recommendation Endpoint

- **URL**: /predict
- **Method**: POST
- **Description**: Accepts car feature inputs and returns a recommendation based on the trained model.
- **Input**: JSON data representing the car attributes for the recommendation.
- **Output**: JSON response with the recommended car.

## Model Training and Evaluation

For details on the model training process and evaluation metrics, check the **CarPrediction.ipynb** notebook.

## Dataset

The **cars.csv** file contains the dataset used to train the car recommendation model. This includes various car features such as brand, model, price, and more.

## License

This project is licensed under the MIT License.
