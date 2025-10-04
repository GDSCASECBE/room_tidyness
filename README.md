# 🏠 Room Tidiness Classifier

A machine learning project that uses computer vision and digital image processing to classify whether a room is clean or messy. This project demonstrates the application of image classification techniques using Python and popular ML libraries.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Implementation Details](#implementation-details)
- [Contributing](#contributing)
- [Project Mentors](#project-mentors)
- [License](#license)

## 🎯 Overview

This project aims to solve the problem of automatically determining whether a room is clean or messy using computer vision techniques. The classifier analyzes room images and provides a binary classification: **Clean** or **Messy**.

### Key Capabilities
- **Binary Classification**: Distinguishes between clean and messy rooms
- **Image Processing**: Converts images to grayscale and processes them for ML
- **Scalable Architecture**: Designed to handle various room types and conditions
- **Educational Purpose**: Perfect for learning computer vision and ML concepts

## ✨ Features

- 🖼️ **Image Preprocessing**: Converts images to grayscale and flattens them for ML processing
- 🧠 **Machine Learning Pipeline**: Implements training and testing functions
- 📊 **Data Visualization**: Includes tools for analyzing and visualizing the dataset
- 🔧 **Modular Design**: Well-structured code with separate functions for different tasks
- 📈 **Progress Tracking**: Uses tqdm for progress monitoring during data processing

## 📁 Dataset

The project includes a carefully curated dataset of room images:

### Dataset Statistics
- **Training Set**: 192 images (96 clean + 96 messy)
- **Validation Set**: 20 images (10 clean + 10 messy)  
- **Test Set**: 10 images (unlabeled for final evaluation)
- **Image Format**: PNG files
- **Image Size**: 128x128 pixels (configurable)

### Dataset Structure
```
room_tidyness/
├── train/
│   ├── clean/          # 96 training images of clean rooms
│   └── messy/          # 96 training images of messy rooms
├── val/
│   ├── clean/          # 10 validation images of clean rooms
│   └── messy/          # 10 validation images of messy rooms
└── test/               # 10 test images for final evaluation
```

## 🏗️ Project Structure

```
room_tidyness/
├── README.md                    # Project documentation
├── Room_tidyness.ipynb         # Main Jupyter notebook with implementation
├── train/                      # Training dataset
│   ├── clean/                  # Clean room images
│   └── messy/                  # Messy room images
├── val/                        # Validation dataset
│   ├── clean/                  # Clean room images
│   └── messy/                  # Messy room images
└── test/                       # Test dataset (unlabeled)
```

## 📦 Dependencies

The project requires the following Python packages:

```python
numpy          # Linear algebra operations
pandas         # Data processing and CSV file I/O
matplotlib     # Data visualization and plotting
opencv-python  # Computer vision and image processing
Pillow         # Python Imaging Library for image handling
tqdm           # Progress bars for long-running operations
```

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/room_tidyness.git
   cd room_tidyness
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install numpy pandas matplotlib opencv-python Pillow tqdm jupyter
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

## 💻 Usage

### Running the Project

1. Open `Room_tidyness.ipynb` in Jupyter Notebook
2. Execute the cells in order to:
   - Load and preprocess the dataset
   - Convert images to grayscale arrays
   - Implement training functions
   - Create testing functions
   - Evaluate model performance

### Key Implementation Tasks

The notebook includes several key tasks:

1. **Image Preprocessing**: Convert images to grayscale and store as binary arrays
2. **Training Function**: Implement model training pipeline
3. **Testing Function**: Create evaluation and prediction functions
4. **Data Visualization**: Analyze and visualize the dataset

### Example Usage

```python
# Set up paths and parameters
train_messy = "./train/messy"
train_clean = "./train/clean"
test_messy = "./val/messy"
test_clean = "./val/clean"
image_size = 128

# Load and preprocess images
# (Implementation details in the notebook)
```

## 🔬 Implementation Details

### Image Processing Pipeline

1. **Loading**: Images are loaded using PIL (Python Imaging Library)
2. **Preprocessing**: Convert to grayscale and resize to 128x128 pixels
3. **Flattening**: Convert 2D images to 1D arrays for ML processing
4. **Normalization**: Prepare data for machine learning algorithms

### Machine Learning Approach

The project uses a structured approach to:
- **Data Preparation**: Organize images into clean/messy categories
- **Feature Extraction**: Convert images to numerical features
- **Model Training**: Implement classification algorithms
- **Evaluation**: Test model performance on validation data

## 🤝 Contributing

We welcome contributions to improve this project! Here's how you can contribute:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Areas for Contribution
- Improve image preprocessing techniques
- Implement different ML algorithms
- Add data augmentation strategies
- Enhance visualization capabilities
- Optimize model performance
- Add comprehensive testing

## 👨‍🏫 Project Mentors

<h1 align="center">Project Mentors</h1>
<p align="center">
<table align="center">
  <tbody>
    <tr>
      <td align="center">
        <a href="https://github.com/SANTHOSH-SACHIN">
          <img alt="" src="https://avatars.githubusercontent.com/SANTHOSH-SACHIN" width="125px;">
          <br>
          <sub><b>Santhosh Sachin</b></sub>
        </a>
        <br>
      </td>
    </tr>
  </tbody>
</table>
</p>

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Thanks to all contributors who help improve this project
- Special thanks to the project mentors for guidance and support
- Inspired by the need for automated room tidiness assessment

---

**Happy Coding! 🚀**

*If you find this project helpful, please give it a ⭐ star!*