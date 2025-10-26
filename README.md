COMVER: Compositional Framework for Visual Grounding via LLM-Driven Decomposition and Verification

COMVER is a compositional visual grounding framework that leverages Large Language Models (LLMs) to decompose textual prompts into structured scene graphs and Grounding DINO for object detection and verification. The system generates both **visual explanations** and **confidence scores** for grounded objects in an image.

This repository contains a fully functional Colab-ready implementation for verifying textual prompts like `"a person in a red shirt"`.

---

## Features

LLM-driven decomposition: Converts free-form text prompts into structured JSON scene graphs containing target objects, attributes, and relationships.
Object detection with Grounding DINO:** Detects objects and their attributes in an image using state-of-the-art object detection models.
Compositional verification:** Verifies object existence and spatial relationships, producing a composite confidence score.
Visual explanations:** Generates annotated images with bounding boxes and textual summaries.
Flexible and extensible:** Easily adaptable for different prompts, images, or LLM/object detection backbones.





Installation

This repository is Colab-ready. Simply run the notebook, and the required libraries will be installed automatically.

**Manual Setup (optional):**

```bash
git clone https://github.com/your-username/comver.git
cd comver
pip install transformers==4.40.1 torch accelerate einops pillow requests
