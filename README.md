# Vehicle-tracking-YOLO11n
Vehicle Tracking with YOLO11n
Real-time vehicle detection and tracking system using YOLO11n model. The system can detect and track cars and trucks in video streams.

# Features

- Real-time vehicle detection
- Multi-class tracking (cars and trucks)
- Video output saving capability
- GPU acceleration support
- Custom dataset training support

## Dataset

Dataset sourced from Roboflow Universe containing annotated vehicle images:
- Classes: Cars and Trucks
- Split: Train, Validation, Test sets
- Version: 1
- License: MIT

Dataset structure:
```
dataset/
├── train/images/
├── valid/images/
└── test/images/
```

## Requirements

```bash
pip install -r requirements.txt
```

### Configuration

data.yaml:
```yaml
train: ../train/images
val: ../valid/images
test: ../test/images

nc: 2
names: ['car', 'truck']

roboflow:
  workspace: my-projects-ons8w
  project: object-tracking-and-detection-mkhw4
  version: 1
  license: MIT
  url: https://universe.roboflow.com/my-projects-ons8w/object-tracking-and-detection-mkhw4/dataset/1
```
## Results

  <img src="results\result.gif" height="50%" width="50%"
        style="object-fit:contain"
    />
## License

MIT License

## Acknowledgments

- Dataset from Roboflow Universe
- YOLO11n by Ultralytics
