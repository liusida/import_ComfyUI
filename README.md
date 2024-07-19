# Import ComfyUI as if it is a Python library

ComfyUI is a highly efficient VRAM management tool. This repository provides instructions for setting up and using ComfyUI in a Python environment, specifically for Jupyter notebooks.

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
