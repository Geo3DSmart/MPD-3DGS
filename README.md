# MPD-GS: Mask-guided Point Densification for Gaussian Splatting


> **Abstract**


### 🔧 Installation

**1. Clone the Repository**

**Important**: This is a repository with submodules. Please clone it with the `--recursive` flag to ensure all submodules are downloaded correctly.

```bash
git clone https://github.com/hjh530/MPD-3DGS.git --recursive
```

**2. Set Up the Conda Environment**
```bash
conda env create -f environment.yml
conda activate MPD-3dgs
```

**3.Depth regularization**
We use the original 3DGS depth regularization method, which can be specifically referenced in the official [3DGS](https://github.com/graphdeco-inria/gaussian-splatting) documentation.

### 🚀 Running

**Datasets**
We follow the same dataset structure as the original Gaussian Splatting. You can use the provided data or place your own images in a folder under the `data/` directory and process them with COLMAP.

**Training**
The training script is very similar to the original implementation.
Example: Train on the 'garden' scene from the Mip-NeRF 360 dataset
```bash
python train.py -s data/mipnerf360/garden -d <path to depth maps>
```
**Evaluation**
```bash
python render.py -m output/<your_run_name>
```

### ✏️ Citation

### 🙏 Acknowledgements

This project is built upon the great work from [3DGS](https://github.com/graphdeco-inria/gaussian-splatting). We sincerely thank the authors for their excellent work. Our project also benefits from the following amazing open-source libraries: [AbsGS](https://github.com/TY424/AbsGS)), [2DGS](https://github.com/hbb1/2d-gaussian-splatting), [Pixel-GS](https://github.com/zhengzhang01/Pixel-GS), [mini-splatting2](https://github.com/fatPeter/mini-splatting2).

