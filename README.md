# Understanding-Amazon-From-Sapce
This notebook was created to perform image classification for the competition Understanding Amazon from Space. A baseline CNN model, VGG-16 and Resnet50 were trained
to perform classification.

All the details are within the notebook and it is self-explanatory.
If someone wants to import the dataset directly into Google Colab without downloading it, please use the below commands in your colab notebook.

Go to kaggle.com and click on your photo on top right corner. Click on Account and scroll down to API. Click on 'Expire API Token', then click on 
'Create New API Token'. A json file will be downloaded. Next go to your Google Colab file and run the below commands.

! pip install -q kaggle

from google.colab import files

files.upload()

After this, you will need to upload the json file downloaded from Kaggle website

Make directory named kaggle and copy kaggle.json file there.
! mkdir ~/.kaggle

! cp kaggle.json ~/.kaggle/

Change the permissions of the file.
! chmod 600 ~/.kaggle/kaggle.json

! kaggle datasets download -d nikitarom/planets-dataset
! mkdir dataset
! unzip planets-dataset.zip -d dataset

In Google Colab, click on 'Files' icon on right-side. You'll see a folder named dataset which will have all your required files.
