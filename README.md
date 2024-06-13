# image_analysis_with_microsoft_azure
Here by providing key and endpoint from microsoft azure services by creating the azure ai serices resource we can analyze the image as Object in the image,People in the image,Removing background and forground matting.
Image Analysis with Azure AI Vision
This project demonstrates how to use Azure AI Vision to analyze images. It includes functionality for extracting captions, dense captions, tags, objects, and people from images, as well as removing backgrounds or generating foreground mattes.

Prerequisites
Before you begin, ensure you have the following installed:

Python 3.6 or later
Azure account with AI Vision subscription
dotenv, Pillow, matplotlib, requests packages
.env file with Azure AI Vision endpoint and key
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Create a .env file in the root directory of your project and add your Azure AI Vision endpoint and key:

plaintext
Copy code
AI_SERVICE_ENDPOINT=your_endpoint
AI_SERVICE_KEY=your_key
Usage
To analyze an image, run the following command:

bash
Copy code
python image-analysis.py path/to/your/image.jpg
Features
Analyze Image: Extracts captions, dense captions, tags, objects, and people from the specified image.
Background Removal: Removes the background from the specified image or generates a foreground matte.
Functions
main(): The main function that sets up configuration, authenticates the Azure AI Vision client, and calls other functions to analyze the image and remove the background.
AnalyzeImage(image_filename, image_data, result): Analyzes the image and prints captions, dense captions, tags, objects, and people detected in the image.
BackgroundForeground(endpoint, key, image_file): Removes the background from the image or generates a foreground matte.
Example
To run the example provided in the repository:

Download or clone the repository.
Navigate to the directory containing the script.
Ensure you have an image file named street.jpg in the images directory or specify your own image path.
Run the script:
bash
Copy code
python image-analysis.py images/street.jpg
Output
The script will print the analysis results in the console.
Annotated images showing detected objects and people will be saved as objects.jpg and people.jpg respectively.
The background removed or foreground matte image will be saved as backgroundForeground.png.
Dependencies
dotenv
os
PIL
sys
matplotlib
azure-core
azure-ai-vision
requests
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Azure AI Vision
