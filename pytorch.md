conda install pytorch torchvision torchaudio -c pytorch  
conda install accelerate -c conda-forge
conda install --channel conda-forge youtube-dl  
conda config --append channels conda-forge

torch.backends.mps.is_available()  
torch.device('mps')  
