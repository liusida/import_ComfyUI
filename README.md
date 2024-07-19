【[中文](README.cn.md)】

# Import ComfyUI as if it is a Python library

ComfyUI is a highly efficient VRAM management tool. This repository provides instructions for setting up and using ComfyUI in a Python environment and Jupyter notebooks.

ComfyUI can significantly reduce the VRAM requirements for running models. For example, the original Stable Diffusion v1 at [RunwayML's stable-diffusion repository](https://github.com/runwayml/stable-diffusion) requires at least 10GB VRAM. With ComfyUI, you can run it with as little as 1GB VRAM. Let's set up the environment and give it a try!

## Setup

### Step 1: Clone the ComfyUI Repository
```
cd lib
git clone https://github.com/comfyanonymous/ComfyUI.git
cd ..
```

### Step 2: Create and Activate a Virtual Environment
```
python -m venv .venv
.\.venv\Scripts\Activate.ps1 # Windows Powershell
./.venv/bin/activate # Linux
```

### Step 3: Install Dependencies
```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121 # manually install pytorch on Windows
pip install -r ./lib/ComfyUI/requirements.txt
pip install -r ./requirements.txt
```

## Usage

### For Python code
```
python example.py
```

### For Jupyter notebook
```
jupyter notebook example.ipynb
```

## License

Since ComfyUI is under GPL-v3, if you import ComfyUI into your project, you are required to use the GPL-v3 License.

Please visit: https://github.com/comfyanonymous/ComfyUI/blob/master/LICENSE
