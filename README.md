# Shape Feature Extraction: Skeletonization and Medial Axis Transformation

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)

This project implements and explores various shape feature extraction techniques, focusing on skeletonization and medial axis transformation. These methods are essential for analyzing and processing binary images, particularly useful in computer vision and image processing applications.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Features](#features)
4. [Examples](#examples)
5. [Contributing](#contributing)
6. [License](#license)

## Installation

To run this project, you need to have Python installed along with several dependencies. You can install the required packages using pip:

```bash
pip install numpy matplotlib scikit-image opencv-python pillow scipy
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/shape-feature-extraction.git
   cd shape-feature-extraction
   ```

2. Run the Jupyter notebook:
   ```bash
   jupyter notebook "Explore Skeletonization.ipynb"
   ```

3. Follow the instructions in the notebook to explore different skeletonization and medial axis transformation techniques.

## Features

- Implementation of various skeletonization methods:
  - Basic skeletonization
  - Lee's algorithm (1994)
- Medial Axis Transform (MAT) with distance transform
- Comparison of different skeletonization techniques
- Visualization of results using matplotlib
- Content-Based Image Retrieval (CBIR) using Hu Moments
- Comparison of CBIR results with and without skeletonization

## Examples

### Skeletonization

The project demonstrates skeletonization on various test images:

```python
test_skeletonize(img)
```

This function visualizes the original image, medial axis transform, basic skeletonization, and Lee's algorithm results.

### Content-Based Image Retrieval

The project includes CBIR functionality:

```python
indx_mat = CBIR_Indexation(loaded_images)
distances = CBIR_Recherche(img_requete, indx_mat)
```

This code indexes the images and performs a search based on Hu Moments, both with and without skeletonization.

## Contributing

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Create a new Pull Request

## License

This project is licensed under the MIT License .
