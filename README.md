# Visualize-rendered-image-errors-with-Flip

![Flip_Result](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/3d240d6c-316f-4dc3-ac92-4b563dc62f08)

# Description
This project uses the [Flip](https://github.com/NVlabs/flip) tool from [NVlabs](https://github.com/NVlabs) to visualize rendered image errors.

## license
This project uses the [Flip](https://github.com/NVlabs/flip) tool by [NVlabs](https://github.com/NVlabs), which is licensed under the BSD 3-Clause License. Please see the [original repository](https://github.com/NVlabs/flip) for more details.

## Getting Started

These instructions will guide you on how to set up and use the Flip tool.

### Prerequisites

- Python 3.12.2
- OpenCV
- Conda

### Setup
1. **Download the Flip repository** from [here](https://github.com/NVlabs/flip).

2. **Create Reference and Test folders** in the Flip folder and put your images in those.

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
3. **Setup Python Interpreter**:
    - Press Ctrl+Shift+P to open the Command Palette.
    - Type "Python: Select Interpreter" and select Python 3.12.2('flip') Conda.

4. **Install OpenCV**:
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

5. **Navigate to the Flip directory**:
    - Navigate to the python directory in the Flip repository (the directory where you cloned the Flip repository) by typing the following command in the terminal and pressing Enter: 
```
cd path_to_flip_directory\flip\python
```
Replace `path_to_flip_directory` with the actual path to the Flip directory.

6. **Activate the Flip environment** before using the tool: 
```
conda activate flip
```
7. **Use the Tool**:
You can use the Flip tool with the following command: 
```python
python flip.py --reference “your_Reference_folder_path”  --test “your_Test_folder_path”
```
Replace `your_Reference_image_folder_path` and `your_Test_image_folder_path` with the paths to your reference and test images folder, respectively.

**Note**: You should path to your directory with "/" like:
```
python flip.py --reference "C:/Users/mohammad.elahi/flip/Test_image/0050shot.png" --test "C:/Users/mohammad.elahi/flip/Reference_image/0033shot.png"
```
**Note**: The image result of the error map will be saved to the Flip folder path: flip\python


# Author
Mohammad Elahi, TU Dresden, Vodafone Chair, mohammad.elahi@mailbox.tu-dresden.de

![Flip_Result2](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/08f12be8-f1ae-4698-98b5-7ac8e30479bf)
