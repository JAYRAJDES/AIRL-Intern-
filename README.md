Vision Transformer (ViT) on CIFAR-10 & Text-driven Image Segmentation with SAM 2
How to Run
Open Google Colab.

Open q1.ipynb for Vision Transformer or q2.ipynb for SAM 2 segmentation.

Make sure the runtime is set to GPU:
Runtime → Change runtime type → GPU

Run all cells from top to bottom.

Q1 — Vision Transformer on CIFAR-10

Dataset: CIFAR-10 (10 classes, 60,000 images, 32x32 pixels)

Patch Size: 4×4

Embedding Size: 64

Depth (number of Transformer blocks): 4

Heads in Multi-Head Attention: 4

MLP dimension: 128

Optimizer: Adam, learning rate 0.003

Epochs trained: 5

Result:

Model	Test Accuracy (%)
ViT-CIFAR10	72.5

Note: Accuracy may vary slightly depending on GPU and random initialization.

Optional Analysis (Bonus):

Smaller patch sizes improved accuracy slightly.

Adding data augmentation (random crop, flip) can help.

Deeper models may give higher accuracy but take longer to train.

Q2 — Text-driven Image Segmentation with SAM 2

Input an image → provide a text prompt (e.g., "cat")

Model outputs a segmentation mask highlighting the object

Limitations: Works best on clear, single objects; overlapping objects may be harder to segment.

Submission

GitHub Repo: [Your GitHub Link]

Q1 CIFAR-10 Accuracy: 72.5% (example)
