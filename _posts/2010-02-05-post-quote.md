The Volume of a $p$-dimensional Sphere
- Let us denote the $p$-dim sphere as $\mathcal{S}_p=\left\{\mathbf{x}: x_1^2+x_2^2+\ldots+x_p^2=1\right\}$
- The volume of which becomes
$$
\begin{aligned}
V_{\mathcal{S}_p} & =\int_{\sum_{j=1}^p x_j^2 \leq 1} \cdots \int_1 \mathrm{~d} x_1 \mathrm{~d} x_2 \cdots \mathrm{~d} x_p=\int_{-1}^1 \mathrm{~d} x_1 \int_{\sum_{j=2}^p x_j^2 \leq 1-x_1^2} \cdots \int_0 \mathrm{~d} x_2 \mathrm{~d} x_2 \cdots \mathrm{~d} x_p \\
& =2 \int_0^1\left(1-x_1^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x_1 \underbrace{}_{\sum_{\mathcal{S}_{p-1}} \underbrace{\sum_{j=1}^{p-1} y_j^2 \leq 1}} \mathrm{~d} y_1 \mathrm{~d} y_2 \cdots \mathrm{~d} y_{p-1} \\
& =2 V_{\mathcal{S}_{p-1}} \int_0^1\left(1-x^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x=V_{\mathcal{S}_{p-1}} \int_0^1 x^{-\frac{1}{2}}(1-x)^{\frac{1}{2}(p-1)} \mathrm{d} x \\
& =V_{\mathcal{S}_{p-1}} \beta(1 / 2,(d+1) / 2)
\end{aligned}
$$

Prathapasinghe Dharmawansa

The Beta Function
- The Beta function takes the following integral form
$$
\beta(z, w)=\int_0^1 t^{z-1}(1-t)^{w-1} \mathrm{~d} t=\frac{\Gamma(z) \Gamma(w)}{\Gamma(z+w)}, \quad \operatorname{Re}\{z, w\}>0
$$
- As a result, we obtain
$$
V_{\mathcal{S}_p}=V_{\mathcal{S}_{p-1}} \frac{\Gamma(1 / 2) \Gamma((p+1) / 2)}{\Gamma(p / 2+1)}, p=3,4,5, \ldots
$$
relation to yield
$$
V_{\mathcal{S}_p}=\frac{\pi^{p / 2}}{\Gamma(p / 2+1)}=\frac{2 \pi^{p / 2}}{p \Gamma(p / 2)}
$$

Prathapasinghe Dharmawansa
115

The Volme and Area of a $p$-dimensional Unit Sphere
$\qquad$

Concentration of Volume Near the Equator
$\qquad$
117

Concentration of Volume Near the Equator
$\qquad$
118
Concentration of Volume Near the Equator
- Let $x_1$ denotes the north. Now consider a spherical cap at a distance $\epsilon$
from the equator (ie., $x_1=0$ )
- The volume of the spherical cap $V(\epsilon)$ assumes
$$
\begin{aligned}
& =\int_c^1\left(1-x_1^{\left.x_1^2\right)^{(p-1)}} \mathrm{d} x_1 \int \cdots \int \mathrm{X}_{\substack{p \\
\sum_{j=1}^{p-1} v_{j \leq 1} \leq 1}} \mathrm{~d} y_2 \cdots \mathrm{~d} y_{p-1}\right.
\end{aligned}
$$

$$
\begin{aligned}
& =\int_\epsilon^1\left(1-x_1^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x_1 \int_{\substack{p-1 \\
\sum_{j=1}^{p-1} y_j^2 \leq 1}} \cdots \int_1 \mathrm{~d} y_1 \mathrm{~d} y_2 \cdots \mathrm{~d} y_{p-1} \\
& =V_{\mathcal{S}_{p-1}} \int_\epsilon^1\left(1-x_1^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x_1 \\
& \text { - We also have } V_{\mathcal{S}_p}=2 V_{\mathcal{S}_{p-1}} \int_0^1\left(1-x_1^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x_1 \\
& \text { Prathapasinghe Dharmawansa }
\end{aligned}
$$

Concentration of Volume Near the Equator
- Consider the following ratio
$$
\begin{aligned}
\frac{2 V(\epsilon)}{V_{S_p}} & =\frac{\int_\epsilon^1\left(1-x^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x}{\int_0^1\left(1-x^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x}=\frac{2 \int_\epsilon^1\left(1-x^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x}{\int_0^1(1-x)^{\frac{1}{2}(p-1)} x^{-\frac{1}{2}} \mathrm{~d} x} \\
& =\frac{p \Gamma(0.5 p)}{\Gamma(0.5) \Gamma(0.5 p+0.5)} \int_\epsilon^1\left(1-x^2\right)^{\frac{1}{2}(p-1)} \mathrm{d} x
\end{aligned}
$$
- Noting that $\left(1-x^2\right) \leq e^{-x^2}$, we obtain
$$
\frac{2 V(\epsilon)}{V_{\mathcal{S}_p}}<\frac{p \Gamma(0.5 p)}{\Gamma(0.5) \Gamma(0.5 p+0.5)} \int_\epsilon^{\infty} e^{-\frac{x^2}{2}(p-1)} \mathrm{d} x<\frac{p \Gamma(0.5 p) e^{-\frac{\epsilon^2}{2}(p-1)}}{\Gamma(0.5) \Gamma(0.5 p+0.5) \epsilon(p-}
$$
$\qquad$

Concentration of Volume Near the Equator
- Therefore, we have
$$
1-\frac{2 V(\epsilon)}{V_{\mathcal{S}_p}}>1-\frac{p \Gamma(0.5 p) e^{-\frac{\epsilon^2}{2}(p-1)}}{\Gamma(0.5) \Gamma(0.5 p+0.5) \epsilon(p-1)}
$$
- For large enough $p$, we have $\frac{\left.2 \Gamma\left(\frac{p-1}{2}+\frac{3}{2}\right)\right)}{\sqrt{\pi(p-1)} \Gamma\left(\frac{p-1}{2}+1\right)} \approx \sqrt{\frac{2}{\pi}}$
- Therefore, we get
$$
1-\frac{2 V(\epsilon)}{V_{\mathcal{S}_p}}>1-\sqrt{\frac{2}{\pi(p-1) \epsilon^2}} e^{-\frac{\epsilon^2}{2}(p-1)}
$$
$\qquad$
121

Concentration of Volume Near the Equator
$\qquad$
122

Concentration of Volume Near the Equator
- Let $\epsilon=\frac{c}{\sqrt{p-1}}$. Then we have
$$
1-\frac{2 V(\epsilon)}{V_{\mathcal{S}_p}}>1-\sqrt{\frac{2}{\pi c^2}} e^{-\frac{c^2}{2}}
$$
- For any $c>0$ and large enough $p$, we have Fraction of the volume within $\left|x_1\right| \leq \frac{c}{\sqrt{p-1}}>1-\delta(c)$
where $\delta(c)=\sqrt{\frac{2}{\pi c^2}} e^{-\frac{c^2}{2}}$.
- Most of the volume concentrates within $\mathcal{O}(1 / \sqrt{p})$ distance from the equator.
$\qquad$

Concentration of Volume in an Annulus at the Boundary
$\qquad$
124

Concentration of Volume in an Annulus at the Boundary

Prathapasinghe Dharmawansa
125
Concentration of Volume in an Annulus at the Boundary

Prathapasinghe Dharmawansa
127
Gaussians in High Dimension
- Let us recall the p.d.f. of $\|\mathbf{x}\|$ as
$$
f_{\|\mathbf{x}\|}(r)=\frac{1}{2^{p / 2-1} \Gamma(p / 2)} r^{p-1} e^{-\frac{1}{2} r^2}
$$
- Therefore, the probability mass is concentrated around the maximum of $f_{\|\mathbf{x}\|}(r)$ given by
$$
\left.\frac{\mathrm{d}}{\mathrm{~d} r} f_{\|\mathbf{x}\|}(r)\right|_{r=r^*} \propto r^{*(p-2)} e^{-\frac{1}{2} r^{* 2}}\left(-r^{* 2}+(p-1)\right)=0 \Longrightarrow r^*=\sqrt{p-1}
$$
- Consequently, as we move away from $r^*$ the probability mass captured
by the tails should decrease. To demonstrate this, let us define by the tails should decrease. To demonstrate this, let us define


The Distribution of $\|\mathbf{x}\|$ for $\mathbf{x} \sim \mathcal{N}_p(\mathbf{0}, \mathbf{I})$
- The p.d.f. of $\mathbf{x}$ is given by $f(\mathbf{x}) \mathrm{d} \mathbf{x}=\frac{1}{(2 \pi)^{p / 2}} e^{-\frac{1}{2} \| \mathbf{x}} \|^2 \mathrm{~d} \mathbf{x}$
- Noting that $\mathrm{d} \mathbf{x}=r^{p-1} \mathrm{~d} r \mathrm{~d} \boldsymbol{\Omega}$ and $\|\mathbf{x}\|=r$ for polar polar coordinate transformation, we get
$$
g(r, \boldsymbol{\Omega}) \mathrm{d} r \mathrm{~d} \boldsymbol{\Omega}=\frac{1}{(2 \pi)^{p / 2}} r^{p-1} e^{-\frac{1}{2} r^2} \mathrm{~d} r \mathrm{~d} \boldsymbol{\Omega}
$$
- Finally, the p.d.f. of $\|\mathbf{x}\|=r$ is given by
$$
\begin{aligned}
h(r) \mathrm{d} r & =\mathrm{d} r \int_{\mathcal{S}_p} g(r, \boldsymbol{\Omega}) \mathrm{d} \boldsymbol{\Omega}=\frac{\mathrm{d} r}{(2 \pi)^{p / 2}} r^{p-1} e^{-\frac{1}{2} r^2} \int_{\mathcal{S}_p} \mathrm{~d} \boldsymbol{\Omega} \\
& =\frac{1}{2^{p / 2-1} \Gamma(p / 2)} r^{p-1} e^{-\frac{1}{2} r^2} \mathrm{~d} r
\end{aligned}
$$

Prathapasinghe Dharmawansa
128

Gaussians in High Dimension
- Mean zero Gaussians for $p=1,2$ have their masses close to the origin
- Their maximum values occur at the origin as well
- However, in high dimensions, there exists little or no probability mass
close to the origin
- Again, in high dimensions, the maximum value occurs at the origin
- Since the Gaussian
$$
f(\mathbf{x})=\frac{1}{(2 \pi)^{p / 2}} e^{-\frac{1}{\|}|x| \|^2}
$$
is circularly symmetric, intuitively we can expect the probability mass to concentrate at a distance $\sqrt{p}(1-\mathcal{O}(1 / \sqrt{p}))=\mathcal{O}(\sqrt{p})$ from the origin
$\qquad$

Gaussians in High Dimension
- Let us recall the p.d.f. of $\|\mathbf{x}\|$ as
$$
f_{\|\times\| \|}(r)=\frac{1}{2^{p / 2-1} \Gamma(p / 2)} r^{p-1} e^{-\frac{1}{2} r^2}
$$
- Therefore, the probability mass is concentrated around the maximum of $f_{\|\times\| \mid}(r)$ given by
$\qquad$
- Consequently, as we move away from $r^*$ the probability mass captured by the tails should decrease. To demonstrate this, let us define
$$
\operatorname{Pr}\{|r-\sqrt{p-1}|>\epsilon\}=\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\times\| \|}(r) \mathrm{d} r+\int_0^{\sqrt{p-1}-\epsilon} f_{\|\times\| \|}(r) \mathrm{d} r
$$

Gaussians in High Dimension
$\qquad$

Gaussians in High Dimension
- Let us focus on the first integral. As such, we rewrite it as
$$
\begin{aligned}
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\mid x\|}(r) \mathrm{d} r & =\int_\epsilon^{\infty} f_{\|\times\| \|}(r+\sqrt{p-1}) \mathrm{d} r \\
& =\frac{2(p-1)^{\frac{1}{2}}(p-1)}{2^{p / 2} \Gamma(p / 2)} e^{-\frac{1}{2}(p-1)} \int_\epsilon^{\infty}\left(1+\frac{r}{\sqrt{p-1}}\right)^{p-1}
\end{aligned}
$$
$$
\times e^{-\frac{1}{2}\left(r^2+2 r \sqrt{p-1}\right)} \mathrm{d} r
$$
- Noting that $(1+x) \leq e^x$ with some algebraic manipulation, we obtain
$$
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\times\|}(r) \mathrm{d} r<\frac{2 p^{\frac{1}{2}(p-1)} e^{-\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} \int_\epsilon^{\infty} e^{-\frac{r^2}{2}} \mathrm{~d} r
$$

Gaussians in High Dimension
- Since it is not difficult to show that $\int_\epsilon^{\infty} e^{-\frac{r^2}{2}} \mathrm{~d} r<\sqrt{\frac{\pi}{2}} e^{-\frac{t^2}{2}}$, we get
$$
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|x\| \|}(r) \mathrm{d} r<\frac{p^{\frac{1}{2}(p-1)} e^{-\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} \sqrt{2 \pi} e^{-\frac{e^2}{2}}
$$
- Now we may use the Stirling's approximation
$$
\Gamma(z)=\sqrt{\frac{2 \pi}{z}} e^{-z} z^z(1+\mathcal{O}(1 / z))
$$
with some algebraic manipulation to arrive at


Gaussians in High Dimension
- Let us focus on the first integral. As such, we rewrite it as
$$
\begin{aligned}
& \int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\mathbf{x}\|}(r) \mathrm{d} r= \int_\epsilon^{\infty} f_{\|\mathbf{x}\|}(r+\sqrt{p-1}) \mathrm{d} r \\
&=\frac{2(p-1)^{\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} e^{-\frac{1}{2}(p-1)} \int_\epsilon^{\infty}\left(1+\frac{r}{\sqrt{p-1}}\right)^{p-1} \\
& \times e^{-\frac{1}{2}\left(r^2+2 r \sqrt{p-1}\right)} \mathrm{d} r
\end{aligned}
$$
- Noting that $(1+x) \leq e^x$ with some algebraic manipulation, we obtain
$$
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\mathrm{x}\|}(r) \mathrm{d} r<\frac{2 p^{\frac{1}{2}(p-1)} e^{-\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} \int_\epsilon^{\infty} e^{-\frac{r^2}{2}} \mathrm{~d} r
$$
Prathapasinghe Dharmawansa
132

Gaussians in High Dimension
- Since it is not difficult to show that $\int_\epsilon^{\infty} e^{-\frac{r^2}{2}} \mathrm{~d} r<\sqrt{\frac{\pi}{2}} e^{-\frac{\epsilon^2}{2}}$, we get
$$
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\mathrm{x}\|}(r) \mathrm{d} r<\frac{p^{\frac{1}{2}(p-1)} e^{-\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} \sqrt{2 \pi} e^{-\frac{\epsilon^2}{2}}
$$
- Now we may use the Stirling's approximation
$$
\Gamma(z)=\sqrt{\frac{2 \pi}{z}} e^{-z} z^z(1+\mathcal{O}(1 / z))
$$
with some algebraic manipulation to arrive at
$$
\int_{\sqrt{p-1}+\epsilon}^{\infty} f_{\|\mathbf{x}\|}(r) \mathrm{d} r<\sqrt{\frac{e}{2}} e^{-\frac{\epsilon^2}{2}}
$$
Prathapasinghe Dharmawansa
133

Gaussians in High Dimension
- The second integral takes the form
$$
\begin{aligned}
\int_0^{\sqrt{p-1}-\epsilon} f_{\|\mathbf{x}\|}(r) \mathrm{d} r & =\int_\epsilon^{\sqrt{p-1}} f_{\|\mathbf{x}\|}(-r+\sqrt{p-1}) \mathrm{d} r \\
= & \frac{2(p-1)^{\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} e^{-\frac{1}{2}(p-1)} \int_\epsilon^{\sqrt{p-1}}\left(1-\frac{r}{\sqrt{p-1}}\right)^{p-1} \\
& \times e^{-\frac{1}{2}\left(r^2-2 r \sqrt{p-1}\right)} \mathrm{d} r \\
& <\frac{2 p^{\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} e^{-\frac{1}{2}(p-1)} \int_\epsilon^{\sqrt{p-1}} e^{-\frac{r^2}{2}} \mathrm{~d} r \\
& <\frac{2 p^{\frac{1}{2}(p-1)}}{2^{p / 2} \Gamma(p / 2)} e^{-\frac{1}{2}(p-1)} \int_\epsilon^{\infty} e^{-\frac{r^2}{2}} \mathrm{~d} r
\end{aligned}
$$
Prathapasinghe Dharmawansa
134

Gaussians in High Dimension
- Following similar arguments as before, we obtain
$$
\int_0^{\sqrt{p-1}-\epsilon} f_{\|\mathbf{x}\|}(r) \mathrm{d} r<\sqrt{\frac{e}{2}} e^{-\frac{\epsilon^2}{2}}
$$
- Finally, we arrive at
$$
\operatorname{Pr}\{|r-\sqrt{p-1}|>\epsilon\}<\sqrt{2 e} e^{-\frac{\epsilon^2}{2}}
$$
- This confirms that the probability mass is in a narrow annulus of radius approximately $\sqrt{p}$
- In other words, alomost all mass of the high dimensional Gaussian lies within the annulus $|r-\sqrt{p-1}| \leq \epsilon$

Gaussians in High Dimension
- Following similar arguments as before, we obtain
$$
\int_0^{\sqrt{p-1}-\epsilon} f_{\|\mathbf{x}\|}(r) \mathrm{d} r<\sqrt{\frac{e}{2}} e^{-\frac{\epsilon^2}{2}}
$$
- Finally, we arrive at
$$
\operatorname{Pr}\{|r-\sqrt{p-1}|>\epsilon\}<\sqrt{2 e} e^{-\frac{\epsilon^2}{2}}
$$
- This confirms that the probability mass is in a narrow annulus of radius approximately $\sqrt{p}$
- In other words, alomost all mass of the high dimensional Gaussian lies within the annulus $|r-\sqrt{p-1}| \leq \epsilon$
Prathapasinghe Dharmawansa
135
