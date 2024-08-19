# Clock App

A web application which shows the current time.

## Built With

* HTML5
* CSS3
* JavaScript

## Getting Started

### Prerequisites

* Google Cloud Platform billing project.
* A text editor or IDE for coding.
* A web browser (e.g., Chrome, Firefox).

### Setup

1. Update source files:
    * index.html
    * css/style.css
    * js/script.js
2. Create a Google Cloud Storage bucket.
```bash
gcloud storage buckets create gs://BUCKET_NAME \
--location=BUCKET_LOCATION \
--project=PROJECT_ID \
```
3. Upload source files into the Cloud Storage bucket.
```bash
gcloud storage cp -r css/ js/ *.html gs://BUCKET_NAME
```
4. Add IAM policy to allow all users Object Viewer role.
```bash
gcloud storage buckets add-iam-policy-binding gs://BUCKET_NAME --member='allUsers' --role='roles/storage.objectViewer'
```
5. Open the application on a web browser by navigating to the following URL: https://storage.googleapis.com/BUCKET_NAME/index.html
6. Delete the Google Cloud Storage bucket.
```bash
gcloud storage rm --recursive gs://BUCKET_NAME
```

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.