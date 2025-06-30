Project Report: The Smartest AI Nutrition Assistant

Project Title:
--------------
The Smartest AI Nutrition Assistant

Objective:
-----------
The objective of this project is to design and implement an AI-powered nutrition assistant 
that can understand user inputs via text or image and provide accurate food identification 
along with nutritional information. It aims to assist users in making informed dietary 
choices through real-time analysis.

Problem Statement:
-------------------
In today’s fast-paced world, many people struggle to track their nutrition accurately. 
Existing apps often require manual input and lack real-time recognition or intelligent 
suggestions. This project addresses the need for a smart, automated system that can 
recognize food from images and return reliable nutrition information.

Tools and Technologies Required:
----------------------------------
- Python 3.10+
- TensorFlow / Keras (MobileNetV2 for image classification)
- NumPy (image preprocessing)
- Requests (for API access)
- USDA FoodData Central API (for nutrition data)
- PIL / Keras image utilities (for image loading and manipulation)

Methodology:
-------------
The application operates in two modes: Text and Image. In text mode, users manually enter 
a food name, while in image mode, a food photo is analyzed using the MobileNetV2 model to 
predict the item. The food name is then used to fetch nutrition data from the USDA 
FoodData Central API. Top 3 predictions are shown for image input with a warning if model 
confidence is low.

System Workflow:
-----------------
1. User selects input mode (text or image).
2. If image mode is selected, the image is loaded and passed through MobileNetV2.
3. Top food predictions are displayed with confidence scores.
4. The predicted (or entered) food name is sent to the USDA API.
5. Nutrient data is fetched and shown to the user.

Code & Output:
---------------
Input - Text mode example:
User input: chicken

Output:
[Displayed nutrition facts for chicken such as calories, protein, fat, carbs]

Input - Image mode example:
Input image: pizza.jpg

Output:
Top 3 predictions with confidence scores (e.g., Pizza 85%, Flatbread 10%, Bread 5%)
Nutrition facts for predicted food displayed below.

Future Scope:
--------------
- Integrate voice input for hands-free interaction
- Use a custom-trained deep learning model for Indian and regional foods
- Deploy as a mobile/web app using Streamlit or Flask
- Include meal suggestions and diet plans based on user goals

Conclusion:
------------
This project successfully demonstrates how AI can be applied to simplify nutrition tracking. 
By using image recognition and real-time APIs, users receive instant and reliable nutritional 
information, paving the way for smarter dietary decisions.
