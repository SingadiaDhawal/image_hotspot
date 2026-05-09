# AI Image Hotspot Detection

Interactive AI-powered image hotspot detection system that allows users to upload images, detect objects, and interact with detected regions using clickable hotspots.

The system identifies objects such as lamps, chairs, bottles, people, laptops, and more directly inside images.

Supports:
- YOLOv8 Version
- OWL-ViT Free Open Source Version

---

# Demo Features

- Upload Image
- Automatic Object Detection
- Interactive Click-Based Hotspots
- Bounding Box Visualization
- JSON Detection Output
- AI Generated Image Support
- Gradio Web Interface
- Google Colab Compatible

---

# Project Preview

## Object Detection

- Detects multiple objects inside uploaded image
- Draws bounding boxes
- Displays object labels and confidence scores

## Hotspot Detection

- Click on any detected object
- System identifies selected object
- Returns object metadata and coordinates

---

# Supported Models

| Model | Type | Free | Use Case |
|---|---|---|---|
| YOLOv8 | CNN Detector | Yes | Fast object detection |
| OWL-ViT | Transformer Detector | Yes | Open vocabulary detection |
| Grounding DINO | Vision Transformer | Yes | Advanced detection |
| SAM | Segmentation | Yes | Pixel-level masking |

---

# Tech Stack

## Frontend

- Gradio

## Backend

- Python

## AI/ML

- YOLOv8
- OWL-ViT
- HuggingFace Transformers
- PyTorch

## Image Processing

- OpenCV
- PIL

---

# Folder Structure

```text
project/
│
├── image_hotspot.py
├── requirements.txt
├── README.md
├── assets/
│   └── sample_images/
│
└── outputs/
```

---

# Installation

## YOLOv8 Version

```bash
pip install ultralytics gradio opencv-python pillow
```

## OWL-ViT Version

```bash
pip install transformers torch torchvision pillow gradio timm
```

---

# Run Project

```bash
python image_hotspot.py
```

OR run directly in Google Colab.

---

# Google Colab Support

This project works directly inside Google Colab.

After execution:

```text
Running on public URL:
https://b30aa80ce40a8301c4.gradio.live/
```

Open the generated Gradio URL in browser.

---

# How It Works

## Step 1 — Upload Image

User uploads:
- Real image
- AI-generated image
- Indoor scene image
- Object image

---

## Step 2 — Object Detection

AI model:
- scans image
- detects objects
- generates bounding boxes

---

## Step 3 — Hotspot Creation

Detected objects become clickable regions.

Each hotspot stores:
- label
- confidence score
- coordinates

---

## Step 4 — User Interaction

User clicks object region.

System:
- checks clicked coordinates
- matches bounding box
- identifies object

---

# Example Detection Output

```json
[
  {
    "label": "lamp",
    "confidence": 0.96,
    "x1": 120,
    "y1": 90,
    "x2": 220,
    "y2": 310
  },
  {
    "label": "chair",
    "confidence": 0.91,
    "x1": 300,
    "y1": 180,
    "x2": 500,
    "y2": 600
  }
]
```

---

# Example Hotspot Output

```text
Object Found

Name: lamp
Confidence: 0.96

Coordinates:
(120, 90)
(220, 310)
```

---

# Supported Objects

The system can detect:
- Lamp
- Chair
- Table
- Sofa
- Bottle
- Cup
- Laptop
- Phone
- Book
- TV
- Plant
- Fan
- Bed
- Clock
- Person

Depends on selected AI model.

---

# YOLOv8 Version

## Advantages

- Faster inference
- Real-time capable
- Lightweight
- Easy deployment

## Best For

- Webcam detection
- Live systems
- Edge devices
- Fast processing

---

# OWL-ViT Version

## Advantages

- Fully free
- Open vocabulary detection
- Transformer-based architecture
- Better semantic understanding

## Best For

- AI-generated images
- Flexible object queries
- Research projects
- Semantic object search

---

# Future Enhancements

- Hover-Based Detection
- Video Hotspot Detection
- Real-time Webcam Support
- Semantic Search
- CLIP Embeddings
- Vector Database Integration
- Multi-object Tracking
- Segmentation Masks
- Similar Object Search
- ERPNext/Frappe Integration

---

# Deployment Options

- Google Colab
- Local Machine
- HuggingFace Spaces
- AWS EC2
- Docker
- Render
- Railway

---

# Requirements

## Minimum

- Python 3.10+
- 4GB RAM

## Recommended

- GPU Runtime
- CUDA Support
- 8GB+ RAM

---

# License

MIT License

---

# Author

Dhawal Singadia

MSc Computer Science  
AI/ML and Full Stack Development

---

# Acknowledgements

- Ultralytics
- HuggingFace
- Google Research
- Gradio
- PyTorch
