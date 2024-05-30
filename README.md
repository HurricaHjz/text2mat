# text2mat
Code for the paper "Generating Parametric BRDFs from Natural Language Descriptions" https://arxiv.org/abs/2306.15679

# Create a new conda virtual environment with Python 3.8 (feel free to use any tool you like)
conda create --name myenv python=3.8
conda activate comp4610
# Solve pip version issue
pip install setuptools==65.5.0 pip==21  # gym 0.21 installation is broken with more recent versions
pip install wheel==0.38.0
# Install all requirements
pip install -r requirements.txt
pip install -r requirements.txt --use-deprecated=legacy-resolver

# If any error occurs, install PyTorch with CUDA 11.3 support explicitly
pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/torch_stable.html
# build aim server
aim init --repo logs
pip install protobuf==3.20.*


 pip install -U 'mlflow>=1.0.0'
