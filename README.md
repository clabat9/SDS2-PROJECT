# A non-linear regression Bayesian model 

![](https://images-na.ssl-images-amazon.com/images/I/51DOVYtpmVL._SX329_BO1,204,203,200_.jpg)

This work is an in-depth fully Bayesian analysis on data that are the result of a NIST study involving circular interference transmittance. The response variable $(Y_i)$ is transmittance $(\in[0,1])$, and the predictor variable $(x_i)$ is wavelength $(cm, \in \mathbb{R}^+)$; there are $N=35$ observations. We decided to consider the following regression model:

$$ Y_i \sim Beta(a_{y_i}, b_{y_i}) \\ \mu_i =\frac{a_{y_i}}{a_{y_i}+b_{y_i}} = f(x_i) = \frac{\beta_1}{\beta_2} \exp\bigg[-\frac{1}{2}\bigg(\frac{x_i-\beta_3}{\beta_2}\bigg)^2\bigg]\\ \sigma_{y_i}^2 = \frac{a_{y_i}b_{y_i}}{(a_{y_i}+b_{y_i})^2(a_{y_i}+b_{y_i}+1)}$$


The complete analysis is in the repository. It is an .html file so you need a reader to read it.
