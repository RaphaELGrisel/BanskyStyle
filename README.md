# Deep Leaning Project

Implementation of a text to image difusion model to generate Banksy-style images 

## Pipeline : 

### Data preprocessing :
    -Collect Banksy artwork and other similar streetart
    -Textual annotation : each images have to be associated with a textual description like "Little girl holding a heart shaped balloon"
    -Image rescaling, and data augmentation

### Backbone architecture:
    -Chose an existing model

### Fine-tuning:
    -Adapt the latent space : add a textual conditioning specified to capture 
    -Fine-tune the stable diffusion model
    -Adjust hyper-parameters to avoid overfitting
    -Add a attention mechanism to ensure texte influence the image generation
    -Use cross-attention layers (link text and image)

### Model evaluation:
    -Qualitative evaluation
    -FID (Fréchet Inception Distance) : measure distance between dataset distribution and generated images distribution
    -CLIPScore : evaluate correspondace between text and images

## GUI : 
    -User interface : text prompt and image output