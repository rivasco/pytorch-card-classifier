# PyTorch Card Classifier

A multiclass neural network for card recognition using PyTorch.

## Overview

Covers three main parts:  
- Using PyTorch datasets and data loaders  
- Defining a PyTorch model with a pretrained backbone  
- Setting up a training loop

## Steps

1. **Dataset**  
   Organize your data for PyTorch and use data loaders for batching and shuffling.

2. **Model**  
   - Use a pretrained model from `timm` or similar.  
   - Modify the final layer for 53 targets.  
   - Structure:
     - `self.base_model` – full pretrained model  
     - `self.features` – backbone layers  
     - `self.classifier` – new head  
   - Connect layers in `forward`.

3. **Training Loop**  
   Standard PyTorch loop with loss calculation, backpropagation, and optimizer steps.
