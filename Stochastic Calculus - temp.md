## C5 Risk-Neutral Pricing
$\rightarrow$ $(\Omega,\mathcal{F},\mathbb{P})$ with almost surely positive $Z$ and $\mathbb{E}Z=1$, Radon-Niksodym derivative process: $Z(t)=\mathbb{E}[Z|\mathcal{F}(t)]$ 
$\rightarrow$ $Z(t)$ is a martingale
$\rightarrow$ let $Y$ be $\mathcal{F}(t)$-measurable, $\widetilde{\mathbb{E}}Y=\mathbb{E}[YZ(t)]$
$\rightarrow$ $0\leq s\leq t \leq T$, $Y$ $\mathcal{F}(t)$-measurable, $\widetilde{\mathbb{E}}[Y|\mathcal{F}(s)]=\frac{1}{Z(s)}\mathbb{E}[YZ(t)|\mathcal{F}(s)]$
$\rightarrow$ $W(t)$ Brownian motion, $(\Omega,\mathcal{F},\mathbb{P})$, $\mathcal{F}(t)$, adapted process $\varTheta(t)$, $Z(t)=\text{exp}\{-\int_0^t\varTheta(u)dW(u)-\frac{1}{2}\int_0^t\varTheta^2(u)du\}$, $\widetilde{W}(t)=W(t)+\int_0^t\varTheta(u)du$, with $\mathbb{E}\int_0^T\varTheta^2(u)Z^2(u)du<\infty$, $Z=Z(T)$, then $\mathbb{E}Z=1$ and $\widetilde{W}(t)$ is Brownian motion under $\widetilde{\mathbb{P}}$
$\rightarrow$ BSM formula
$\rightarrow$ martingale representation theorem: $W(t)$, $(\Omega,\mathcal{F},\mathbb{P})$, $\mathcal{F}(t)$, martingale $M(t)$ with respect to $\mathcal{F}(t)$, there is an adapted $\varGamma(u)$ such that $dM(t)=\varGamma(t)dW(t)$
$\rightarrow$ multiple dimensions Girsanov
$\rightarrow$ multiple dimensions martingale representation
$\rightarrow$ risk neutral measure: equivalent and $D(t)S_i(t)$ is martingale
$\rightarrow$ portfolio $X(t)$, arbitrage: $X(0)=0$, $\mathbb{P}\{X(T)\geq 0\}=1$ and $\mathbb{P}\{X(T)>0\}>0$
$\rightarrow$ first fundamental theorem of asset pricing: risk neutral measure exists $\Rightarrow$ no arbitrage
$\rightarrow$ a market model is complete if every derivative security can be hedged
$\rightarrow$ second fundamental theorem of asset pricing: model complete $\Leftrightarrow$ risk-neutral measure unique
$\rightarrow$ note: understanding of the system here: existence and uniquen risk-neutral measure ensures that any asset (V(T) depends on S_i and FT measurable can be hedged(duplicated) and is a martingale), then its price can be determined by the expectations
$\rightarrow$ $\text{For}_S(t,T)=\frac{S(t)}{B(t,T)}$


## C6 Connections with Partial Differential Equations
$\rightarrow$ stochastic differential equation: $dX(u)=\beta(u,X(u))du+\gamma(u,X(u))dW(u)$
$\rightarrow$ $g(t,x)=\mathbb{E}^{t,x}h(X(T))$, $\mathbb{E}[h(X)|\mathcal{F}(t)]=g(t,X(t))$
$\rightarrow$ $g(t,X(t))$ is martingale
$\rightarrow$ Feynman-Kac theorem: $g(t,x)$ satisfies pde $g_t(t,x)+\beta(t,x)g_x(t,x)+\frac{1}{2}\gamma^2(t,x)g_{xx}(t,x)=0$ and terminal condition $g(T,x)=h(x)$ for all $x$
$\rightarrow$ multiple dimension Feynman-Kac

## C7 
## C11 Introduction to Jump Processes
$\rightarrow$ $(\varOmega,\mathcal{F},\mathbb{P})$ with $\mathcal{F}(t)$, Brownian motion $W(t)$ is a BM relative to this filtration if $\sigma(W(t))\subset\mathcal{F}(t)$ and $W(u)-W(t)$ is independent of $\mathcal{F}(t)$, similar for compound Poisson process $Q(t)$
$\rightarrow$ jump process $X(t)=X(0)+I(t)+R(t)+J(t)$ where $I(t)=\int_0^t\varGamma(s)dW(s)$, $R(t)=\int_0^t\varTheta(s)ds$ and $J(t)$ is an adapted, right-continuous, pure jump process(finite jumps in finite interval and constancy otherwise); $X^c(t)=X(0)+I(t)+R(t)$
$\rightarrow$ for adpated $\varTheta(t)$, $\int_0^t\varTheta(s)dX(s)=\int_0^t\varTheta(s)\varGamma(s)dW(s)+\int_0^t\varTheta(s)\varTheta(s)ds+\sum_{0<s\leq t}\varTheta(s)\varDelta J(s)$
$\rightarrow$ if $X(s)$ martingale and $\varTheta(s)$ left-continous, then $\int_0^t\varTheta(s)dX(s)$ is martingale
$\rightarrow$ $[X_1,X_2](T)=\int_0^T\varGamma_1(s)\varGamma_2(s)ds+\sum_{0<s\leq T}\varDelta J_1(s)\varDelta J_2(s)$
$\rightarrow$ $f(X(t))=f(X(0))+\int_0^tf^\prime(X(s))dX^c(s)+\frac{1}{2}\int_0^tf^{\prime\prime}(X(s))dX^c(s)dX^c(s)+\sum_{0<s\leq t}[f(X(s))-f(X(s-))]$
$\rightarrow$ $df(t,X_1,X_2)=f_tdt+f_{x_1}dX_1^c+f_{x_2}dX_2^c+\frac{1}{2}f_{x_1,x_1}dX_1^cdX_1^c+f_{x_1,x_2}dX_1^cdX_2^c+\frac{1}{2}f_{x_2,x_2}dX_2^cdX_2^c\\+f(t,X_1(t),X_2(t))-f(t,X_1(t-),X_2(t-))$
$\rightarrow$ $d(X_1X_2)=X_2dX_1^c+X_1dX_2^c+dX_1^cdX_2^c+X_1(t)X_2(t)-X_1(t-)X_2(t-)\\=X_1(t-)dX_2+X_2(t-)dX_1+dX_1dX_2$
$\rightarrow$ $N(t)$ a Poisson process relatie to $(\varOmega,\mathcal{F},\mathbb{P})$, $Z(t)=e^{(\lambda-\widetilde{\lambda})t}(\frac{\widetilde{\lambda}}{\lambda})^{N(t)}$ $\Rightarrow$ $dZ(t)=\frac{\widetilde{\lambda}-\lambda}{\lambda}Z(t-)dM(t)$
$\rightarrow$ $N(t)$ is $Poisson(\widetilde{\lambda})$ under $\widetilde{\mathbb{P}}(A)=\int_AZ(T)d\mathbb{P}$