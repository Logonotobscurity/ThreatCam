# ThreatCam

## Overview
ThreatCam is an advanced AI-powered camera security system that leverages cutting-edge machine learning technologies to provide intelligent surveillance capabilities. Built on the foundation of computer vision and deep learning, this project aims to transform traditional CCTV systems into smart security solutions.

## Key Features
- **Real-time Person Detection**: Utilizes YOLOv7 for accurate human detection
- **Facial Recognition**: Advanced facial recognition capabilities for identity verification
- **Intrusion Detection**: Smart alerting system for unauthorized access
- **Person Re-Identification (ReID)**: Track and identify individuals across multiple camera views
- **Traffic Monitoring**: Analyze and monitor vehicle movement patterns
- **Edge AI Processing**: Local processing capabilities for enhanced privacy and reduced latency

## Technology Stack
- **AI/ML Framework**: 
  - YOLOv7 (Object Detection)
  - FastReID (Person Re-Identification)
  - ResNet50 (Feature Extraction)
- **Database**: 
  - Milvus Vector Database (Feature Storage)
- **Development Tools**:
  - Docker (Containerization)
  - Python 3.6+ (Core Development)
  - LabelStudio (Data Annotation)

## System Requirements
- **Hardware**:
  - Supported Devices:
    - NVIDIA Jetson (Nano, Xavier AGX)
    - Raspberry Pi (4GB/8GB)
    - Intel x64 Systems
  - Compatible Cameras:
    - RTSP Cameras
    - IP Cameras
    - USB Webcams
- **Software**:
  - Docker
  - Python 3.6 or higher
  - CUDA (for GPU acceleration)

## Installation

### Prerequisites
1. Install Docker
2. Install Python 3.6+
3. Ensure you have a compatible camera setup

### Quick Start
```bash
# Install the package
pip3 install sharpai-hub

# Start the main service
sharpai-cli yolov7_reid start
```

### Configuration
1. Access the web interface at `http://localhost:8000`
2. Configure your camera settings
3. Set up detection parameters
4. Configure alert notifications

## Usage
1. **Camera Setup**:
   - Connect your camera
   - Configure RTSP/IP settings
   - Verify connection

2. **Detection Configuration**:
   - Set detection zones
   - Configure sensitivity
   - Set up alert rules

3. **Monitoring**:
   - Access live feed
   - View detection events
   - Manage alerts

## Features in Detail
- **Person Detection**
  - Real-time human detection
  - Multiple person tracking
  - Movement pattern analysis

- **Facial Recognition**
  - Face detection and recognition
  - Identity matching
  - Unknown person alerts

- **Traffic Monitoring**
  - Vehicle detection
  - Traffic pattern analysis
  - Parking monitoring

## Integration
- Home Assistant compatible
- REST API available
- Webhook support for notifications

## Development
```bash
# Clone the repository
git clone [repository-url]

# Install development dependencies
pip install -r requirements-dev.txt

# Run tests
python -m pytest tests/
```

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## Security Considerations
- All data is processed locally
- No cloud dependencies required
- End-to-end encryption for data transmission
- Regular security updates

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Support
- GitHub Issues: [Link to Issues]
- Documentation: [Link to Docs]
- Community Forum: [Link to Forum]

## Acknowledgments
- YOLOv7 Team
- FastReID Contributors
- Milvus Database Team
- Open Source Community

## Disclaimer
This software is provided as-is, without any guarantees or warranties. Users are responsible for complying with local privacy and surveillance laws.
