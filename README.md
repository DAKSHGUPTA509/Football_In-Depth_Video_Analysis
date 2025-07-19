# ⚽ Football In-Depth Video Analysis 📊

This application provides advanced video analysis tools tailored for football analysts and developers. 👨‍💻 It enhances raw football footage, providing insights through automated processing and visualization. ⚙️ This allows for detailed examination of player movements, tactical formations, and key moments within a game. 🔍

## Table of Contents
- [Features](#features)
- [Installation](#installation-💻)
- [Dependencies](#dependencies-🧩)
- [Usage](#usage-🚀)
- [Contribution Guidelines](#contribution-guidelines-🤝)
- [Troubleshooting](#troubleshooting-🛠️)
- [Directory Structure](#directory-structure)

## Features

*   **Automated Player Tracking:** 🏃‍♂️ Identifies and tracks players throughout the video.
*   **Tactical Formation Analysis:** 📐 Analyzes and visualizes team formations.
*   **Event Detection:** 💥 Automatically detects key events like passes, shots, and tackles.
*   **Enhanced Visualization:** 📈 Overlays data and visualizations onto the original video to highlight important information.
*   **Before-and-After Comparison:** 🖼️ Demonstrates the enhancement achieved through video processing.

This is the input video file pic before processing:
![Before Processing](https://github.com/user-attachments/assets/4c15cb70-a9ab-4294-b16b-d368e23993d6)

This is the output video file pic after processing:
![After Processing](https://github.com/user-attachments/assets/f8cae508-d46c-4a93-b7c7-a827e90ff0b2)

## Installation 💻

1.  **Clone the repository:**
> *   Python 3.7+ 🐍
*   OpenCV 📸
*   TensorFlow or PyTorch (depending on the model) 🧠
*   NumPy 🔢
*   [List any other specific Python packages]

> List any specific versions of the dependencies if required for compatibility.

Model file is linked in `models/models.txt`. 🔗

## Usage 🚀

bash
> python main.py --input_video [path_to_input_video] --output_video [path_to_output_video] --config [path_to_config_file]
>     *   `--input_video`: Path to the input video file. 📹
    *   `--output_video`: Path to the output video file. 🎬
    *   `--config`: Path to the configuration file (optional, defaults to `config.ini`). ⚙️

        Example:
> *   **Input:** The application primarily supports `.mp4` video files. Other common formats like `.mov` and `.avi` might work but are not guaranteed. 🎥
*   **Output:** The processed video is output as an `.avi` file by default. This can be configured in the `config.ini` file. 📤

> Note that using other video formats might require installing additional codecs.

## Contribution Guidelines 🤝

1.  Fork the repository. 🍴
2.  Create a new branch for your feature or bug fix. 🌿
3.  Make your changes and commit them with descriptive messages. ✍️
4.  Submit a pull request. 📤

> Please follow the coding style and conventions used in the project.

## Troubleshooting 🛠️

*   **Issue:** "ModuleNotFoundError: No module named 'cv2'"

    **Solution:** Install OpenCV: `pip install opencv-python`
*   **Issue:** "Error: Model file not found"

    **Solution:** Ensure the model file is downloaded and the `model_path` in `config.ini` is correct.
*   **Issue:** "Video processing is slow"

    **Solution:** Try reducing the resolution of the input video or using a more powerful machine. Also, ensure that you are using GPU acceleration if available.

## Directory Structure

<pre>
└── daxgupta-football_in-depth_video_analysis/
    ├── README.md
    ├── main.py
    ├── yolo_custom.ipynb
    ├── yolo_inference.ipynb
    ├── camera_movement_estimator/
    │   ├── __init__.py
    │   └── camera_movement_estimator.py
    ├── development_and_analysis/
    │   └── color_assignement.ipynb
    ├── models/
    │   └── Link to download file under moodels.txt
    ├── output_video/
    │   └── Link to download files under output_video.txt
    ├── player_ball_assigner/
    │   ├── __init__.py
    │   └── player_ball_assigner.py
    ├── runs/
    │   └── Link to download all the files and folders under runs.txt
    ├── speed_and_distance_estimator/
    │   ├── __init__.py
    │   └── speed_and_distance_estimator.py
    ├── stubs/
    │   ├── camera_movement_stub.pkl
    │   └── track_stubs.pkl
    ├── team_assigner/
    │   ├── __init__.py
    │   └── team_assigner.py
    ├── trackers/
    │   ├── __init__.py
    │   └── tracker.py
    ├── training/
    │   └── Football_video_analysis.ipynb
    ├── utils/
    │   ├── __init__.py
    │   ├── bbox_utils.py
    │   └── video_utils.py
    └── view_transformer/
        ├── __init__.py
        └── view_transformer.py
</pre>
