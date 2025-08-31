**Carbon Footprint Estimator**

A Spring Boot application that estimates the carbon footprint of dishes based on their name (text input) or an uploaded image filename (simplified).

This is a demo project showcasing how AI-powered estimation could be integrated into food sustainability apps.

**Running the Project**

Prerequisites:

Java 22+

Maven 3.9+
Run Locally
# Clone the repo
git clone https://github.com/your-username/carbon-footprint-estimator.git


cd carbon-footprint-estimator

# Build
mvn clean install

# Run
mvn spring-boot:run


App will start at http://localhost:8080

# API Endpoints

1. Estimate from Text
POST /api/carbon/text

Request:

json:

{

  "dishName": "chicken biryani"
  
}

Response:


<img width="1448" height="1068" alt="Screenshot 2025-08-31 092029" src="https://github.com/user-attachments/assets/396c74a3-b720-4767-8c01-bd891d831930" />


2. Estimate from Image
   
POST /api/carbon/image

Form-data:

file: image file (e.g., veg fried rice.png)

Response (filename-based mapping):

<img width="1449" height="1065" alt="Screenshot 2025-08-31 092008" src="https://github.com/user-attachments/assets/9aa4fd61-ee58-4efc-a49d-50a58b96dcc3" />

