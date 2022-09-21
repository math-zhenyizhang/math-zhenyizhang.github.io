# Stefan Problem

## Stefan  condition

When a change of phase takes place, a *latent heat* is either **absorbed** or **released**, while the temperature of the material changing its phase remains constant.

In the following we denote by $L > 0$ the latent heat per unit of volume (p.u.v.), and neglect for the sake of simplicity any volume change in the material undergoing the change of phase. We also assume the critical temperature of change of phase to be a constant, $\theta_0$.

To be specific, consider at time $t=t_{0}$ a domain $A$ divided by the plane $x_{1}=s_{0}$ into two subdomains. At time $t=t_{0}$ the sub-domain $A_{1}=A \cap \{x_{1}<s_{0} \}$ is filled by water, while $A_{2}=A \cap\left\{x_{1}>s_{0}\right\}$ is filled by ice. In the terminology of problems of change of phase, $A_{1}$ is the liquid phase and $A_{2}$ is the solid phase. The surface separating the two phases is referred to as the interface. Assume also the setting is plane symmetric, that is the temperature $\theta$ is a function of $x_{1}$ only, besides the time $t$, and the interface is a plane at all times. Denote by $x_{1}=s(t)$ the position of the interface at time $t$. Note that, due to the natural assumption that temperature is continuous,

$$
\theta(s(t)+, t)=\theta(s(t)-, t)=\theta_{0}, \quad \forall t .
$$

Assume ice is changing its phase, that is the interface is advancing into the solid phase. Due to the symmetry assumption we stipulate, we may confine ourselves to consider any portion $D$, say a disk, of the interface at time $t_{0}$. At a later time $t_{1}>t_{0}$ the interface occupies a position $s\left(t_{1}\right)>s\left(t_{0}\right)=s_{0}$. The cylinder $D \times\left(s\left(t_{1}\right), s\left(t_{0}\right)\right)$ has been melted over the time interval $\left(t_{0}, t_{1}\right)$ (see Figure 1$)$. **The change of phase has therefore absorbed a quantity of heat**

volume of the melted cylinder $\times$ latent heat p.u.v. $=\operatorname{area}(D)\left(s\left(t_{1}\right)-s\left(t_{0}\right)\right) L$.

The heat must be provided by diffusion, as we assume that no heat source or sink is present. We adopt for heat diffusion Fourier's law

$$
\text { heat flux }=-k_{i} \nabla_x \theta \text {, }
$$

where $k_{1}>0$ is the diffusivity coefficient in water, and $k_{2}>0$ is the diffusivity coefficient in ice (in principle $k_{1} \neq k_{2}$ ). Thus, the quantity of heat in (1.2) must
equal

$$
\begin{array}{r}
\int_{t_{0}}^{t_{1}} \int_{D(t)}\left[-k_{1} \nabla \theta(s(t)-, t) \cdot \mathbf{e}_{1}-k_{2} \nabla \theta(s(t)+, t) \cdot\left(-\mathbf{e}_{1}\right)\right] \mathrm{d} x_{2} \mathrm{~d} x_{3} \mathrm{~d} t= \\
\operatorname{area}(D) \int_{t_{0}}^{t_{1}}\left[-k_{1} \theta_{x_{1}}(s(t)-, t)+k_{2} \theta_{x_{1}}(s(t)+, t)\right] \mathrm{d} t .
\end{array}
$$

Equating the two quantities, dividing the equation by $t_{1}-t_{0}$ and letting $t_{1} \rightarrow t_{0}$, we finally find

$$
-k_{1} \theta_{x_{1}}(s(t)-, t)+k_{2} \theta_{x_{1}}(s(t)+, t)=L \dot{s}(t),
$$

where we have substituted $t_{0}$ with the general time $t$, as the same procedure can be obviously carried out at any time. This is called the Stefan condition on the free boundary. We stress the fact that the Stefan condition is merely a law of **energetical balance**.

## The free boundary problem

$$
\begin{cases}
&c_{1} \theta_{t}-k_{1} \theta_{x x}=0, \quad \text { in } Q_{1}\\
&c_{2} \theta_{t}-k_{2} \theta_{x x}=0, \quad \text { in } Q_{2}, \quad \text {  }\\
&-k_{1} \theta_{x}(0, t)=h_{1}(t), \quad 0<t<T, \quad \text { }\\
&-k_{2} \theta_{x}(d, t)=h_{2}(t), \quad 0<t<T, \quad \text {  }\\
&-k_{1} \theta_{x}(s(t)-, t)+k_{2} \theta_{x}(s(t)+, t)=L \dot{s}(t), \quad 0<t<T,\\
&\theta(s(t)-, t)=\theta(s(t)+, t)=\theta_{0}, \quad 0<t<T,\\
&s(0)=b .
\end{cases}
$$

Neumann Boundary Conditions

### Enthalpy Method

The *two-phase Stefan problem* can be expressed as a heat conduction problem in a semi-infinite slab geometrically represented by $I=(0, \infty)$. We set $Q=I \times[ 0, \infty]$. The generic point in $I$ is denoted by $x$ and the generic time is $t$. The slab is initially solid at the temperature $T(\cdot, 0)=0$. It is then gradually melted by imposing the temperature $T(0, \cdot)$ to a fixed value $T_{1}$, larger than the melting temperature $T_{m}$. We have $T_{1}>T_{m}>0$. We therefore introduce the enthalpy function,

$$
E(T)=\lambda T+L f(T),
$$

where $f(\theta)$ is the fraction of liquid phase at the temperature $\theta$. There is a range of the possible values of $f$ at the fusion temperature $T_{m}$. Hence, $f$ is multi-valued and is defined by

$$
f(\theta)= \begin{cases}0 & \theta<T_{m} \\ {[0,1]} & \theta=T_{m} \\ 1 & \theta>T_{m}\end{cases}
$$

We have set

$$
\lambda=(\rho C) \kappa^{-1}, \quad L=\left(\rho L_{a}\right) \kappa^{-1},
$$

where $L_{a}$ is the latent heat of fusion, the density $\rho$, the specific heat capacity $C$ and the conductivity $\kappa$ are to have the same values in the solid and liquid phases. This choice is made only by the desire to simplify the exposition. The overall results we develop here extend as well to account for different options, at the cost of more technical calculations.
The temperature distribution is a solution of the following enthalpy problem: Find $(T, H)$ with $H \in E(T)$ and

$$
\begin{cases}
\begin{aligned}
\partial_{t} H-\partial_{x x} T &=0 & \text { in } Q, \\
T(0, \cdot)=T_{1}, & \text { on } T(0, \infty)=0 \\
T(\cdot, 0) &=0 & \text { on } I .
\end{aligned}
\end{cases}
$$

The notation $T(\infty, \cdot)$ should be taken in the sense of the limit $x \rightarrow \infty$. This is the two-phase Stefan problem that can be formulated as a free boundary problem. Considering $X(t)$ as the melted depth of the solid phase which is a function of time; the Stefan problem consists of finding $(T, X)$ such that

$$
\begin{cases}
\begin{aligned}
&\lambda \partial_{t} T-\partial_{x x} T=0 \quad \text { in }(0, X(t)) \times(0, \infty) \text {, }\\
&\lambda \partial_{t} T-\partial_{x x} T=0 \quad \text { in }(X(t), \infty) \times(0, \infty) \text {, }\\
&X(0)=0, \quad T(X(t), t)=T_{m}, \quad L\left(\partial_{t} X\right)(t)=\left[\partial_{x} T\right](X(t), t), \quad \text { in }(0, \infty),\\
&T(0, \cdot)=T_{1}, \quad T(\infty, \cdot)=0 \quad \text { on }(0, \infty) \text {, }\\
&T(\cdot, 0)=0 \quad \text { on } I \text {. }
\end{aligned}
\end{cases}
$$
