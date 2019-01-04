# The-Repeat-of-NAAG-NDAG
Winbugs code for comparing the average number of the repeat units between the Asian and African samples used in 

## Genetic polymorphisms in the circumsporozoite protein of Plasmodium malariae show a geographical bias
by Saralamba N, et al.,Malaria Journal 2018
https://malariajournal.biomedcentral.com/articles/10.1186/s12936-018-2413-3


To compare the average number of the repeat units between the Asian and African samples, the sampling model for each repeat type: NAAG and NDAG, was generated as follow;

$\lambda{}$

$r_{ij} \sim poisson(\lambda_{jk})$

$\lambda_{jk} \sim normal(\mu_k,\sigma_k)$

where $r_{ij}$ refer to the repeat number of the sample i, j indexes country and k indexes continent. The repeat numbers of each repeat type from the sample from any country was assumed to be sampled from a Poisson distribution where its average number was $\lambda{}$. These average numbers $\lamba{}$ were thought to be varied between countries and also be distributed normally around the average numbers in the continent level ($\mu$) with the standard deviation $\sigma$. 
