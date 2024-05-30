# text2mat
Code for the paper "Generating Parametric BRDFs from Natural Language Descriptions" https://arxiv.org/abs/2306.15679

# install omniverse and isaac 2022.1.1
# install vscode installer 2022 for windows, with windows 10 sdk

# format input, need to ensure use omniverse python env
C:\Users\jerry\AppData\Local\ov\pkg\isaac_sim-2022.1.1\python.bat -m pip ...

# Install all requirements
pip install -r requirements.txt
pip install -r requirements.txt --use-deprecated=legacy-resolver

<!-- # Solve pip version issue
pip install setuptools==65.5.0 pip==21  
pip install wheel==0.38.0 -->
<!-- # Install PyTorch with CUDA 11.3 support explicitly
pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/torch_stable.html -->

# build aim server
<!-- pip install protobuf==3.20.*
pip install -U 'mlflow>=1.0.0' -->

C:\Users\jerry\AppData\Local\ov\pkg\isaac_sim-2022.1.1\python.bat -m pip install chromadb==0.3.29
C:\Users\jerry\AppData\Local\ov\pkg\isaac_sim-2022.1.1\python.bat -m pip install lpips 
C:\Users\jerry\AppData\Local\ov\pkg\isaac_sim-2022.1.1\python.bat -m pip install --upgrade typing_extensions 
# build aim server
aim init --repo logs


$Env:INCLUDE = "C:\Program Files (x86)\Windows Kits\10\Include\10.0.20348.0\ucrt;C:\Program Files (x86)\Windows Kits\10\Include\10.0.20348.0\shared;C:\Program Files (x86)\Windows Kits\10\Include\10.0.20348.0\um;C:\Program Files (x86)\Windows Kits\10\Include\10.0.20348.0\winrt"
$Env:LIB = "C:\Program Files (x86)\Windows Kits\10\Lib\10.0.20348.0\ucrt\x64;C:\Program Files (x86)\Windows Kits\10\Lib\10.0.20348.0\um\x64"


$Env:PATH += ";C:\Program Files (x86)\Windows Kits\10\bin\10.0.20348.0\x86"


C:\Users\jerry\AppData\Local\ov\pkg\isaac_sim-2022.1.1\python.bat run.py -c scene_model


