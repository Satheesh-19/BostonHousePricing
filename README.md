# Boston House Pricing Prediction

A Flask-based web application to predict house prices using a machine learning model trained with scikit-learn. The application is containerized using Docker and deployed to Heroku with CI/CD configured through GitHub Actions.

---

## Features
- Predict house prices using a regression model.
- User-friendly web interface for input and output.
- API endpoint for programmatic predictions (`/predict_api`).
- Containerized using Docker for portability.
- Automated deployment to Heroku using GitHub Actions.

---

## Tech Stack
- **Backend Framework:** Flask
- **Machine Learning Libraries:** scikit-learn, pandas, numpy
- **Visualization:** matplotlib
- **Deployment Tools:** gunicorn, Docker, Heroku, GitHub Actions

---

## Directory Structure

```plaintext
.
├── app.py                 # Main Flask application
├── home.html              # HTML template for the web interface
├── regmodel.pkl           # Trained regression model
├── scaling.pkl            # Scaler used for data preprocessing
├── Dockerfile             # Docker configuration file
├── requirements.txt       # Python dependencies
├── main.yaml              # GitHub Actions workflow for CI/CD
├── README.md              # Project documentation

```

Setup and Installation
Prerequisites
1.Install Python (>= 3.9)
2.Install Docker
3.Install the Heroku CLI

Steps
1.Clone the Repository:
git clone <repository_url>
cd <repository_directory>

2.Create a Virtual Environment:
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

3.Install Dependencies:
pip install -r requirements.txt

4.Run the Application Locally:
python app.py
Access the app at http://127.0.0.1:5000.

5.Dockerize the Application Build and run the Docker container:
docker build -t boston-house-pricing .
docker run -p 5000:5000 boston-house-pricing

Deployment to Heroku
Steps
1.Log in to Heroku
heroku login

2.Create a Heroku App
heroku create <app-name>

3.Deploy the App Use GitHub Actions for automated deployment. Ensure your Heroku credentials (HEROKU_EMAIL, HEROKU_API_KEY, HEROKU_APP_NAME) are added as secrets in your GitHub repository settings.

4.Access the Application Visit: https://<app-name>.herokuapp.com


