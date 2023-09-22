# CamScanner

CamScanner is a Python project that utilizes computer vision techniques to enhance and scan documents. Below, you'll find an overview of the project's key components and how they work together to achieve the goal of document scanning.

## Table of Contents
- [Imports](Document%20Scanner.ipynb#Imports)
- [Utilities](Document%20Scanner.ipynb#Utilities)
- [Image](Document%20Scanner.ipynb#Image)
- [Process](Document%20Scanner.ipynb#Process)
  - [Morphological Operation and GrabCut](Document%20Scanner.ipynb#Morphological-Operation-and-GrabCut)
  - [Grayscale Transform](Document%20Scanner.ipynb#Grayscale-Transform)
  - [Blurring the Image](Document%20Scanner.ipynb#Blurring-the-Image)
  - [Edge Detection](Document%20Scanner.ipynb#Edge-Detection)
  - [Contour Detection](Document%20Scanner.ipynb#Contour-Detection)
  - [Perspective Transform](Document%20Scanner.ipynb#Perspective-Transform)
  - [Image Enhancement](Document%20Scanner.ipynb#Image-Enhancement)
  - [Result](Document%20Scanner.ipynb#Result)

---

## Imports

The "Imports" section at the beginning of your Jupyter Notebook contains the necessary Python libraries that are imported to support image processing and manipulation. This includes OpenCV (cv2), NumPy (numpy), and Matplotlib (matplotlib).

[Code Reference](Document%20Scanner.ipynb#Imports)

---

## Utilities

The "Utilities" section includes utility functions that simplify image manipulation and processing. Two primary functions are `imshow` (for displaying images) and `reorder` (for reordering vertices).

[Code Reference](Document%20Scanner.ipynb#Utilities)

---

## Image

In the "Image" section, an example image is loaded using OpenCV's `imread` function. The loaded image serves as the input for subsequent processing steps.

[Code Reference](Document%20Scanner.ipynb#Image)

---

## Process

The "Process" section outlines the step-by-step procedure for enhancing and scanning the document image. Each subsection corresponds to a distinct image processing step:

### Morphological Operation and GrabCut

This step involves applying morphological operations and the GrabCut algorithm to remove text and unnecessary details from the document image, leaving only the main content.

[Code Reference](Document%20Scanner.ipynb#Morphological-Operation-and-GrabCut)

### Grayscale Transform

The "Grayscale Transform" section focuses on converting the color document image to grayscale. This simplifies further image processing and analysis.

[Code Reference](Document%20Scanner.ipynb#Grayscale-Transform)

### Blurring the Image

Here, blurring techniques are applied to the grayscale image to reduce noise and enhance document clarity. Bilateral filtering is one option provided.

[Code Reference](Document%20Scanner.ipynb#Blurring-the-Image)

### Edge Detection

The "Edge Detection" step involves using the Canny edge detection algorithm to identify edges and outlines within the document image.

[Code Reference](Document%20Scanner.ipynb#Edge-Detection)

### Contour Detection

This part revolves around identifying and detecting the four vertices of the document by analyzing image contours. The goal is to create a 4x2 array representing the vertices.

[Code Reference](Document%20Scanner.ipynb#Contour-Detection)

### Perspective Transform

The "Perspective Transform" section focuses on cropping out the document region from the image by applying a perspective transformation. It ensures the final output is aligned and rectangular.

[Code Reference](Document%20Scanner.ipynb#Perspective-Transform)

### Image Enhancement

Image enhancement techniques are optional and can be implemented based on your preferences. This step allows you to improve the quality of the scanned document further. Functions for techniques like cartooning, histogram equalization, thresholding, adaptive thresholding, CLAHE, and division by fake flat field F are provided.

[Code Reference](Document%20Scanner.ipynb#Image-Enhancement)

### Result

The "Result" section combines all the previous processing steps to scan and enhance the document image. The final scanned output is displayed and saved as an image file.

[Code Reference](Document%20Scanner.ipynb#Result)

---

## Contributing

Feel free to contribute to this project by creating pull requests or opening issues. Your feedback and contributions are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
