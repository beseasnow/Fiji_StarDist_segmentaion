# Fiji_StarDist_segmentaion
imageJ Fiji- install and use StarDist to do segmentation of nuclei H&amp;E and fluorescent image
## imageJ Fiji- install and use StarDist to do segmentation

## install Fiji to Application (note: must be in Application) https://imagej.net/software/fiji/
## for Macos M chip need TensorFlow install through terminal, software requirements macOS 10.12.6 or higher, Python3.9-3.12, pip version 19.0 or higher
## check python version
python3 --version
python3 -m pip --version

## install TensorFlow
pip install --upgrade pip # TensorFlow requires a recent version of pip
pip install tensorflow

## verify the installation
python3 -c "import tensorflow as tf; print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
## If a tensor is returned, you've installed TensorFlow successfully.

## open Fiji -Help - update... - manage update sites- search 'CSBDeep', 'StarDist', and 'TensorFlow' check all 3 - click apply and close - apply changes
![image](https://github.com/user-attachments/assets/78e45421-b616-49bc-a6ad-1b67a4c51085)
![image](https://github.com/user-attachments/assets/5baf817d-ee8b-4a17-8c0c-1f404b3cad45)


## from Fiji-Edit-options-TensorFlow... select TF1.12.0CPU
![image](https://github.com/user-attachments/assets/c244662f-4f38-44c7-935b-a1eded66cb34)

## quit imageJ and re-open
## drag HE image - plugins -select StarDist 2D
![image](https://github.com/user-attachments/assets/fb1e5c3f-ca6c-4053-9550-bdbb8a635a61)

## choose model and probability/score and overlap threshold then click OK
![image](https://github.com/user-attachments/assets/1ec7ce1e-94bb-4883-9ed4-dc6f4f24ca23)
