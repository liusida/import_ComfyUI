【[EN](README.md)】

# 导入 ComfyUI 作为 Python 库

ComfyUI 是一个高效的 VRAM 管理工具。本仓库提供了在 Python 环境和 Jupyter 笔记本中设置和使用 ComfyUI 的说明。

ComfyUI 可以显著减少运行模型所需的 VRAM。例如，原版 Stable Diffusion v1 在 [RunwayML's stable-diffusion 仓库](https://github.com/runwayml/stable-diffusion) 中至少需要 10GB VRAM。而使用 ComfyUI，只需 1GB VRAM 即可运行。让我们设置环境并试试吧！

## 设置

### 第一步：克隆 ComfyUI 仓库
```bash
cd lib
git clone https://github.com/comfyanonymous/ComfyUI.git
cd ..
```

### 第二步：创建并激活虚拟环境
```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1 # Windows Powershell
./.venv/bin/activate # Linux
```

### 第三步：安装依赖
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121 # 在 Windows 上手动安装 pytorch
pip install -r ./lib/ComfyUI/requirements.txt
pip install -r ./requirements.txt
```

## 使用

### Python 代码
```
python example.py
```

### Jupyter notebook
```
jupyter notebook example.ipynb
```

## 许可证 License

由于 ComfyUI 采用 GPL-v3 许可证，如果您在项目中导入 ComfyUI，则必须使用 GPL-v3 许可证。

详情请访问: https://github.com/comfyanonymous/ComfyUI/blob/master/LICENSE
