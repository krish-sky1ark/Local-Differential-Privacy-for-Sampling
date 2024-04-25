# Local Differential Privacy for Sampling

---

Local Differential Privacy (LDP) is a privacy protection technique where individuals inject random noise into their data before sharing it.</br>
We propose a novel LDP method for sampling, based on a boosting-based density estimation algorithm. The idea is to learn a sampler that can produce synthetic data points from the distribution of each individual, while satisfying LDP. The results metrices discussed are Negative Log Likelihood and Mode Coverage.

---

## Features

1. **Boosting-based Density Estimation:** The code implements a boosting algorithm for density estimation, where a weak learner, represented by a Multi-Layer Perceptron (MLP) classifier, is trained iteratively to improve the estimate of the target distribution.
   
2. **Local Differential Privacy (LDP) Support:** The boosting algorithm is designed to ensure local differential privacy (LDP), a privacy-preserving technique where individuals add noise to their data before sharing it. This allows for the generation of synthetic datasets while protecting the privacy of individual data points.
   
3. **Synthetic Dataset Generation:** After training the boosting algorithm, a synthetic dataset is generated based on the final estimate of the target distribution. This synthetic dataset closely approximates the original dataset while preserving privacy guarantees.


---

## Installing Dependencies

- Python 3.x
- NumPy
- Matplotlib
- TensorFlow
- Sklearn
- Scipy
- Keras
- Pandas

## Getting Started and How to Use

1. Install the above mentioned Dependencies
2. If Dataset is present for applying LDP, Specify the path of the dataset in place of original dataset in the implementation cell of the code file LDP_forsampling.ipynb and use appropriate measures to read its content.
3. In case datset is not present, run the code file LDP_forsampling.ipynb as it is, a random dataset will be picked up as original dataset in the Implementation cell of the code.
4. Run all the cells in the code file after specifying the dataset.

---

## Conect with me:
- LinkedIn: [LinkedIn Profile]( https://www.linkedin.com/in/krish-khadria-034401271/)
- GitHub: [GitHub Profile](https://github.com/krish-sky1ark)

---

## Acknowledgements

- We are thankful to Hisham Husain, Borja Balle, Zac Cranko and  Richard Nock for making available their valuable research. Insights of this project has been taken from the research paper "Local Differential Privacy for Sampling" http://proceedings.mlr.press/v108/husain20a/husain20a.pdf .
