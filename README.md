# AI Image Generation using Stable Diffusion (Google Collab)

This repository contains a Google Colab script for generating images using AI-powered Stable Diffusion models. The script utilizes the `diffusers` library from Hugging Face along with PyTorch to create high-quality images from text prompts.

## Features
- Uses **Stable Diffusion 2.1** for image generation
- Supports **custom prompts, image sizes, guidance scale, and seed** for reproducibility
- Saves generated images automatically
- Compatible with **Google Colab and local execution**
- Uses **GPU acceleration** for faster processing

## Installation
Before running the script, install the required dependencies:
```bash
!pip install --upgrade diffusers transformers accelerate torch bitsandbytes scipy safetensors xformers
```

## Usage
Run the script in **Google Colab** or locally using Python:
```bash
python generate_image.py --prompt "A boy in a red shirt eating pizza on a mountain" --width 1024 --height 1024 --guidance_scale 7.5 --save_path output/generated_image.png
```

### Arguments
| Argument | Description | Default |
|----------|-------------|---------|
| `--model_id` | Model ID to use for generation | `stabilityai/stable-diffusion-2-1` |
| `--prompt` | Text prompt for image generation | "boy in red shirt having pizza on mountain" |
| `--width` | Image width in pixels | 1024 |
| `--height` | Image height in pixels | 1024 |
| `--guidance_scale` | Strength of prompt guidance | 7.5 |
| `--seed` | Random seed for reproducibility | None |
| `--save_path` | Path to save generated image | `output/generated_image.png` |

## Running in Google Colab
To run the script in Google Colab:
1. Open the Colab notebook.
2. Install the dependencies using the provided `pip` command.
3. Run the script by executing the cells.

## Example Output

<img src="https://github.com/user-attachments/assets/3dd10b55-9784-4a3a-b4b9-5d58cfe3401c" width="400"/>


## Dependencies
- Python 3.x
- PyTorch
- diffusers
- transformers
- accelerate
- scipy
- PIL
- Matplotlib

## License
This project is licensed under the **MIT License**.

## Contributing
Feel free to open **issues** or submit **pull requests** if you want to improve this project!

## Contact
For any queries, reach out via sarthakk.arora1@gmail.com.

