Shape Feature Extraction: Skeletonization and Medial Axis Transformation

This project implements and explores various shape feature extraction techniques, focusing on skeletonization and medial axis transformation. These methods are essential for analyzing and processing binary images, particularly useful in computer vision and image processing applications.

Table of Contents

    Installation
    Usage
    Features
    Examples
    Contributing
    License

Installation

To run this project, you need to have Python installed along with several dependencies. You can install the required packages using pip:

bash

Copy Code
pip install numpy matplotlib scikit-image opencv-python pillow scipy

Usage

    Clone the repository:

bash

Copy Code
   git clone https://github.com/yourusername/shape-feature-extraction.git
   cd shape-feature-extraction

    Run the Jupyter notebook:

bash

Copy Code
   jupyter notebook "Explore Skeletonization.ipynb"

    Follow the instructions in the notebook to explore different skeletonization and medial axis transformation techniques.

Features

    Implementation of various skeletonization methods:
        Basic skeletonization
        Lee's algorithm (1994)
    Medial Axis Transform (MAT) with distance transform
    Comparison of different skeletonization techniques
    Visualization of results using matplotlib
    Content-Based Image Retrieval (CBIR) using Hu Moments
    Comparison of CBIR results with and without skeletonization

Examples
Skeletonization

The project demonstrates skeletonization on various test images:

python

Execute

Copy Code
test_skeletonize(img)

This function visualizes the original image, medial axis transform, basic skeletonization, and Lee's algorithm results.
Content-Based Image Retrieval

The project includes CBIR functionality:

python

Execute

Copy Code
indx_mat = CBIR_Indexation(loaded_images)
distances = CBIR_Recherche(img_requete, indx_mat)

This code indexes the images and performs a search based on Hu Moments, both with and without skeletonization.

Contributing

Contributions to this project are welcome. Please follow these steps:

    Fork the repository
    Create a new branch (git checkout -b feature/your-feature)
    Make your changes
    Commit your changes (git commit -am 'Add some feature')
    Push to the branch (git push origin feature/your-feature)
    Create a new Pull Request

License

This project is licensed under the MIT License - see the LICENSE file for details.

Step 9: Final Touches

Lastly, I would add some badges at the top of the README for quick information:

Python
License
Contributions welcome

