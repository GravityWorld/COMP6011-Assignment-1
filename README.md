# DISCLAIMER

This project uses the TwinLiteNet+ implementation from:
https://github.com/chequanghuy/TwinLiteNetPlus

I did NOT author the original model or code.

Modifications made: 
- Updated demo.py lines 50-57 for stable inference
- Fixed dimension mismatch between segmentation masks and input images
- Added resizing/cropping to ensure compatibility with SydneyScapes dataset


These changes were necessary to run the model on a dataset different from the one it was originally trained on (BDD100K).
Dataset tested with this code is: SydneyScapes

# Project Setup and Installation Guide

This guide will walk you through setting up a dedicated Python environment and installing all required dependencies to ensure the project runs smoothly.

---
## Running the code

1. Create and activate a Python environment (recommended):
    
    Set the command line to TwinNetPlus_MODIFIED before proceeding.

	```bash
	python -m venv .venv
	source .venv/bin/activate  # on macOS/Linux
	```

2. Install dependencies (from the repository root, which contains `requirements.txt`):

	```bash
	pip install -r requirements.txt
	```

3. Run the command used to test images on the TwinNetPlus - Nano model: (or refer to README inside TwinNetPlus_MODIFIED for more commands)
    
	```bash
    python demo.py --config 'nano' --weight 'models/nano.pth' --source 'test/'
    ```