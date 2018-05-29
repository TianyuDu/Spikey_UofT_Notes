### Chapter 7: Introduction to Simple Regression

#### On Population

​	$N$ = Size

​	$x$ = Independent(explanatory) variable

​	$y$ = Dependent(response) variable.

**Question**: Does and how does $y$ dependent on $x$ ?

​	i.e. Is $y$ a function of $x$ ?

Select a randome *sample* from the population.

#### On Sample

​	$n$ = size

​	Observations are $\{x_1, \dots , x_n\}$ and $\{y_1, \dots , y_n\}$ (**sample data**)

|    i     |    x     |    y     |
| :------: | :------: | :------: |
|    1     |  $x_1$   |  $y_1$   |
|    2     |  $x_2$   |  $y_2$   |
| $\vdots$ | $\vdots$ | $\vdots$ |
|    n     |  $x_n$   |  $y_n$   |

#### Visualization

Plot $(x_i,y_i)$ in a **scatter diagram**, with a fitted linear line.

![image-20180522143347166](/var/folders/0p/f6j25qz17l7gx64mk8c1q5300000gn/T/abnerworks.Typora/image-20180522143347166.png)

Let $f$ denote the fitted linear function, then consider an explanatory data $x_i$ we denote the predicted value from the linear fitting as

$y_i$ := the **actual** value at $x_i$

$\hat{y_i} = f(x_i)$ := the **estimated** $y$ value at $x_i$

$e_i$ = $y_i - \hat{y_i}$ := the **error** of $y$ value at $x_i$ also referred as **residual**

However the total error $\sum_{i=1}^n {e_i} = 0 $

To formalize the optimization problem, consider **sum of squared error(SSE)**, also referred as **sum of squared residual(SSR)**

$SSE = \sum_{i=1}^n{e_i^2}$

*The line minimize the **SSE** is the best line to relate $x$ and $y$.*

Let the fitted linear line be represented as

$\hat{y} = b_0 + b_1 x$

**Motivation** Find $b_0$ and $b_1$ to minimize *SSE*.

Consider:

$SSE = \sum_{i=1}^n{e_i^n} = \sum_{i=1}^n {(y_i - \hat{y_i})^2} = \sum_{i=1}^n{(y_i - b_0 - b_1 x_1)^2}$

Solve equations for first order conditions for minimization

$\begin{cases} \frac{d}{db_0}SSE=0 \\ \frac{d}{db_1}SSE = 0\end{cases}$

Solution;

$\begin{cases} b_0 = \frac{\sum{(x_i - \overline{x}) (y_i - \overline{y})}}{\sum_{i=1}^n{(x_i - \overline{x})^2}} \\ b_1 = frac{}\end{cases}$

OLS

#### Analysis of Variance(ANOVA)

$y_i$:= actually $y$ value at $x_i$

$\hat{y_i}$:= estimated $y$ value at $x_i$

$y_i - \overline{y} = (\hat{y_i} - \overline{y}) + (y_i - \hat{y_i})$

Therefore $(y_i - \overline{y})^2 = ()$