# CentraleSupélec - Fine-tuning a Pre-trained Neural Network Classifier with LoRA

Romain MONDELICE - Yanis CHAMSON

This repository contains code and resources for fine-tuning a pre-trained neural network classifier on a subset of the MNIST dataset containing digits 0 to 4. The objective is to compare the test accuracy of the baseline model, obtained by optimizing all weights, versus fine-tuning using Low-Rank Adaptation (LoRA).

## Repository Structure

The repository is organized as follows:

- `notebook/`: Jupyter notebooks with the code for fine-tuning the neural network classifier and evaluating the results.
- `models/`: Directory to store the pre-trained model.
- `data/MNIST/raw/`: Directory to store the MNIST dataset.

## Dataset

The MNIST dataset is used for this project. It consists of a large collection of handwritten digit images. For this specific task, only a subset of the dataset containing digits 0 to 4 is utilized. The dataset should be placed in the `Data/MNIST/raw/` directory.

## Neural Network Architecture

The neural network architecture used in this project is artificially large to simulate the scenario where LoRA is typically applied to Large Language Models with billions of parameters. The specific architecture details can be found in the Jupyter notebooks located in the `notebook/` directory.

## Fine-tuning Approaches

Two fine-tuning approaches are explored in this project:

1. **Baseline Model**: The pre-trained neural network classifier is fine-tuned by optimizing all weights using standard training techniques.

2. **LoRA**: Low-Rank Adaptation (LoRA) is applied to fine-tune the pre-trained neural network classifier. LoRA is a technique that adapts the model by learning a low-rank update to the weights, reducing the number of trainable parameters while maintaining performance.

## Results and Comparison

The test accuracy of the baseline model and the LoRA-based fine-tuned model will be evaluated and compared. The results and analysis can be found in the Jupyter notebooks located in the `notebook`.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- We used the LoRA technique that is based on the paper "LoRA: Low-Rank Adaptation of Large Language Models" [https://arxiv.org/pdf/2106.09685.pdf].