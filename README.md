# Robust Defenses Against Physically Realizable Attacks on Image Classification

This repository contains the code and resources for our project "Robust Defenses Against Physically Realizable Attacks on Image Classification." Our work builds upon and improves the base model presented in the [original research](https://arxiv.org/abs/1909.09552).

## Overview

In this project, we develop enhanced defense mechanisms to improve the robustness of image classification models against physically realizable attacks. We specifically target the adversarial robustness on datasets such as MNIST and CIFAR10. Our improvements demonstrate significant gains in both test accuracy and adversarial accuracy compared to the base model.

## Improvements

The original base model can be found in this [Colab Notebook](https://colab.research.google.com/gist/tongwu2020/bbf836348be405f3bebe96d0ea12df43/roa-doa_test.ipynb). We have made substantial improvements over the original model, yielding the following results:

| Dataset | Model                | Test Accuracy | Adversarial Accuracy | Attack Size |
|---------|----------------------|---------------|----------------------|-------------|
| MNIST   | [1] model            | 81.80%        | 41.26%               | 10x10       |
| MNIST   | Our proposed model   | 89.45%        | 72.80%               | 10x10       |
| CIFAR10 | [1] model            | 15.10%        | 10.50%               | 10x10       |
| CIFAR10 | Our proposed model   | 16.80%        | 12.00%               | 10x10       |

**Table 2: Results**

## Project Structure

- `data/`: Contains the datasets used for training and evaluation.
- and .py files

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/sadam452/Robust-Defenses-Against-Physically-Realizable-Attacks-on-Image-Classification.git
    cd Robust-Defenses-Against-Physically-Realizable-Attacks-on-Image-Classification
    ```

2. **Install the required dependencies**:
    ```bash
    Installation commands are written in python script.
    ```

3. **Run the training script**:
    Base model on Cifar10: 
    ```bash
    python cifar10Base.py
    ```
    Our improved model on Cifar10: 
    ```bash
    python cifar10Final.py
    ```
    Base model on MNIST: 
    ```bash
    python Mnist_Base.py
    ```
    Our improved model on MNIST: 
    ```bash
    python Mnist_Final.py
    ```

4. **Evaluate the model**:
    ```bash
    When you run the python script, evaluation results will be displayed as well.
    ```
## Report
- You can read the detailed report [here](/report.pdf)
## Citation

If you use this code or the provided models in your research, please cite the original paper:

```
@article{DBLP:journals/corr/abs-1909-09552,
  title={Defending Against Physically Realizable Attacks on Image Classification},
  author={Tong Wu, et al.},
  journal={CoRR},
  volume={abs/1909.09552},
  year={2019},
  url={http://arxiv.org/abs/1909.09552},
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

We would like to thank the authors of the original paper for providing their foundational work and base model for this research. 

For any questions or collaborations, please contact [Sadam](https://www.github.com/sadam452).

---

Feel free to fork this repository and contribute to the project!