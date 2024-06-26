# Inverse Kinematics for Robot Arms with Python
This is a simple model to visualize the trajectory of a two-arm robot finding its target through inverse kinematics process using simple gradient method.

## Simple Gradient Algorithm
while $`dist(T - E)`$ > tolerance:\
&emsp;$`\theta^{i+1}_{1} = \theta_1^{i} + J_1(\theta)`$\
&emsp;$`\theta^{i+1}_{2} = \theta_2^{i} + J_2(\theta)`$\
&emsp;calculate $`E(\theta_{1}, \theta_{2})`$    
end

- $` J_{1}(\theta) = dist(T - E(\theta_{1}-\Delta\theta, \theta_{2})) - dist(T - E(\theta_{1}+\Delta\theta, \theta_{2})) `$
- $` J_{2}(\theta) = dist(T - E(\theta_{1}, \theta_{2}-\Delta\theta)) - dist(T - E(\theta_{2}, \theta_{2}+\Delta\theta)) `$
- $` dist()`$ refer to euclidean distance between two given points


## Example
![](https://github.com/thiofahr/Inverse-Kinematics-for-Robot-Arms/blob/main/two-arms-robot.gif)
