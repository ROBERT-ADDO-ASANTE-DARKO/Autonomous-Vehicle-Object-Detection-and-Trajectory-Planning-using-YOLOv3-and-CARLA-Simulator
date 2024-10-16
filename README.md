# Autonomous Vehicle Object Detection and Trajectory Planning

## Project Overview

This final year project focuses on Autonomous Vehicle Object Detection and Trajectory Planning using YOLOv3 and CARLA Simulator. The project demonstrates the integration of state-of-the-art object detection techniques with a realistic autonomous driving simulator to enhance vehicle perception and decision-making capabilities.

### Key Features:
- Object detection using YOLOv3 algorithm
- Integration with CARLA Simulator for realistic autonomous driving scenarios
- Trajectory planning based on detected objects and environmental constraints
- Performance monitoring and visualization using TensorBoard

## Installation

### Prerequisites:
- Python 3.7 or higher
- CARLA Simulator 0.9.11

### Steps:

1. Download the required version of the CARLA Simulator ZIP file for Windows:
   ```
   https://github.com/carla-simulator/carla/releases
   cd CARLA_0.9.11
   ```

2. Install CARLA_0.9.11 following the official documentation.

3. Clone this project repository:
   ```
   https://github.com/ROBERT-ADDO-ASANTE-DARKO/Autonomous-Vehicle-Object-Detection-and-Trajectory-Planning-using-YOLOv3-and-CARLA-Simulator.git
   cd Autonomous-Vehicle-Object-Detection-and-Trajectory-Planning-using-YOLOv3-and-CARLA-Simulator
   ```

4. Install the required Python libraries:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Copy the `object_detection.py` file to the CARLA PythonAPI examples directory:
   ```
   cp object_detection.py CARLA_0.9.11/PythonAPI/examples/
   ```

2. Download the yolov3.weights and yolo3.cfg files
   '''
   https://huggingface.co/spaces/Epitech/Scarecrow/resolve/main/yolov3.weights
   '''

3. Run the CARLA Simulator:
   ```
   cd CARLA_0.9.11
   ./CarlaUE4.exe
   ./CarlaUE4 -dx11
   ```

4. In a new terminal, navigate to the PythonAPI examples directory and run the script:
   ```
   cd /path/to/carla/PythonAPI/examples
   python object_detection.py
   ```

## Monitoring Model Performance

To monitor and track the YOLOv3 model performance using TensorBoard:

1. Start TensorBoard:
   ```
   tensorboard --logdir=path/to/logs
   ```

2. Open a web browser and go to `http://localhost:6006` to view the TensorBoard dashboard.

## Project Structure

- `object_detection.py`: Main Python script for object detection and trajectory planning
- `requirements.txt`: List of required Python libraries
- `models/`: Directory containing trained YOLOv3 model weights
- `config/`: Configuration files for YOLOv3 and trajectory planning
- `logs/`: TensorBoard log files for performance monitoring

## Contributing

Contributions to improve the project are welcome. Please feel free to fork the repository, make changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- CARLA Simulator team for providing a robust autonomous driving simulation platform
- YOLOv3 developers for the efficient object detection algorithm

