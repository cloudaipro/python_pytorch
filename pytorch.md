conda install pytorch torchvision torchaudio -c pytorch  
conda install accelerate -c conda-forge
conda install -c conda-forge opencv
conda install -c conda-forge albumentations
conda install -c conda-forge pandas
pip install grad-cam

conda install --channel conda-forge youtube-dl  
conda config --append channels conda-forge

torch.backends.mps.is_available()  
torch.device('mps')  

python -c 'import torch; print(torch.cuda.is_available())'