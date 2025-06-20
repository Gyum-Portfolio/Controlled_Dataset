# Controlled_Dataset
This repository contains the resources and results for a controlled dataset experiment investigating bias in large vision-language models (VLMs) when comparing real-world and synthetically generated images.

This script generates a synthetic image using OpenAI's DALL·E 3 model and saves it to the current directory. The image style is randomly selected from three predefined prompt templates.

## Requirements

- Python 3.7 or higher

### Install dependencies:

```bash
pip install openai requests pillow
```

### Get your OpenAI API key:

1. Visit https://platform.openai.com/account/api-keys
2. Create or copy an API key (starts with sk-...)

## How to Run

1. Save the Python script (e.g., generate_image.py)
2. Edit the script and replace this line:

```python
openai.api_key = "your_openai_api_key_here"
```

with your actual OpenAI API key:

```python
openai.api_key = "sk-..."
```

3. Run the script:

```bash
python generate_image.py
```

## Output

After running, the script will generate one synthetic image named:

```
synthetic_image.png
```

It will be saved in the same directory where the script is run.

## Prompt Styles Used

One of the following prompt styles is randomly selected during generation:

1. Draw Style:  
   Maximalist masterpiece, painted, acrylic painting, trending on pixiv fanbox, palette knife and brush strokes, style of Makoto Shinkai, Jamie Wyeth, James Gilleard, Edward Hopper, Greg Rutkowski, Studio Ghibli, Genshin Impact

2. Cinematic Photo Style:  
   Photo realistic, extreme detail, lifelike, crisp, precise, environmental, detailed, 35mm photograph, film, bokeh, professional, 4k, highly detailed

3. Cinematic Film Style:  
   Film grain, cinematic film still, shallow depth of field, highly detailed, high budget, cinemascope, moody, epic, overall detail, gorgeous, 2000s vintage Raw photo, photorealistic, candid camera, color graded cinematic, eye catchlights, atmospheric lighting, natural
