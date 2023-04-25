# Stable Diffusion Prompt Optimizer

This colab notebook (https://colab.research.google.com/drive/1nCoa55cm8JpIXxBW9RaVSvb8B1WO2ZFz?usp=sharing) is an attempt to automatically optimize stable diffusion prompts.

## Rationale

The rationale is that for a good prompt, you need to have the objects, art movement, art medium, artists, and flavor modifiers.

For all these tags, the closer they are, the most harmonious they are and thus produces higher quality images from stable diffusion. For example, for an impressionism painting (an art movement), it pairs well with Claude Monet, Edouard Manet, Pierre-Auguste Renoir (artists), oil paiting (medium), and unblended color and natural lights (flavors).

## Process
To do this process automatically, I did the following:
1. Collected lists of art movements, artists, art medium, and flavors tags that work in stable diffusion.
2. Turn them into vector embeddings with pre-trained embeddings.
3. Compare them with the user's existing tags to find art movements, artists, art medium, and flavors to add to the prompt.

## How to use
To use the notebook, if you just need to optimize your prompt, you can run the second section.

If you want to create your own lists and embeddings, you can refer to the first section.
