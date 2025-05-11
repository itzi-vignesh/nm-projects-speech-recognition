# Audio Data Preprocessing and Augmentation Project

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)

## Overview
This project focuses on preprocessing and augmenting audio data from the Common Voice dataset. It implements a comprehensive pipeline for audio data preparation, including format conversion, data cleaning, and augmentation techniques. The project is designed to help researchers and developers prepare audio datasets for machine learning applications.

## Features
- Audio format conversion (MP3 to WAV)
- Data cleaning and metadata processing
- Audio augmentation techniques:
  - Random noise addition
  - Pitch shifting
- Sample rate standardization (16kHz)
- Metadata management and organization
- Batch processing for memory efficiency
- Progress tracking and error handling

## Dependencies
- Python 3.x
- pandas
- librosa
- soundfile
- numpy

## Project Structure
```
nm-unit1/
├── nm-unit1.ipynb      # Main notebook containing the implementation
├── README.md          # This file
├── LICENSE           # MIT License
└── CONTRIBUTING.md   # Contribution guidelines
```

## Implementation Details
1. **Data Loading and Preprocessing**
   - Loads audio data from Common Voice dataset
   - Processes metadata from TSV files
   - Cleans and organizes audio file paths
   - Handles missing or corrupted data

2. **Audio Processing**
   - Converts MP3 files to WAV format
   - Standardizes sample rate to 16kHz
   - Handles audio file loading and saving
   - Implements efficient batch processing

3. **Data Augmentation**
   - Implements noise addition with configurable noise factor
   - Applies pitch shifting for data variety
   - Randomly applies augmentations to create diverse dataset
   - Maintains audio quality standards

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/itzi-vignesh/nm-projects-speech-recognition.git
   cd nm-unit1
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Update the data paths in the notebook to match your local setup:
   - Source directory for MP3 files
   - Destination directory for processed WAV files
   - Metadata file paths

2. Run the notebook cells sequentially to:
   - Process the audio files
   - Apply augmentations
   - Generate augmented dataset

## Contributing
We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute to this project.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Notes
- The project uses the Common Voice dataset format
- Audio files are processed in batches to manage memory efficiently
- Augmentation parameters can be adjusted in the code for different effects
- Error handling and logging are implemented for robust processing

## Contact
For questions and feedback, please open an issue in the GitHub repository. 