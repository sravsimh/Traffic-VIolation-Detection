# Vechile Violation Detection and Challan Generation
this project is developed to detect traffic violations from a video feed and capture the number plate of the violater. i have used yolov5 for traffic violation detection and easyocr for license plate detection. the outcome of the project is to automatically generate a traffic challan without human intervention

this repositories include trained model on helmet detection named best_violation_detection.pt

it also includes license plate model on cars named as best_violation_detection.pt

the last file is of license plate model on bikes named as best_bike_plate.pt

# Model Workflow
1. The model detect violations using best_violation_detection.pt
2. Once the model detects violations it then uses license plate detection.
3. The car and bike license plate is cropped using these models and sent for character detection.
4. Using easyocr and tesseract we detect the characters and get the final output.
