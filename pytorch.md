conda install -c conda-forge opencv
conda install pytorch torchvision torchaudio -c pytorch
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia  
conda install accelerate -c conda-forge
conda install -c conda-forge pandas
conda install -c conda-forge wandb
conda install -c conda-forge albumentations
conda install grad-cam

pip install grad-cam

conda install --channel conda-forge youtube-dl  
conda config --append channels conda-forge

torch.backends.mps.is_available()  
torch.device('mps')  

python -c 'import torch; print(torch.cuda.is_available())'

conda config --describe channel_priority
conda config --add channels conda-forge
conda config --set channel_priority strict