# PINN
Physics Informed Neural Networks
---

# Theory

Newtons Second Law :- Any change in the motion of body is directly proportional to the force acting on it and that this change in movement always takes place in the same direction in which force acts

---

$$m \ddot{x} = - \mu \dot{x} - kx$$

$$\ddot{x} + {\mu \over m}\dot{x} + {k \over m} x = 0$$

$$\ddot{x}+\frac{\mu}{m}\dot{x}+\frac{k}{m}x=0 $$
which is a linear, homogenous second order differential equation with constant co efficients

Let $$x(t)=Ce^{\lambda t}$$

$$\dot{x} (t)=\lambda Ce^{\lambda t}$$

$$\ddot{x} (t)=\lambda^{2} C e^{\lambda t}$$

$$\lambda^{2} C e^{\lambda t} + \frac{\mu}{m} \lambda Ce^{\lambda t} + \frac{k}{m}Ce^{\lambda t}=0$$

$$\lambda^2 + \frac{\mu}{m} + \frac{k}{m}=0$$

Solution for above equation is:-
$$\lambda_{1,2} = - \frac{ \frac{\mu}{m} \pm \sqrt {\Big( \frac{\mu}{m} \Big)^2-4 \Big(\frac{k}{m}\Big)}}{2} $$

$$\lambda_{1,2} = - \frac{\mu}{2m} \pm \sqrt{\Big( \frac{\mu}{2m}\Big)^2 -\frac{k}{m}}$$

Let $$\delta = \frac{\mu}{2m} \space\space, \omega_{0} = \sqrt{\frac{k}{m}}$$

Thus $$\lambda_{1,2} = -\delta \pm \sqrt{\delta^2 - \omega_{0}^2}$$

General Solution is of the form $$x(t) = C_{1}x_{1} (t) + C_{2}x_{2} (t)$$



---

# References

[Physics-informed learning of governing equations from scarce data](https://arxiv.org/abs/2005.03448)

[Finite Basis Physics-Informed Neural Networks (FBPINNs): a scalable domain decomposition approach for solving differential equations](https://arxiv.org/abs/2107.07871)

https://benmoseley.blog/my-research/so-what-is-a-physics-informed-neural-network/

