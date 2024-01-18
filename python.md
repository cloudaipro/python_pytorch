**install tensorflow**
```
pip install "tensorflow[and-cuda]"
```

```
if __name__ == __main__: #this test defines the test block  
  <block of statements>
```  
    The key is the first line, which checks the value of the built-in variable  __name__. This string variable is automatically created and is always de-  fined when Python runs. (Try putting print(__name__) inside one of your  programs or type it in an interactive session.) Inside an imported module,  __name__ holds the name of the module, whereas in the main program its  value is "__main__".  

 ```
sudo apt-get install python3.9-venv
```
 ```
 !pip install albumentations==0.4.6
 ! git clone https://github.com/IsHYuhi/BEDSR-Net_A_Deep_Shadow_Removal_Network_from_a_Single_Document_Image.git
  ! gdown https://drive.google.com/file/d/1RShxL-qcda08plhzpHJo4AWTl1UxblOY
from google.colab import drive
drive.mount('/content/drive')
! unzip -u pretrained.zip && rm pretrained.zip

! ls
cd BEDSR-Net_A_Deep_Shadow_Removal_Network_from_a_Single_Document_Image
```

```
python -W ignore foo.py
```

**How do I revert to a previous package in Anaconda?**
```
conda list --revisions
conda install --revision [revision number]
```

```
python -m site

pip3 list --user
```

```
brew install python@3.8
python3.8 -m venv coreml
source coreml/bin/activate
```

**remove all currently installed packages**
```
pip freeze > remove.txt
pip uninstall -r remove.txt
#re-insatll all packages 
pip install -r requriement.txt
```
```
pip install torch==1.8.1 torchvision==0.10.0  -f https://download.pytorch.org/whl/torch_stable.html
pip install torchvision==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html
```
**install TA-lib**
```
In Ubuntu 22.04 I solved this issue by following these steps below;

(BTW it is also mentioned in the official page here )

Download ta-lib-0.4.0-src.tar.gz and put it to the directory where you are planning to install talib, lets' say "~/talib" open bash and skip to the directory that you just put the downloaded file cd ~/talib and;
tar -xzf ta-lib-0.4.0-src.tar.gz
cd ta-lib/
./configure --prefix=/usr
make
sudo make install
add necessary directories to the path. To do that;
Edit .bashrc in your home directory and add the following line: please remember to change PREFIX with your path to talib (~/talib/ta-lib/)

export TA_LIBRARY_PATH=$PREFIX/lib

export TA_INCLUDE_PATH=$PREFIX/include

pip install TA-Lib
Then it was installed successfully. Good luck!
```
