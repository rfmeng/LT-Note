## Chapter 1
$\rightarrow$ sample space $\Omega$ 
$\rightarrow$ $\sigma$-algebra and probability function $\mathbb{P}$
$\rightarrow$ X is random variable if $\{X\in B\}=\{w\in \Omega \mid X(w)\in B\}\in \mathcal{F}$
$\rightarrow$ distribution measure: $\mu_X$ with $\mu_X(B)=P\{X\in B\}$
$\rightarrow$ density function: $f(x)\geq 0$ s.t. $\mu_X[a,b]=\int_a^bf(x)dx$
$\rightarrow$ Lebesgue sum: $LS_\Pi^-(X)=\sum_{k=1}^{\infty}y_k\mathbb{P}(A_k)$ with $A_k=\{w\mid y_k\leq X(w)\leq y_{k+1}\}$
$\rightarrow$ Lebesgue integral: $\int_\Omega X(w)d\mathbb{P}(w)$ or $\int_\Omega Xd\mathbb{P}$
$\rightarrow$ integrable: $\int_\Omega|X|d\mathbb{P}<\infty$ (linearity to be proved)
$\rightarrow$ $\mathbb{E}X=\int_\Omega X(w)d\mathbb{P}(w)$
$\rightarrow$Jensen's inequality: if $\varphi$ convex, $\varphi(\mathbb{E}X)\leq \mathbb{E}\varphi(X)$ (to be proved)
$\rightarrow$ Legesgue measure, Lebesgue integral $\int_\mathbb{R}f(x)d\mathcal{L}(x)$
$\rightarrow$ Riemann integral $\int_a^bf(x)dx$ defined $\Leftrightarrow$ set of points not continuous has Lebesgue measure 0; $\int_a^bf(x)dx$ defined $\Rightarrow$ $f$ is Borel measurable and the Riemann and Lebesgue integrals agree
$\rightarrow$ Monotone convergence
$\rightarrow$ Dominated convergence
$\rightarrow$ $\mathbb{E}g(X)=\int_\mathbb{R}g(x)d\mu_X(x)$ standard machine
$\rightarrow$ $\mathbb{E}g(X)=\int_{-\infty}^\infty g(x)f(x)dx$
$\rightarrow$ $Z\geq0$ and $\mathbb{E}Z=1$, $\widetilde{\mathbb{P}}(A)=\int_A Z(w)d\mathbb{P}(w)$ is a probability measure, $\widetilde{\mathbb{E}}X=\mathbb{E}[XZ]$
$\rightarrow$ $\widetilde{P}$ and $P$ on $(\Omega,\mathcal{F})$ are equaivalent if they agree which sets in $\mathcal{F}$ have probability zero
$\rightarrow$ with $\widetilde{\mathbb{P}}(A)=\int_A Z(w)d\mathbb{P}(w)$ and $Z$ almost surely positive, $Z$ is called the Radon-Nikodym derivative of $\widetilde{\mathbb{P}}$ with respect to $\mathbb{P}$, $Z=\frac{d\widetilde{\mathbb{P}}}{d\mathbb{P}}$
$\rightarrow$ to let $Y=X+\theta$ is standard normal, we can scaling pdf
$\rightarrow$ $\mathbb{P}$ and $\widetilde{\mathbb{P}}$ are equivalent, there exists almost surely positive $Z$ with $\mathbb{E}Z=1$ and $\widetilde{\mathbb{P}}(A)=\int_A Z(w)d\mathbb{P}(w)$ (to be proved)


## Chapter 2
$\rightarrow$ on $\Omega$, filtration $\mathcal{F}(s)\subset\mathcal{F}(t)$ for $0\leq s\leq t\leq T$
$\rightarrow$ $\sigma$-algebra generated by X: $\sigma(X)=\{\{X\in B\}\mid B\in \mathcal{B}\}$
$\rightarrow$ $X$ is $\mathcal{G}$-measurable if $\sigma(X)\subset\mathcal{G}$
$\rightarrow$ $X$ and $Y$ $\mathcal{G}$-measurable, $f(x,y)$ Borel-measurable, then $f(X,Y)$ is $\mathcal{G}$-measurable
$\rightarrow$ adapted stochastic process: nonempty sample space $\Omega$ with filtration $\mathcal{F}(t)$, $0\leq t\leq T$; $X(t)$ a collection of random varibles and $X(t)$ is $\mathcal{F}(t)$-measurable
$\rightarrow$ $\mathcal{F}$ and $\mathcal{G}$ are independent if $\mathbb{P}(A\cap B)=\mathbb{P}(A)\mathbb{P}(B)$ for $A\in \mathcal{F}$ and $B\in \mathcal{G}$; $X$ and $Y$ are independent; $X$ and $\mathcal{G}$ are independent
$\rightarrow$ $\mathcal{G}_1,\mathcal{G}_2,...,\mathcal{G}_n$ are independent; $\mathcal{G}_1,\mathcal{G}_2,...$ are independent 
$\rightarrow$ $f$, $g$ measuable, $X$, $Y$ independent, then $f(X)$ and $g(Y)$ are independent
$\rightarrow$ $\mu_{X,Y}(C)=\mathbb{P}\{(X,Y)\in C\}$ is a probability measure on $\mathbb{R}^2$
$\rightarrow$ $F_{X,Y}(a,b)$, $f_{X,Y}(x,y)$, then we have $\mu_X$, $\mu_Y$, $F_{X}$, $F_Y$
$\rightarrow$ $\mathbb{E}h(X,Y)=\int_{\mathbb{R}_2}h(x,y)d\mu_{X,Y}(x,y)$
$\rightarrow$ $X$ and $Y$ independent $\Leftrightarrow$ $\mu_{X,Y}(A\times B)=\mu_{X}(A)\mu_{Y}(B)$ $\Leftrightarrow$ $F_{X,Y}(a,b)=F_X(a)F_Y(b)$ $\Leftrightarrow$ $\mathbb{E}e^{uX+vY}=\mathbb{E}e^{uX}\mathbb{E}e^{vY}$ $\Leftrightarrow$ $f_{X,Y}(x,y)=f_X(x)f_Y(y)$ $\Rightarrow$ $\mathbb{E}[XY]=\mathbb{E}X\mathbb{E}Y$
$\rightarrow$ $\text{Var}(X)$, $\text{Cov}(X,Y)$
$\rightarrow$ multidimensional normal distribution
$\rightarrow$ $\mathbb{E}[X|\mathcal{G}]$: $\mathcal{G}$-measurable and $\int_A\mathbb{E}[X|\mathcal{G}](w)d\mathbb{P}(w)=\int_AX(w)d\mathbb{P}(w)$ for $A\in\mathcal{G}$
$\rightarrow$ $\mathbb{E}[X|W]$ if $\mathcal{G}=\sigma(W)$
$\rightarrow$ $\mathbb{E}[c_1X+c_2Y|\mathcal{G}]=c_1\mathbb{E}[X|\mathcal{G}]+c_2\mathbb{E}[Y|\mathcal{G}]$; $X$ $\mathcal{G}$-measurable $\Rightarrow$ $E[XY|\mathcal{G}]=X\mathbb{E}[Y|\mathcal{G}]$; $\mathcal{H}\subset \mathcal{G}$ $\Rightarrow$ $\mathbb{E}[\mathbb{E}[X|\mathcal{G}]|\mathcal{H}]=\mathbb{E}[X|\mathcal{H}]$; $X$ independent of $\mathcal{G}$ $\Rightarrow$ $\mathbb{E}[X|\mathcal{G}]=\mathbb{E}X$; $\varphi$ convex, $\mathbb{E}[\varphi(X)|\mathcal{G}]\geq \varphi(\mathbb{E}[X|G])$
$\rightarrow$ $X_i$ $\mathcal{G}$-measurable and $Y_i$ independent of $\mathcal{G}$, define $g(x_1,...,x_K)=\mathbb{E}f(x_1,...,x_K,Y_1,...,Y_L)$ $\Rightarrow$ $\mathbb{E}[f(X_1,...,X_K,Y_1,...,Y_L)|\mathcal{G}]=g(X_1,...,X_K)$
$\rightarrow$ $(\Omega,\mathcal{F},\mathbb{P})$, $\sigma(M(t))\subset\mathcal{F}(t)\subset\mathcal{F}$, martingale is $\mathbb{E}[M(t)|\mathcal{F}(s)]=M(s)$ for $0\leq s\leq t\leq T$
$\rightarrow$ Markov process: for all $0\leq s\leq t\leq T$ and any nonnegative Borel measurable funciton$f$, there is Borel measurable $g$, s.t. $\mathbb{E}[f(X(t))|\mathcal{F}(s)]=g(X(s))$

## C3 Brownian Motion
$\rightarrow$ $X_j=1,-1$ $\rightarrow$ $M_k=\sum_{j=1}^kX_j$ $\rightarrow$ quadratic variation $[M,M]_k=\sum_{j=1}^k(M_j-M_{j-1})^2$ $\rightarrow$ $W^{(n)(t)}=\frac{1}{\sqrt{n}}M_{nt}$
$\rightarrow$ central limit: distribution of $W^{(n)}(t)$ converges to $\mathcal{N}(0,t)$
$\rightarrow$ Brownian motion: for each $w\in\Omega$, there is continuous $W(t)$ which have independent increments distributed normally
$\rightarrow$ filtration for Brownian motion: $W(u)-W(t)$, $u>t$, is independent of $\mathcal{F}(t)$
$\rightarrow$ first order variation $FV_T(f)=\int_0^T|f^\prime(t)|dt=\lim\limits_{\|\Pi\|\rightarrow0}\sum_{j=0}^{n-1}|f(t_{j+1})-f(t_j))|$ 
$\rightarrow$ quadratic variation $[f,f](T)=\lim\limits_{\|\Pi\|\rightarrow0}\sum_{j=0}^{n-1}[f(t_{j+1})-f(t_j)]^2$
$\rightarrow$ $f$ with continuous derivative has 0 quadratic variation
$\rightarrow$ $[W,W](T)=T$ almost surely for Brownian motion 
$\rightarrow$ $dW(t)dW(t)=dt$, $dW(t)dt=0$, $dtdt=0$
$\rightarrow$ brownian motion is Markov chain
$\rightarrow$ $Z(t)=exp\{\sigma W(t)-\frac{1}{2}\sigma^2t\}$ is martingale
$\rightarrow$ martingale stoped at stop time is martingale

## C4 Stocastic Calculus
$\rightarrow$ simple integrand, $\varDelta(t)$ adapted, $I(t)=\int_0^T\varDelta(t)dW(t)=\\ \sum_{j=0}^{k-1}\varDelta(t_j)[W(t_{j+1})-W(t_j)]+\varDelta(t_k)[W(t)-W(t_k)]$ $\mathbb{E}I(t)=0$, $Var(I(t))=\mathbb{E}I^2(t)=\mathbb{E}\int_0^t\varDelta^2(u)du$, $[I,I](t)=\int_0^t\varDelta^2(u)du$
$\rightarrow$ $I(t)=I(0)+\int_0^t\varDelta(u)dW(u)$ $\Leftrightarrow$ $dI(t)=\varDelta(t)dW(t)$
$\rightarrow$ Ito's integral condition $\mathbb{E}
\int_0^T\varDelta^2(t)dt<\infty$
$\rightarrow$ $\lim\limits_{n\rightarrow\infty}\mathbb{E}\int_0^T|\varDelta_n(t)-\varDelta(t)|^2dt=0$ $\Rightarrow$ 
define $\int_0^t\varDelta(u)dW(u)=\lim\limits_{n\rightarrow\infty}\int_0^t\varDelta_n(u)dW(u)$
$\rightarrow$ $I(t)$ is conitnuous, $\mathcal{F}(t)$-measurable and martingale
$\rightarrow$ $df(t,W(t))=f_tdt+f_WdW(t)+\frac{1}{2}f_{WW}dt$
$\rightarrow$ when $\varDelta(t)$ and $\varTheta(t)$ adapted Ito's process:
$X(t)=X(0)+\int_0^t\varDelta(u)dW(u)+\int_0^t\varTheta(u)du$
$\rightarrow$ $[X,X](t)=\int_0^t\varDelta^2(u)du$
$\rightarrow$ $X$ Ito process, $\varGamma$ adapted,
$\int_0^t\varGamma(u)dX(u)=\int_0^t\varGamma(u)\varDelta(u)dW(u)+\int_0^t\varGamma(u)\varTheta(u)du$
$\rightarrow$ $df(t,X(t))=(f_t+f_x\varTheta+f_{xx}\varDelta^2)dt+f_x\varDelta dX(t)$
$\rightarrow$ let $\varDelta(s)$ be a deterministic function, $I(t)=\int_0^t\varDelta(s)dW(s)$ is normal with mean 0 and variance $\int_0^t\varDelta^2(s)ds$
$\rightarrow$ BSM equation
$\rightarrow$ multiple Brownian motions $W(t)=(W_1(t),...,W_d(t))$: $W_i$ Brownian motion, $W_i$ and $W_j$ independent, $W(u)-W(t)$ independent of $\mathcal{F}(t)$
$\rightarrow$ $dW_i(t)dW_j(t)=0$
$\rightarrow$ $dX(t)=\varTheta_1(t)dt+\sigma_{11}(t)dW_1(t)+\sigma_{12}(t)dW_2(t)$, 
$dY(t)=\varTheta_2(t)dt+\sigma_{21}(t)dW_1(t)+\sigma_{22}(t)dW_2(t)$,
$dX(t)dX(t)=(\sigma_{11}^2(t)+\sigma_{12}^2(t))dt$, $dX(t)dY(t)=(\sigma_{11}(t)\sigma_{21}(t)+\sigma_{12}(t)\sigma_{22}(t))dt$
$\rightarrow$ $df(t,X,Y)=f_tdt+f_xdX+f_ydY+\frac{1}{2}f_{xx}dXdX+f_{xy}dXdY+\frac{1}{2}f_{yy}dYdY$
$\rightarrow$ $d(XY)=XdY+YdX+dXdY$
$\rightarrow$ $M(t)$ martingale with continuous path, $[M,M](t)=t$ $\Rightarrow$ $M(t)$ is Brownian motion
$\rightarrow$ two dimensional Levy theorem
$\rightarrow$ Gaussian process: $X(t_1)$,..., $X(t_n)$ jointly normal
$\rightarrow$ Brownian bridge from 0 to 0: $X(t)=W(t)-\frac{t}{T}W(T)$
$\rightarrow$ Brownian bridge from a to b: $X^{a\rightarrow b}(t)=a+(b-a)t/T+X(t)$

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
$\rightarrow$ note: understanding of the system here: existence and unique risk-neutral measure ensures that any asset (V(T) depends on S_i and FT measurable can be hedged(duplicated) and is a martingale), then its price can be determined by the expectations
$\rightarrow$ $\text{For}_S(t,T)=\frac{S(t)}{B(t,T)}$
