\label{fig:splat-diagram}Diagram of the core Splat simulation model. Input are parameters indicated with double borders and those that can be estimated from real data are shaded blue. Red shading indicates the final output. The simulation begins by generating means from a gamma distribution. Outlier expression genes are added by multiplying by a log-normal factor and the means are proportionally adjusted for each cells library size. A mean-variance trend is enforced by adjusting the means using a simulated Biological Coefficient of Variation (BCV). These final means are used to generate counts from a Poisson distribution. In the final step dropout is (optionally) simulated by randomly setting some counts to zero, based on each gene's mean expression.