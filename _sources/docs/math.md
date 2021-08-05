# Mathematical modeling

The introduction of mathematical modeling in biotechnology dates back to around 1960 and an inspiring review of early work in the field is written by Bailey {cite}`Bailey1998`. Further inspiration is provided by the more recent review by Cvijovic *et al.* that summarizes the main modeling approaches of biological processes and illustrate their applications in industrial biotechnology {cite}`Cvijovic2011`.

Two important classes of mathematical models are those based on

- systems of differential equations
- agent-based modeling

Representing the former class, a cornerstone in the modeling of the dynamics of biological systems is the [Lotka–Volterra equations](https://en.wikipedia.org/wiki/Lotka%E2%80%93Volterra_equations), also referred to as the predator–prey equations:

\begin{align*}
\frac{dx}{dt} & = \alpha x - \beta xy \\
\frac{dy}{dt} & = \delta xy - \gamma y
\end{align*}

where $x$ and $y$ are the number of preys and predators, respectively, and their interactions are phenomenologically and collectively described by the coefficients $\alpha$, $\beta$, $\delta$, and $\gamma$. There is no track record of individual members in the populations, which is both a strength and a weakness. In epidemiology, for instance, it can set a clear focus on a single key parameter namely the *[basic reproduction number](https://en.wikipedia.org/wiki/Basic_reproduction_number)*, $R_0$, that acts as a risk indicator for infectious diseases. The limitations are equally obvious as a disease spread is affected by decisions made by individuals that may be difficult to predict.

[Agent-based models](https://en.wikipedia.org/wiki/Agent-based_model) (ABMs) are created to simulate the seemingly stochastic behaviour of the microscopic individuals to build up and predict the appearance of complex macroscopic phenomena. Most agent-based models are composed of: (1) numerous agents specified at various scales (typically referred to as agent-granularity); (2) decision-making heuristics; (3) learning rules or adaptive processes; (4) an interaction topology; and (5) an environment. The use and advancements of ABMs is promoted by the increasing computational power of modern computers and there is a natural appeal in explaining macroscopic phenomena from microscopic interactions. There may be a risk, however, of not seeing the forest for all the trees as the complexity of decision-makinng can be increased.