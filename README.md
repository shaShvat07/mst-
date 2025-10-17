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
    ├── 📁 balloons_ms/
         ├── 📁 balloons_ms/
              ├── 📄 baloons_ms_01.png
              ├── 📄 baloons_ms_02.png
              ............
              ├── 📄 baloons_RGB.bmp
├── 📁 checkpoints/
├── 📁 results/
├── 📄 .gitignore
├── 📄 best_model.pth
├── 📄 README.md
└── 📄 index.ipynb
```
# Dependencies

This project uses the following Python packages and standard library modules. Install the third‑party packages with the pinned versions for reproducibility.
- `python` verison == 3.11.11
  
## Third‑party packages

- `matplotlib`==3.10.1  
- `numpy`==1.24.3  
- `scipy`==1.15.2  
- `opencv-python-headless`==4.8.1.78  
- `torch`==2.1.2+cu121  
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

## Environment notes

- Ensure that the CUDA build of torch matches your system/CUDA runtime (listed above as +cu121). If running on CPU‑only, install the CPU build of torch and matching torchvision/torchaudio.  
- Standard library modules are bundled with Python and don’t require manual installation.

## Running the code

- First, clone the repository, open your terminal and hit `git clone https://github.com/shaShvat07/mst-.git`
- Then, download the `CAVE Dataset` from the above link provided. Place it and name it in your workspace as mentioned in the file structure.
- Delete the folder `watercolors_ms` folder from the `CAVE Dataset` as it was not consistent with other folder contents!
- Install the dependencies/packages as mentioned above using pip 
- After that, you can simply run the code in jupyter kernel one by one
- Lastly, after completing the training and inference process, the results are stored in `results` folder
