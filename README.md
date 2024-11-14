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
