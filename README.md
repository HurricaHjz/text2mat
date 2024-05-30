# text2mat
Code for the paper "Generating Parametric BRDFs from Natural Language Descriptions" https://arxiv.org/abs/2306.15679

# Create a new conda environment with Python 3.8
conda create --name myenv python=3.8

# Activate the environment
conda activate myenv
pip install setuptools==65.5.0 pip==21  # gym 0.21 installation is broken with more recent versions
pip install wheel==0.38.0

# Install PyTorch with CUDA 11.3 support
pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/torch_stable.html

