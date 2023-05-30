# GenerativeAI
**Image Generation with Leap AI API**

This Jupyter Notebook demonstrates the process of generating images using the Leap AI API. The code interacts with the API to generate realistic images based on given prompts. The prompts provide high-level descriptions or concepts, and the API uses machine learning models to generate corresponding images.

**Prerequisites**

Before running this notebook, make sure you have the following dependencies installed:

requests: !pip install requests
IPython: !pip install IPython


**Configuration**

To use the Leap AI API, you need an API key. Replace the API_KEY variable in the code with your actual API key for authentication.


**Image Generation**

The code defines two functions: generate_image and get_inference_job. The generate_image function initiates the image generation process by making a POST request to the API, providing a model ID and a prompt. It retrieves the inference ID and the initial status of the inference job.

The get_inference_job function checks the status of the inference job by making a GET request to the API, providing the model ID and the inference ID. It retrieves the updated status and the generated images (if available).

The code calls the generate_image function with a specific model ID and a prompt describing the desired image. It then enters a loop that repeatedly checks the status of the inference job until it is finished.

Once the inference job is finished, the code retrieves the generated images using the get_inference_job function.

The code displays the generated images inline within the notebook using the IPython library.

**Modifying Prompts**

To generate different types of images, you can modify the prompts in the code. The prompts should provide descriptive and detailed descriptions or concepts related to the desired image. Feel free to experiment with various prompts to generate images based on your preferences.
