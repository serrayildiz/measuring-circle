# Object Dimension Measurement using OpenCV

This repository contains Python code to measure the dimensions of objects in an image using OpenCV. The code utilizes contour detection, perspective transformation, and Euclidean distance measurement techniques to accurately calculate the dimensions.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- imutils

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/serrayildiz/object-dimension-measurement.git
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Place the image containing the object whose dimensions you want to measure in the project directory.
2. Update the `image_path` variable in the Python script with the path to your image.
3. Run the script:

   ```bash
   python measure_dimensions.py
   ```

4. Follow the on-screen instructions to view the calculated dimensions.

## Methodology

The script performs the following steps:

1. **Image Preprocessing**: Convert the image to grayscale, apply Gaussian blur, and detect edges using the Canny edge detector.
2. **Contour Detection**: Find contours in the edge-detected image.
3. **Contour Filtering**: Filter out small contours that are likely noise.
4. **Contour Sorting**: Sort contours from left to right.
5. **Dimension Calculation**: For each remaining contour, calculate the dimensions using perspective transformation and Euclidean distance measurement.
6. **Display**: Display the original image with annotated dimensions.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project was inspired by [OpenCV](https://opencv.org/) and [imutils](https://github.com/jrosebr1/imutils).


