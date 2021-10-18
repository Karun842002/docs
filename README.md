# Overview
DeepSqueak is a USV detection and analysis software suite that can perform human quality USV detection and classification automatically, rapidly, and reliably using cutting-edge regional convolutional neural network architecture (Faster-RCNN). DeepSqueak was engineered to allow non-experts easy entry into USV detection and analysis yet is flexible and adaptable with a graphical user interface and offers access to numerous input and analysis features. 

# Installation

DeepSqueak v3 relies on recently introduced neural network architecture and will only run on MATLAB 2020a or later.
To install MATLAB follow the instruction at https://in.mathworks.com/help/install/install-products.html

### Required Matlab toolboxes:
```
Computer Vision System Toolbox™
Curve Fitting Toolbox™
Image Processing Toolbox™
Deep Learning Toolbox™ (formerly Neural Network Toolbox™)
Parallel Computing Toolbox™
Statistics and Machine Learning Toolbox™
Signal Processing Toolbox™
```

Clone the repository
```
git clone https://github.com/DrCoffey/DeepSqueak.git
```

To run DeepSqueak, navigate to the main DeepSqueak folder in MATLAB, and type "DeepSqeak" into the command line. DeepSqueak will add itself to the MATLAB path after running.

### Troubleshooting
```
Q : DeepSqueak V3 requires MATLAB 20201 or later. It looks like you are use MATLAB
A : Update MATLAB to the latest version
```
```
Q : Toolbox not found
A : 1. Launch the MATLAB Installer
    2. Choose the necessary toolboxes.
    3. Install the toolboxes.
```

# Main Window
![Main Window](https://i.imgur.com/6KMLQiD.png)

**1\. Main Menus**

  - File: Working Folder Selection, Session Save, & Import/Export 

**2\. Call Statistics**

  - See [Export to Excel](export-to-excel)

**3\. Waveform and Extracted Contour**

  - Call [<span class="underline">contour</span>](contour-detection),
    slope line.
  - Contour extraction is now handled automatically
  - Contour extraction thresholds are still editable in Tools menu 

**4\. Working Folder Dropdowns**

  - Selected items will used when detect and load buttons are called

**5\. Detect, Load, and Record Buttons**

  - [Detect Calls] Load selected neural network and audio file
  - [Load Calls] Load selected detected call file
  - [Load Audio] Load selected audio file without any detections

**6\. Detection Review Buttons**

  - Keyboard shortcuts in parentheses
  - Drag box corners to adjust 
  - Right click to delete box
  - Double click for custom labels
  - Custom label keyboard shortcuts can be defined in "Tools "

**7\. Navigation Buttons**

  - [>] Move one call
  - [>>] Move one focus window
  - [>>>] Move one page window
 
**8\. Quick Access Settings**

  - [Focus] Change focus window (11) scale
  - [Page] Change page window (10) scale
  - [Scale] Change spectrogram display settings
  - [Colormap] Change colormap, invert colormap, adjust brightness/contrast

**9\. Complete Audio File Timeline**

  - Green curve represents detected call density
  - Click anywhere to jump locations in the file

**10\. Page Window**

  - View a large chuck of the audio file for better context
  - Click anywhere to move focus window (11)

**11\. Focus Window**

  - Adjust call boxes
  - Delete call boxes
  - Reject call boxes
  - Add new call boxes


