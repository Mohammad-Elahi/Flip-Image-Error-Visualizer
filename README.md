# [Visualize Rendered Image Errors with Flip](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip)
![Flip_Result](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/b3b5bbd1-3425-4dca-a1e4-9948c395d313)

# Description
This project uses the [Flip](https://github.com/NVlabs/flip) tool from [NVlabs](https://github.com/NVlabs) to visualize rendered image errors. With Flip, we can easily compare two images and visualize the differences, which is particularly useful in rendering, where detecting subtle differences can be challenging.

## license
This project uses the [Flip](https://github.com/NVlabs/flip) tool by [NVlabs](https://github.com/NVlabs), which is licensed under the BSD 3-Clause License. Please see the [original repository](https://github.com/NVlabs/flip) for more details.

## Getting Started

These instructions will guide you on how to set up and use the Flip tool.

### Prerequisites

- Python 3.12.2 
- OpenCV 
- Conda 

### Setup
1. **Download the repository** 

2. In the Flip folder, create **Reference_image and Test_image folders** and put your images in them.

3. **Open VSCode and create a new Python file**.

4. **Clone the Flip repository**:
    - Open a terminal in VSCode (Ctrl+` ).
    - Clone the Flip repository from GitHub to your local machine using the command: 
```
git clone https://github.com/NVlabs/flip.git
```
Navigate to the Python directory in the cloned repository: 
```
cd flip/python
```
5. **Setup Python Interpreter**:
    - Press Ctrl+Shift+P to open the Command Palette.
    - Type "Python: Select Interpreter" and select Python 3.12.2('flip') Conda.

6. **Install OpenCV**:
    - In the same terminal, type the following command and press Enter to install OpenCV: 
```
conda install -c conda-forge opencv
```
Check if OpenCV is successfully installed by typing the following commands in the terminal and pressing Enter:
```
python 
import cv2 as cv
```
If OpenCV is installed correctly, these commands should not return any errors.

7. **Navigate to the Flip directory**:
    - Navigate to the python directory in the Flip repository (the directory where you cloned the Flip repository) by typing the following command in the terminal and pressing Enter: 
```
cd path_to_flip_directory\flip\python
```
Replace `path_to_flip_directory` with the actual path to the Flip directory.

8. **Activate the Flip environment** before using the tool: 
```
conda activate flip
```
9. **Use the Tool**:
You can use the Flip tool with the following command: 
```python
python flip.py --reference “your_Reference_folder_path”  --test “your_Test_folder_path”
```
Replace `your_Reference_image_folder_path` and `your_Test_image_folder_path` with the paths to your reference and test images folder, respectively.

**Note**: You should path to your directory with using "/" like:
```
python flip.py --reference "C:/Users/mohammad.elahi/flip/Test_image/0050shot.png" --test "C:/Users/mohammad.elahi/flip/Reference_image/0033shot.png"
```
**Note**: The image result of the error map will be saved to the Flip folder path: flip\python


# Author
Mohammad Elahi, TU Dresden, Vodafone Chair, mohammad.elahi@mailbox.tu-dresden.de

![Flip_Result2](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/3090ae56-df57-40a9-95c1-aadba4be7b03)

