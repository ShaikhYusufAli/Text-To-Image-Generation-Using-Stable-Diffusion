# Text-To-Image-Generation-Using-Stable-Diffusion
This project is intended to show the capability of Stable Diffusion, an advanced deep learning model designed for the sole intent of creating high-quality images based on user-supplied textual descriptions. The project entails several crucial steps, such as the development of a Python programming environment that is best suited for such an endeavor, the installation of all the libraries needed that will assist the process, the development of a comprehensive script that appropriately processes the text prompts supplied, and lastly, the development of images that are based on artificial intelligence techniques.

2. Project Setup
Step 1: Creating the Project Folder
To keep all files organized and structured for easy management.

🔹 Process:
Open Visual Studio Code (VS Code).
Create a new folder and name it TextToImage.
This folder will store the script, generated images, and required dependencies.

Step 2: Creating the Python Script
The script will contain the logic to interact with the AI model, take user input, and generate images.

🔹 Process:
Inside the TextToImage folder, create a new Python file:
texttoimg.py
This script will be responsible for handling text-to-image generation.

Step 3: Installing Required Libraries
The project relies on deep learning and diffusion models, which require specific dependencies.

🔹 Installation Steps:
Open a terminal in VS Code.
Install the required libraries:
*pip install torch,torchvision,torchaudio, Cuda and diffusers*
After installation, all dependencies will be ready for use.

Step 4: Implementing the Python Code
What does the script do?
Loads the Stable Diffusion model.
Takes user input (text prompt).
Processes the text and generates an image.
Saves the image and displays it.

Step 5: Running the Script
Running the script allows us to test the AI model and see the generated images.

🔹 Execution Steps:
Open VS Code and open a terminal.

Run the script using:
*python filename*

Enter a text description when prompted (e.g., "A girl having an apple").

The script will:
Process the text input.
Generate an image.
Save the image as a file (generated_image.png).
Display the image to the user.

*NOTES: If the generated image does not match the prompt, try:*
*Using a more specific text prompt.*
*Increasing num_inference_steps to improve quality.*
*Adjusting guidance_scale to ensure prompt accuracy.*

3. Challenges Faced
   
1. Library Installation Issues:
   
Some dependencies (torch, torchvision, diffusers) required large file downloads.
Version mismatches caused installation failures.
✅ Solution: Installed correct versions and ensured Python compatibility.

3. CUDA/GPU Availability Issues:
   
Running on a CPU was extremely slow, requiring GPU acceleration.
Systems without CUDA support had long processing times.
✅ Solution: Implemented a check for CUDA availability and optimized processing for CPU users.

4. Model Loading Errors:
   
The Stable Diffusion model had version conflicts and missing dependencies.
✅ Solution: Installed correct versions and handled errors using proper exception handling.

5. Image Not Matching the Prompt:
   
Issue: The generated image sometimes does not match the given text prompt.
✅ Solution:
Increased guidance_scale to 8-10 for more prompt accuracy.
Increased num_inference_steps for better image clarity.
Experimented with different prompt structures for more accurate outputs.

6. High Memory Consumption:
   
The model required high VRAM (GPU memory), causing crashes on low-end systems.
✅ Solution: Reduced inference steps and used lower-resolution image settings.

4. Outputs and Result
   
 Generated Image Example:
Below is an example of an AI-generated image based on a text prompt:
Prompt: "A girl having an apple"

![image](https://github.com/user-attachments/assets/186e98b6-ae29-446b-9cfd-10af5889d579)


File Name: generated_image.png
Location: Stored inside the TextToImage folder.

5. Conclusion
🚀 This project successfully demonstrates how AI models can generate images from text descriptions using Stable Diffusion.

🔹 Key Takeaways:
✔ Proper library management is crucial.
✔ GPU acceleration significantly improves performance.
✔ Error handling and optimizations are needed for smooth execution.

✅ Future Improvements:

Implement a GUI interface for better usability.
Allow batch processing for multiple images.
Optimize memory usage for low-end systems.
