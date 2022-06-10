# Hill2D
 Families of periodic solutions to the plain Hill problem

## Short description 

The Hill’s problem is a certain limiting case of the 
restricted three body problem (RTBP), and it is 
used for studying dynamics of a zero mass body (satellite) in the vicinity of a minor of two gravitating bodies. 
If two massive bodies rotate uniformly in circular orbits 
relative to their common center of mass, the problem 
is called circular. 

The Hamilton function for the planar circular Hill’s problem 
$H(\mathbf x,\mathbf y)=\frac12\left(y_1^2+y_2^2\right)+x_2y_1-x_1y_2-x_1^2+\frac12x_2^2-\dfrac1r,\quad r=\sqrt{x_1^2+x_2^2}$, where
$\mathbf x=(x_1,x_2)$ is the coordinates vector, а $\mathbf y=(y_1,y_2)$ is the conjugate momenta vector.

Canonical equations of motion 

$\dot x_1=y_1+x_2, \dot y_1=y_2+2x_1-\dfrac{x_1}{r^3}$,

$\dot x_2&=y_2-x_1, \dot y_2=-y_1-x_2-\dfrac{x_2}{r^3}$.

Equations of motion have a single first integral 
which is traditionally written in the form of Jacobi 
integral in variables $(\mathbf x,\dot{\mathbf x})$:
$\mathcal J=3x_1^2+\dfrac{2}{r}-\dot x_1^2-\dot x_2^2=C$, 
where $C$ is the Jacobi constant.

Equations of the Hill’s problem are invariant 
with respect to a finite group of linear transformations 
of phase variables $(\mathbf х,\mathbf у)$ and time $t$: 
* $\Sigma_1: (t,x_1,x_2,y_1,y_2)\to(-t,x_1,-x_2,-y_1,y_2)$
* $\Sigma_2: (t,x_1,x_2,y_1,y_2)\to(-t,-x_1,x_2,y_1,-y_2)$
* $\Sigma_{12}: (t,x_1,x_2,y_1,y_2)\to(t,-x_1,-x_2,-y_1,-y_2)$

All periodic solutions to the Hill’s problem can be divided in three groups depending on their paradigm 
of changes under the action of the above transformations:

* *asymmetric solutions*, which go over into other 
solutions under the action of any of above transforma 
tions;
* *singly symmetric* solutions that pass into itself under 
the action of one of the above transformation, while 
two other transformations allow one to obtain one 
more new solution;
* *doubly symmetric* solutions that are invariant with 
respect to any of the above transformations.

With regard to the behavior  at 
continuation over parameter С, all families of periodic 
solutions can be conventionally divided in several 
groups: 

* *Closed families* exist only on a certain finite interval 
of the С parameter.
* *Halfopen families* exist on a semiinfinite interval 
of С parameter values. They can be continued either 
until contraction to a point or to the end on another 
family, or until reaching an extreme value in С.
* *Open families* that exist at any values of С.

Since all such families are continued in parameter 
С up to their natural terminations, all of them are *natural families*.

Here we provide data of initial conditions to some families of periodic orbits of the planar circular Hill's problem. 

## Description of the data
Data for each family is placed into its own directory.  
Initial data is stored into the file with .dat extension. 
The first row describes the columns according to the symmetry of the family.


| Column name | $\Sigma_1$-symmetric | $\Sigma_2$-symmetric |
|:------------|:--------------------:|:--------------------:|
| No          | number of row        | number of row        |
| x0,py0 (y0,px0)     | $x(0), py(0)$        | $y(0), px(0)$        |
| T           | period               | period               | 
| C           | Jacobi integral | Jacobi integral |
| Stab        | stability index | stability index |
| xh,pyh (yh,pxh)| $x(T/2), py(T/2)$        | $y(T/2), px(T/2)$     |
