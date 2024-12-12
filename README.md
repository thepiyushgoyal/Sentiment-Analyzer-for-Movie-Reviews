# Sentiment Analyzer for Movie Reviews
## Overview
The Sentiment Analyzer for Movie Reviews is a web-based application built using FastAPI that predicts the sentiment of movie reviews as either Positive or Negative. It utilizes Natural Language Processing (NLP) techniques to analyze the text input and provide a quick and accurate sentiment classification.

## Features
* Text Input Analysis: Users can input movie reviews to analyze their sentiment.
* Sentiment Prediction: Predicts whether the review expresses a positive or negative sentiment.
* RESTful API: Exposes endpoints for integration with other applications or systems.
* Interactive Swagger UI: Provides an interactive interface to test the API endpoints.
## Tools and Technologies
* FastAPI: For building and hosting the API.
* NLP Techniques: Preprocessing and sentiment classification using a pre-trained model.
* JSON Responses: For easy integration with external systems.
## Endpoints
1. GET /
Description: Displays a simple index page or information about the API.
2. POST /predict
Parameters:
document (string): The text of the movie review to analyze.
### Response:
{
  "prediction": "Positive Review"
}
### Example Usage
#### Input:
Review: "Very fun to watch movie, love the comedy!"

API Request:
curl -X 'POST' \
  'http://127.0.0.1:5000/predict?document=Very%20fun%20to%20watch%20movie%2C%20love%20the%20comedy' \
  -H 'accept: application/json' \
  -d ''
#### API Response:
{
  "prediction": "Positive Review"
}
![Screenshot 2024-12-12 111023](https://github.com/user-attachments/assets/e0909794-9dc4-4fea-af1c-3b4bf50777ad) ![Screenshot 2024-12-12 111205](https://github.com/user-attachments/assets/63688a27-3ed9-4d23-8a49-0227a5d6ef5f)



## Objectives
* To build a reliable system for sentiment analysis using movie reviews.
* To gain hands-on experience with FastAPI and NLP techniques.
* To provide a lightweight, efficient API for sentiment classification.
## Future Enhancements
* Support for multi-class sentiment analysis (e.g., neutral, mixed).
* Integration with a database for storing review analytics.
* Deployment to cloud services for broader accessibility.
### How to Use
* Clone this repository.
* Install the required dependencies using:
* pip install -r requirements.txt
* Run the FastAPI server using:
* uvicorn main:app --reload
* Access the interactive API documentation at http://127.0.0.1:8000/docs.
