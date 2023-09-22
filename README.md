# Cam-Scanner

CamScanner is a Python project that utilizes computer vision techniques to enhance and scan documents. Below, you'll find an overview of the project's key components and how they work together to achieve the goal of document scanning.

## Table of Contents
- [Imports](#imports)
- [Utilities](#utilities)
- [Image](#image)
- [Process](#process)
  - [Morphological Operation and GrabCut](#morphological-operation-and-grabcut)
  - [Grayscale Transform](#grayscale-transform)
  - [Blurring the Image](#blurring-the-image)
  - [Edge Detection](#edge-detection)
  - [Contour Detection](#contour-detection)
  - [Perspective Transform](#perspective-transform)
  - [Image Enhancement](#image-enhancement)
  - [Result](#result)

---

## Imports

In this section, the necessary Python libraries are imported to support image processing and manipulation. This includes OpenCV (cv2), NumPy (numpy), and Matplotlib (matplotlib).

[Code Reference](#imports)

---

## Utilities

The Utilities section contains utility functions that simplify image manipulation and processing. Two primary functions are `imshow` (for displaying images) and `reorder` (for reordering vertices).

[Code Reference](#utilities)

---

## Image

In this part, an example image is loaded using OpenCV's `imread` function. The loaded image will be used as the input for subsequent processing steps.

[Code Reference](#image)

---

## Process

The Process section outlines the step-by-step procedure for enhancing and scanning the document image. Each subsection corresponds to a distinct image processing step:

### Morphological Operation and GrabCut

This step involves applying morphological operations and the GrabCut algorithm to remove text and unnecessary details from the document image, leaving only the main content.

[Code Reference](#morphological-operation-and-grabcut)

### Grayscale Transform

The Grayscale Transform section focuses on converting the color document image to grayscale. This simplifies further image processing and analysis.

[Code Reference](#grayscale-transform)

### Blurring the Image

Here, blurring techniques are applied to the grayscale image to reduce noise and enhance document clarity. Bilateral filtering is one option provided.

[Code Reference](#blurring-the-image)

### Edge Detection

The Edge Detection step involves using the Canny edge detection algorithm to identify edges and outlines within the document image.

[Code Reference](#edge-detection)

### Contour Detection

This part revolves around identifying and detecting the four vertices of the document by analyzing image contours. The goal is to create a 4x2 array representing the vertices.

[Code Reference](#contour-detection)

### Perspective Transform

The Perspective Transform section focuses on cropping out the document region from the image by applying a perspective transformation. It ensures the final output is aligned and rectangular.

[Code Reference](#perspective-transform)

### Image Enhancement

Image enhancement techniques are optional and can be implemented based on your preferences. This step allows you to improve the quality of the scanned document further. Functions for techniques like cartooning, histogram equalization, thresholding, adaptive thresholding, CLAHE, and division by fake flat field F are provided.

[Code Reference](#image-enhancement)

### Result

The Result section combines all the previous processing steps to scan and enhance the document image. The final scanned output is displayed and saved as an image file.

[Code Reference](#result)

---

## Contributing

Feel free to contribute to this project by creating pull requests or opening issues. Your feedback and contributions are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

