# NanoGPT Shakespeare Character-Level Model Experiment

Experiment training Andrej Karpathy's nanoGPT model on the Shakespeare dataset for character-level text generation. Used Google Colab with a T4 GPU.

## Overview

*   **Model:** nanoGPT (character-level configuration)
*   **Dataset:** Shakespeare (from `data/shakespeare_char/prepare.py`)
*   **Environment:** Google Colab (GPU: T4 - *or whatever GPU you got*)
*   **Training Iterations:** Trained for approximately 1290 iterations (stopped early).
*   **Colab Notebook:** [shakespeare_char_training.ipynb](shakespeare_char_training.ipynb) (*Update the filename if you changed it*)

## Training Details

The model was configured as per `config/train_shakespeare_char.py` in the nanoGPT repository, with the exception that `compile=False` was used due to compatibility issues with `torch.compile` on the Colab GPU.

*   Final (approximate) training loss at 1290 iterations: ~1.29
