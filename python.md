if __name__ == __main__: #this test defines the test block  
  <block of statements>
  
    The key is the first line, which checks the value of the built-in variable  __name__. This string variable is automatically created and is always de-  fined when Python runs. (Try putting print(__name__) inside one of your  programs or type it in an interactive session.) Inside an imported module,  __name__ holds the name of the module, whereas in the main program its  value is "__main__".  
 
 
 !pip install albumentations==0.4.6
 ! git clone https://github.com/IsHYuhi/BEDSR-Net_A_Deep_Shadow_Removal_Network_from_a_Single_Document_Image.git
 
 
 ! gdown https://drive.google.com/file/d/1RShxL-qcda08plhzpHJo4AWTl1UxblOY
 
 from google.colab import drive
drive.mount('/content/drive')
! unzip -u pretrained.zip && rm pretrained.zip

! ls
cd BEDSR-Net_A_Deep_Shadow_Removal_Network_from_a_Single_Document_Image

python -W ignore foo.py

How do I revert to a previous package in Anaconda?
conda list --revisions
conda install --revision [revision number]

python -m site
 
pip3 list --user

brew install python@3.8
python3.8 -m venv coreml
source coreml/bin/activate


#remove all currently installed packages
pip freeze > remove.txt
pip uninstall -r remove.txt
#re-insatll all packages 
pip install -r requriement.txt

pip install torch==1.8.1 torchvision==0.10.0  -f https://download.pytorch.org/whl/torch_stable.html
pip install torchvision==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html