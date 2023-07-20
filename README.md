The GFPGAN algorithm leverages rich priors learned from a pretrained face GAN to restore faces, even in challenging conditions. It can enhance low-quality, low-resolution, or damaged face images by generating high-quality, realistic facial detailsThe algorithm is available as an open-source project on GitHub.

Version	   Model Name	    Description
V1.3	GFPGANv1.3.pth	     Based on V1.2; more natural restoration results; 
                             better results on very low-quality / high-quality inputs.




You can install our requirement.txt file using a ;
pip install -r requirements.txt

Dependencies and Installation
Python >= 3.7 (Recommend to use Anaconda or Miniconda)
PyTorch >= 1.7
Option: NVIDIA GPU + CUDA

Installation
Clone repo

git clone https://github.com/TencentARC/GFPGAN.git
cd GFPGAN
Install dependent packages

# Install basicsr - https://github.com/xinntao/BasicSR
# We use BasicSR for both training and inference
pip install basicsr

# Install facexlib - https://github.com/xinntao/facexlib
# We use face detection and face restoration helper in the facexlib package
pip install facexlib
python setup.py develop

# If you want to enhance the background (non-face) regions with Real-ESRGAN,
# you also need to install the realesrgan package
pip install realesrgan



## License
http://www.apache.org/licenses/
