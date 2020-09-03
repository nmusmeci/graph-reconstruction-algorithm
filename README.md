# Network-reconstruction-algorithm-
Algorithm that reconstructs missing connections of a network starting from a limited amount of information. I invented this technique as part of my Master degree's thesis in Statistical Physics. We demonstrated its predictive power in a number of real-world applications, such as interbank lending and world trade networks, in peer-reviewed scientific papers [1,2].

The algorithm takes as input the following variables:

* a non-topological quantity for each node, called "fitness", which is somehow correlated with the number of connections of the node (e.g. GDP of a country, which correlates with the country's number of trading connections)
* number of connections of at least one node in the network ("seed")

The missing connections are reconstructed by running a "fitness model" [3] whose main parameter "z" is calculated by Maximum Likelihood Estimation using the information provided by the seed(s). Since the algorithm assumes that a "fitness model" is a good approximation for the network structure, the more this assumption is reasonable the more reliable the reconstructed network is.  

---
References:
[1] N. Musmeci, S. Battiston, G. Caldarelli, A. Gabrielli, M. Puliga: “Bootstrapping topology and systemic risk of Complex Networks using the Fitness Model ”, Journal of Statistical Physics (2013) https://link.springer.com/article/10.1007/s10955-013-0720-1 (pdf from arxiv: https://arxiv.org/pdf/1209.6459.pdf) 

[2] G. Cimini, T. Squartini, N. Musmeci, M. Puliga, A. Gabrielli, D. Garlaschelli, S. Battiston, G. Caldarelli: "Reconstructing topological properties of complex networks using the fitness model", International Conference on Social Informatics (2015) https://link.springer.com/chapter/10.1007/978-3-319-15168-7_41 (pdf from arxiv: https://arxiv.org/pdf/1410.2121.pdf)

[3] Caldarelli, G., Capocci, A., De Los Rios, P., Munoz, M.: "Scale-free networks from varying vertex intrinsic fitness". Physical review letters 89 (25), 258,702 (2002)
