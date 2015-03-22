# Network-reconstruction-algorithm-
Algorithm for reconstructing topology of complex networks from a limited number of links (Bootstrapping method [1]).
The algorithm assumes the knowledge of:

* a non-topological quantity for each node, called "fitness", and related to the node degree;
* neighbours for a subset of nodes ('seeds').

The complete topology is reconstructed by running a "fitness model" [2] whose main parameter "z" is calculated by Maximum Likelihood Estimation over the 'seeds' information. Since the algorithm assumes that a "fitness model" is a good approximation for the network structure, the more this assumption is reasonable the more reliable is the reconstructed network.  

References:
[1] N. Musmeci, S. Battiston, G. Caldarelli, A. Gabrielli, M. Puliga: “Bootstrapping topology and systemic risk of Complex Networks using the Fitness Model ”, Journal of Statistical Physics (2013)
[2] Caldarelli, G., Capocci, A., De Los Rios, P., Munoz, M.: "Scale-free networks from varying vertex intrinsic fitness". Physical review letters 89 (25), 258,702 (2002)
