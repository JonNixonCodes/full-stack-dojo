# Simple Website

A simple web application.

## Built With

* HTML5
* CSS3
* JavaScript
* Python
* Flask
* Google App Engine

## Getting Started

### Prerequisites

* A text editor or IDE for coding.
* A web browser (e.g., Chrome, Firefox).

### Setup

1. Create a Python virtual environment.
2. Activate the Python virtual environment.
3. Install required Python packages in the virtual environment.
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
4. Deploy the application locally.
```bash
python main.py
```
5. Deploy the application using Google App Engine.
6. Open the application on a web browser.
```bash
gcloud app deploy
gcloud app browse
```
7. Disable the app on Google Cloud Console.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Learning Resources
- [GAE Guides | Build an app](https://cloud.google.com/appengine/docs/standard/python3/building-app/)