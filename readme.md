# Automatic Vehicle Speed Detection using Video Processing

This project aims to detect vehicle speed from a video using YOLO (You Only Look Once) object detection and custom tracking algorithms.

## Files and Directories

speed.py: Main script to run the vehicle speed detection.
main.py: Script for vehicle tracking and displaying vehicle IDs.
tracker.py: Contains the Tracker class used for tracking vehicles between frames.
coco.txt: List of object classes used by the YOLO model.

## Requirements

Python 3.x
OpenCV
Pandas
NumPy
Ultralytics YOLO
A pre-trained YOLO model (e.g., yolov8s.pt)

## How to Run the Project

1. Ensure you have the required libraries installed. You can install them using:
    ```bash
    pip install opencv-python-headless pandas numpy ultralytics
    ```

2. Download the YOLO model weights (`yolov8s.pt`) and place it in the same directory as the project files.

3. Ensure you have a video file named `veh2.mp4` in the same directory as the project files.

4. Run the `speed.py` file to start the vehicle speed detection:
    ```bash
    python speed.py
    ```

5. Optionally, you can run the `main.py` file to see a simplified version of the object detection and tracking:
    ```bash
    python main.py
    ```
## Important Notes

- The distances used for speed calculation are assumed to be 10 meters. Adjust this value based on the actual distances in your video for accurate speed calculation.
- The project uses a basic tracker implementation and may require further refinement for more accurate tracking and speed detection in different scenarios.

## License

This project is open-source and available under the MIT License.