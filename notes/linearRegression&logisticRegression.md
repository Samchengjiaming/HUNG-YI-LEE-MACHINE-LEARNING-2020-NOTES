# introduction## classification of ML- Regression- Binary Classification- Multi-class Classification- Generation- supervised learning- unsupervised learning- meta learning- reinforcement learning- life-long learning# Linear Regression *linear model* 　　 y=b+∑w<sub>i</sub>x<sub>i</sub>  *loss function* 　　L=∑(y<sup>^</sup>-y)<sup>2</sup>  <font color=#FF0000> overfitting :  A more complex model does not always lead to better performance on test data</font>Regularization : L=∑(y<sup>^</sup>-y)<sup>2</sup>  +λ∑(w<sub>i</sub>)<sup>2</sup>  <font color=#1E90FF> Regularization make the function more smoother to reduce the effects of noise.</font>   ## bias&variances![](./img/bias&variances.PNG)generally speaking,the more complex linear regression model have lower bias and higher variance,the more simpler model have higher bias and lower variance.so the complex model usually overfitting,the
simple model usually underfitting.  
<font color=#FF0000> 
how to deal overfitting?  
1.more data  
2.regularization
</font>
## Gradient Descent Tips  - reduce the learning rate by every few epoch  
$$
n^t=\frac{n}{\sqrt{t+1}}
$$
- learnig rate cannot be one-size-fits-all