# mathematica-dynamics
A few physics simulations written in Mathematica notebooks: an arbitrary n-spring system, a double pendulum, and a more complex project comparing relativistic and nonrelativistic charged particle dynamics in electromagnetic fields.
## N-spring system
The motion of a mass on a spring is modeled by Hooke's Law, which states that the spring force F = -kx, the spring constant multiplied by the displacement from equilibrium. When multiple masses are attached by springs in a chain, the spring force on every mass is influenced by the spring on its left and its right, which causes the equations of motion to be "coupled": the motion of each mass must be solved for simultaneously, as the motions of all masses are interdependent. 
The Mathematica notebook file [springdynamics.nb](springdynamics.nb) provides code that generates the set of coupled differential equations governing a series of coupled springs (springs connected in a chain), then integrates these equations to obtain the motion of each spring and animates the result:

![ten spring animation](tenspringanimation.gif)

## Double pendulum
Deriving the equations of motion of a double pendulum is a classic problem in Lagrangian mechanics, a sophomore-level physics topic, and the double pendulum is notable as an example of a chaotic system, meaning that small changes in initial conditions (the angles of the two pendulum rods) cause the resulting trajectories to differ wildly. The notebook [doublependulum.nb](doublependulum.nb) numerically integrates the coupled differential equations describing the system, and returns a manipulable plot which allows one to change the initial conditions and then animate the pendulum. Powerful equation solving tools and a simple implementation of manipulable plots are distinguishing features of the Wolfram language, and this notebook highlights those abilities very well. This animation is for one set of initial conditions:

![double pendulum](doublependulum.gif)

## Relativistic and nonrelativistic particle dynamics in electromagnetic fields
Models of particle motion in electromagnetic fields are commonly used in particle physics and plasma physics, as electromagnetic (EM) fields are the most useful tool for trapping or accelerating charged particles. At low particle velocities, the equations governing the trajectory of a charged particle in an EM field can be solved using standard methods from Newtonian physics, but at extreme speeds, those close to the speed of light <i>c</i>, the effects of Albert Einstein's theory of relativity warp particle trajectories in ways that cannot be explained by Newtonian physics. 

Nonrelativistic (Newtonian) models still have their place in modern physics in low-velocity cases, as they greatly simplify calculations, but at higher velocities, the more complex relativistic models are necessary for accurate calculations. In this project, numerical solvers in Mathematica were used to study the trajectories of charged particles in electromagnetic wave systems, and comparisons between nonrelativistic and relativistic predictions were made.
