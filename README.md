# LineDetection
## Abstract
A pipeline which extract edges from an image with Canny Edge Detector and then identifies lines, which form those edges. Here we provided our own implementation of OpenCV algorithms [Canny](https://docs.opencv.org/3.1.0/dd/d1a/group__imgproc__feature.html#ga04723e007ed888ddf11d9ba04e2232de) and [HoughLines](https://docs.opencv.org/2.4/modules/imgproc/doc/feature_detection.html?highlight=houghlines#houghlines), which we compared with original OpenCV realization.
## How to use
Just clone/fork the repository and run the `main.ipynb` file. If you want to use it with your own images, update `Image_path` with correct image path in section "Global Parameters". You might need to update other parameters as well.
## Algorithm
Basically, we could divide the entiry process into 3 steps:
* **Data Preprocessing:** convering image to a greyscale and then binarizing it,
* **Edge Detection:** extracting figure's edges with Canny Edge Detector,
* **Line Detection:** discovering line, which identifies the edges, with Hough transform.

You can find a step by step description of Canny Edge Detection [here](http://justin-liang.com/tutorials/canny/#grayscale), while for Hough transform you can check a great explanation [here](http://aishack.in/tutorials/hough-transform-basics/)
## References
* [The Hough Transform. The Basics](http://aishack.in/tutorials/hough-transform-basics/)
* [CANNY EDGE DETECTION](http://justin-liang.com/tutorials/canny/#grayscale)
* [Understanding Hough Transform With Python](https://alyssaq.github.io/2014/understanding-hough-transform/)
* [Implementing a simple python code to detect straight lines using Hough transform](https://www.science-emergence.com/Articles/Implementing-a-simple-python-code-to-detect-straight-lines-using-Hough-transform/)
* [PythonCannyEdge](https://github.com/fubel/PyCannyEdge)
