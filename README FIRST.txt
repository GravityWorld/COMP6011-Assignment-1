This project uses the TwinLiteNet+ implementation from:
https://github.com/chequanghuy/TwinLiteNetPlus

I did NOT author the original model or code.

Modifications made: 
- Updated demo.py lines 50-57 for stable inference
- Fixed dimension mismatch between segmentation masks and input images
- Added resizing/cropping to ensure compatibility with SydneyScapes dataset


These changes were necessary to run the model on a dataset different from the one it was originally trained on (BDD100K).
Dataset tested with this code is: SydneyScapes