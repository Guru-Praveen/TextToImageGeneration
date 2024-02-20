# TextToImageGeneration Using StableDiffusion
This repository contains a simple GUI application that allows users to generate images from textual prompts using a pre-trained Stable Diffusion model. The model is implemented using the diffusers library, and the GUI is built with the tkinter library.

## Configuration Class (CFG)
The CFG class holds configuration settings for the application:

device: The device to use for model inference (e.g., "cpu").
seed: Random seed for reproducibility.
generator: PyTorch random seed generator.
image_gen_steps: Number of inference steps for image generation.
image_gen_model_id: Model identifier for Stable Diffusion.
image_gen_size: Size of the generated image.
image_gen_guidance_scale: Guidance scale for the image generation model.
Model Initialization
The Stable Diffusion model is initialized using the StableDiffusionPipeline from the diffusers library. The model is loaded with pre-trained weights and configured with specified parameters.

## GUI Creation
A Tkinter window is created for the GUI with an input entry for the user to enter a textual prompt. A "Generate" button triggers the image generation process.

## Image Generation Function
The generate_image function is responsible for generating an image based on the entered text. It uses the Stable Diffusion model to produce an image, resizes it, and displays it on the Tkinter canvas.

## Tkinter Canvas
A canvas is used to display the generated image. The canvas is cleared before each generation to ensure only the latest image is displayed.

## Running the Application
The main event loop (window.mainloop()) runs the Tkinter application, allowing users to interact with the GUI.

## Acknowledgments
The application utilizes the Stable Diffusion model from Hugging Face's model hub.
