# Semantic-Image-and-Text-Alignment

## Overview
This project is aimed at automating the generation of advertisement sequences using a combination of images and text. The tool takes input from a JSON file that outlines a series of creative concepts. Each concept includes details such as the creative idea's name, a frame-by-frame breakdown, an overarching description of the advertisement's concept, and recommended assets for each frame. The tool then composes these concepts into frames and generates a sequence to convey the intended message to the audience. It's designed to streamline the process of creating ads for various platforms.

## Input JSON Format
The input JSON file outlines a series of concepts, with each object containing the following details:
- **Concept**: The creative idea's name.
- **Implementation**: A detailed, frame-by-frame breakdown, providing visual representations and explanations for each segment.
- **Explanation**: An overarching description of the advertisement's concept and the intended user flow.
- **Asset Suggestions**: For each frame, a curated list of three recommended assets is provided, detailing the category and a brief description of each suggested element.

## Features
- **Image and Text Integration**: Incorporate both images and text seamlessly into the ad frames.
- **Image Composition**: Utilize a variety of layout templates to arrange images and text within frames.
- **Storyboard Generation**: Automatically generate a sequence of frames to create a cohesive narrative or flow for the advertisement.
- **Export Options**: Export the final ad sequence in various formats suitable for different platforms and resolutions.

## Installation
1. Clone this repository to your local machine using the following command:
    ```bash
    git clone https://github.com/natybkl/Semantic-Image-and-Text-Alignment.git

    cd Semantic-Image-and-Text-Alignment
    ```
2. Install the required dependencies using pip and the provided `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```


## Usage
### Image Analysis with YOLO v3
As a starter, you can perform image analysis using the provided data-analysis folder.

1. Download the pre-trained YOLO v3 weights file from [this link](https://pjreddie.com/media/files/yolov3.weights) and place it in the current directory. Alternatively, you can download it directly to the current directory using the following command in the terminal:
    ```bash
    wget https://pjreddie.com/media/files/yolov3.weights
    ```

2. Run the image analysis script using the following command format:
    ```bash
    python data-analysis/object_detection_using_yolo.py --image /path/to/input/image --config /path/to/config/file --weights /path/to/weights/file --classes /path/to/classes/file
    ```

    For example:
    ```bash
    python data-analysis/object_detection_using_yolo.py --image data-analysis/unlabeled_images/toy_car.png --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt
    ```

Replace the `/path/to/input/image`, `/path/to/config/file`, `/path/to/weights/file`, and `/path/to/classes/file` with the respective paths in your system.

This will perform object detection using YOLO v3 on the specified image using the provided configuration, weights, and classes files.

### Image & Text Generation

### Composition

### Storyboard

## Example
