# Dentifycare-Cloud-Computing

## Base URL  
**ML Deployment Documentation**  
[ML API Documentation](https://dentifycare-ml-api-363002036886.asia-southeast2.run.app/docs)

---

## Powered by Google Cloud Platform (GCP)  
<img src="https://github.com/Dentifycare/Dentifycare-Cloud-Computing/blob/main/Google_Cloud_logo.png" alt="GCP Logo" width="200"/>  

Google Cloud Platform (GCP) provides a suite of cloud computing services that allows us to build, deploy, and scale applications with ease. In this project, GCP enables us to handle machine learning models and APIs efficiently.

---

## Cloud Technologies Used  

### Cloud Storage  
<img src="https://github.com/Dentifycare/Dentifycare-Cloud-Computing/blob/main/Google-Storage.png" alt="Cloud Storage Logo" width="200"/>  

Cloud Storage is used to store the machine learning model files securely and reliably.  
#### Steps to Use Cloud Storage:  
1. Upload the pre-trained ML model files (e.g., `.h5` or `.pkl`) to a GCP Cloud Storage bucket.  
2. Set the appropriate access permissions for the bucket (e.g., grant access to Cloud Run or authorized users).  
3. Use the GCP storage URL to access the models during deployment or runtime.  

---

### Cloud Build  
<img src="https://github.com/Dentifycare/Dentifycare-Cloud-Computing/blob/main/Cloud-build.png" alt="Cloud Build Logo" width="200"/>  

Cloud Build automates the building and packaging of the ML model and API into Docker containers.  
#### Steps to Deploy with Cloud Build:  
1. Write a `Dockerfile` defining the environment and dependencies for the ML model and API.  
2. Push the source code and `Dockerfile` to a Git repository (e.g., GitHub).  
3. Trigger a build in Cloud Build by connecting the repository and configuring a `cloudbuild.yaml` file.  
4. Cloud Build generates a Docker image and pushes it to the Container Registry.  

---

### Cloud Run  
<img src="https://github.com/Dentifycare/Dentifycare-Cloud-Computing/blob/main/Cloud-run.png" alt="Cloud Run Logo" width="200"/>  

Cloud Run is used to deploy and run the machine learning API as a scalable, serverless container.  
#### Steps to Deploy on Cloud Run:  
1. Select the Docker image created by Cloud Build from the Container Registry.  
2. Deploy the image to Cloud Run, specifying required resources (e.g., memory, CPU) and environment variables.  
3. Configure the endpoint to allow authorized access or public access if necessary.  
4. Test the API by accessing the provided Cloud Run URL or Base URL.  

---

This documentation provides a comprehensive overview of how **Cloud Storage**, **Cloud Build**, and **Cloud Run** are utilized to deploy and manage our ML models and APIs effectively using GCP services.
