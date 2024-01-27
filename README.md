# fish-counter

How to set up the project:

- Establish a python virtual environment        python -m venv .virtenv
- Activate the virtual environment              .virtenv\Scripts\activate
- Install dependencies                          py -m pip install opencv-python numpy matplotlib.pyplot


Fish detection and tracking algorithm:

Step 1: Detect fish using YOLO-Fish

Step 2: Track fish between frames using SIFT
- For each object (bounding box) found in Step 1, use SIFT to detect key features
- Save object and feature information in an array representing spatial layout of frame
- Compare features by considering objects from previous frame within a limited spatial range
