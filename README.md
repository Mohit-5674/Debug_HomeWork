

Debug Challenge 

What was the bug? The main issues were that y_test was generated as boolean values instead of integers, the learning rate was too high, and the cost function was numerically unstable due to log(0).

How did you identify it? I identified the bug by observing unstable loss values and checking the datatype of y_test. I also noticed that the learning rate was too large and that the cost function could produce NaN values.

Why did it cause the specific problem? Boolean labels caused incorrect accuracy calculations, the high learning rate caused gradient descent to diverge, and log(0) produced numerical errors, leading to unstable training.

What learning rate worked best? 0.01

What accuracy did you achieve? Train: ~55% Test: ~50%

Mohit Kumar
