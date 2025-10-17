# MST++ Coding Implementation
## Description
- Hyperspectral image reconstruction based on RGB inputs
## Dataset
- CAVE Dataset[~400-450MB] is used for training the model. From the following link, it can be downloaded
- https://cave.cs.columbia.edu/old/databases/multispectral/zip/complete_ms_data.zip

## 📁 Project Structure

```
📁 your_folder/ 
├── 📁 .ipynb_checkpoints/
├── 📁 cave_dataset/
├── 📁 checkpoints/
├── 📁 results/
├── 📄 .gitignore
├── 📄 best_model.pth
├── 📄 README.md
└── 📄 index.ipynb
```
# Dependencies

This project uses the following Python packages and standard library modules. Install the third‑party packages with the pinned versions for reproducibility.

## Third‑party packages

- `matplotlib`==3.10.1  
- `numpy`==1.24.3  
- `scipy`==1.15.2  
- `opencv-python-headless`==4.8.1.78  
- `torch`==2.1.2+cu121  
- `torchaudio`==2.1.2+cu121  (if audio functionality is used alongside torch; otherwise omit)  
- `torchvision`==0.16.2+cu121  (if vision models/transforms are used; otherwise omit)  
- `Pillow`==11.1.0  
- `typing_extensions`==4.12.2  

Note: Torch submodules (torch.nn, torch.nn.functional, torch.optim, torch.utils.data, torch.optim.lr_scheduler) are included with the torch version above.

## Standard library modules

- `os`  
- `typing`  
- `warnings`  
- `time`  
- `pathlib (Path)`  
- `random`  
- `glob`  
- `math`  

## Example installation

Using pip:

```
pip install \
  matplotlib==3.10.1 \
  numpy==1.24.3 \
  scipy==1.15.2 \
  opencv-python-headless==4.8.1.78 \
  torch==2.1.2+cu121 \
  Pillow==11.1.0 \
  typing_extensions==4.12.2
```

If you also need the Torch vision/audio extras:

```
pip install torchvision==0.16.2+cu121 torchaudio==2.1.2+cu121
```

## Environment notes

- Ensure that the CUDA build of torch matches your system/CUDA runtime (listed above as +cu121). If running on CPU‑only, install the CPU build of torch and matching torchvision/torchaudio.  
- Standard library modules are bundled with Python and don’t require manual installation.
