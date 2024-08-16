# MLE (Maximum Likelihood Estimator) with Python 

* Utilizing [World Hapiness Report Data](https://worldhappiness.report/data/), this repository tries to deploy MLE estimator through Python.
* 🔗Refer to this [Blog Post](https://ethhong.github.io/statistics/datascience/2024/08/10/Reviewing-MLE-(Maximum-Liklihood-Estimator).html) for detailed review on MLE for Gaussian and Linear Regression.

<img width="762" alt="image" src="https://github.com/user-attachments/assets/2cb09692-865c-4c83-bf8f-8104d768b584">

# Formulation of MLE
* Given that we are estimating the best linear (polynomial) model:

$$
$y = \theta_0 + \theta_ix_1 + ... \theta_nx_n
$$

Log Likelihood for MLE is formulated as: 

$$
\begin{aligned}
\log L(\theta, \sigma^2) &= -\frac{n}{2} \log(2\pi) - n \log(\sigma) \\
&\quad - \frac{1}{2\sigma^2} \left( \sum_{i=1}^n y_i - \theta_0 - \sum_{j=1}^k \theta_j x_{ij} \right)^2 - \frac{\lambda}{2} \sum \theta_i^2
\end{aligned}
$$

Maximizing this likelihood is same as finding Least Square Error with L2 Regularization.
