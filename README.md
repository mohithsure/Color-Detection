Color Detection
============================
**Project Overview**
----------------
This Python-based application loads an image and lets the user interact with it. Upon a double-click, it captures the pixProject Structure

-----------------

Color-Detection/

■■■ color_detection.py # Main application script

■■■ colors.csv # Color dataset (names, hex, RGB)

■■■ colorpic.jpg # Input image for color detection

**System Requirements**
-------------------
- Operating System: Windows / macOS / Linux
- Processor: Dual-core 2 GHz or higher
- RAM: Minimum 4 GB
  
**Library Requirements**
--------------------
Make sure you have Python 3.6 or above installed.
Install required packages using:
pip install opencv-python pandas

**How to Run**
----------
1. Clone this repository:
 git clone https://github.com/yourusername/color-detection.git
 cd color-detection
2. Replace 'colorpic.jpg' with your own image if desired.
3. Run the script:
 python color_detection.py
4. Double-click anywhere on the image to detect the color. Press ESC to exit.
   
**How It Works**
------------
- Loads image using OpenCV.
- Loads color data from 'colors.csv'.
- Captures RGB values on mouse double-click.
- Compares the clicked color to the dataset using Manhattan distance:
 Distance = |R1-R2| + |G1-G2| + |B1-B2|
- Displays the closest color name and its RGB values on the image.
  
**Example Output**
--------------
Displays color name and RGB values on a color-filled rectangle on the image.

**References**
----------
- OpenCV: https://opencv.org
- pandas: https://pandas.pydata.org
- Color dataset: Public repositories on GitHub/Kaggle
  
**Future Enhancements**
-------------------
- Add web-based interface using Flask or Streamlit
- Use a machine learning model for better perceptual color matching
- Add multi-language color support
  
**License**
-------
This project is open-source and available under the MIT License.
