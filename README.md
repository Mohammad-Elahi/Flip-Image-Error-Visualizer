# [Visualize Rendered Image Errors with Flip](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip)
![Flip_Result](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/b3b5bbd1-3425-4dca-a1e4-9948c395d313)

## Description
This project uses the [Flip](https://github.com/NVlabs/flip) tool from [NVlabs](https://github.com/NVlabs) to visualize rendered image errors. With Flip, we can easily compare two images and visualize the differences, which is particularly useful in rendering, where detecting subtle differences can be challenging.

## License
This project uses the [Flip](https://github.com/NVlabs/flip) tool by NVlabs, which is licensed under the BSD 3-Clause License. Please see the original repository for more details.

## Getting Started

These instructions will guide you on how to set up and use the Flip tool using the source code provided in this repository.

### Prerequisites
- [Conda](https://docs.conda.io/en/latest/miniconda.html) or Anaconda installed on your system.

### Installation & Setup

**1. Clone this repository**
Open a terminal and run the following commands:
```sh
git clone https://github.com/Mohammad-Elahi/Flip-Image-Error-Visualizer.git
cd Flip-Image-Error-Visualizer
```

**2. Create and Activate the Conda Environment**
We will create an environment specifically for this project with Python 3.12:
```sh
conda create -n flip python=3.12.2 -y
conda activate flip
```

**3. Install Dependencies**
Install OpenCV via Conda forge:
```sh
conda install -c conda-forge opencv -y
```

### Usage

We have already included sample directories (`Reference_image/` and `Test_image/`) inside this repository. You can place your own images in these folders.

To generate the error map between a test image and a reference image, navigate to the `python` directory and run the `flip.py` script:

```sh
cd python
python flip.py --reference "../Reference_image/your_reference_image.png" --test "../Test_image/your_test_image.png"
```

*Note: Ensure you replace `your_reference_image.png` and `your_test_image.png` with the actual file names of your images.*

The resulting error map will be saved in the `python/` folder by default.

## Author
**Mohammad Elahi**  
Research Assistant at Vodafone Chair for Mobile Communications Systems, TU Dresden  
mohammad.elahi@mailbox.tu-dresden.de

![Flip_Result2](https://github.com/Mohammad-Elahi/Visualize-rendered-image-errors-with-Flip/assets/93424032/3090ae56-df57-40a9-95c1-aadba4be7b03)
