# introduction## classification of ML- Regression- Binary Classification- Multi-class Classification- Generation- supervised learning- unsupervised learning- meta learning- reinforcement learning- life-long learning# Linear Regression*linear model* 　　 　　![](./formula/9.png)  *loss function*　　 　　![](./formula/10.png)  <font color=#FF0000> overfitting :  A more complex model does not always lead to better performance on test data</font>Regularization : 　　　![](./formula/8.png)  <font color=#1E90FF> Regularization make the function more smoother to reduce the effects of noise.</font>   ## bias&variances![](./img/bias&variances.PNG)  generally speaking,the more complex linear regression model have lower bias and higher variance,the more simpler model have higher bias and lower variance.so the complex model usually overfitting,the simple model usually underfitting.  
<font color=#FF0000> how to deal overfitting?  
1.more data  
2.regularization</font>
## Gradient Descent Tips- reduce the learning rate by every few epoch.
　　　　　　　　　　　　　　　![](./formula/7.png)  
- learnig rate cannot be one-size-fits-all.
giving different paramenters different learning rate.
　　　　　　　　　　　　　　　![](./formula/6.png)  
　　　　　　　　　　　　　　　![](./formula/5.png)  
　　　　　　　　　　　　　　　![](./formula/4.png)  
- Stochastic Gradient Descent
pick an example x<sup>n</sup> in the model.
- Feature Scaling
# Classification
### Bayes formula
In the Binary Classification,the Bayes formula as follow:
　　　　　　　　　　　　　　　![](./formula/2.png)  
if the probability is greater than 0.5 output Class one,else output Class two.
### Gaussion Distribation
function of Gaussion Distribation:
　　　　　　　　　　　　　　　![](./formula/1.png)  
input:vector x,output:probability of sampling x. The shape of the function determines by mean u and vavariance matrix ∑.
we have class one feature:x<sub>1</sub>,x<sub>2</sub>,x<sub>3</sub>,....x<sub>n</sub>,we assume x<sub>1</sub>,x<sub>2</sub>,x<sub>3</sub>,....x<sub>n</sub> generate from the Gaussion function(u<sup>^</sup>,∑<sup>^</sup>).
　　　　　　　　　　　　　　　![](./formula/3.png) 
　　　　　　　　　　　　　　　![](./formula/11.png)
result:
　　　　　　　　　　　　　　　![](./formula/12.png)
　　　　　　　　　　　　　　　![](./formula/13.png)
simplify the Bayes formula:
　　　　　　　　　　　　　　　![](./formula/14.png)
　　　　　　　　　　　　　　　![](./formula/15.png)
so,the final formula as follow:
　　　　　　　　　　　　　　　![](./formula/17.png)
　　　　　　　　　　　　　　　![](./formula/18.png)
the Logistic Regression formula:
　　　　　　　　　　　　　　　![](./formula/19.png)
how to do gradient descent for Logistic Regression?
- Training data:

|x<sub>1| x<sub>2 | x<sub>3 | x<sub>n |
| -- | -- | -- | -- |
| C<sub>1 | C<sub>1 | C<sub>2 | C<sub>1 |
Assume the data is generated based on ![](./formula/20.png),the Loss function as follow:
　　　　　　　　　　　　　　　![](./formula/21.png)
　　　　　　　　　　　　　　　![](./formula/22.png)
　　　　　　　　　　　　　　　![](./formula/23.png)
the loss function final is a bernoulli distribution
　　　　　　　　　　　　　　　![](./formula/24.png)
### multi-class classification
multi-class classification will use the softmax function:
　　　　　　　　　　　　　　　![](./formula/25.png)
cascading Logistic Regression models become Neural Network
　　　　　　　　　　　　　　　![](./img/cascading_logistic_regression.png)
The function of a layer of logistic regression is to transform the data into features .
