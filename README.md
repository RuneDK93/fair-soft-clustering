# fair-soft-clustering

## Description
Python implementation of the paper "Fair Soft Clustering". The paper involves algorithmic fairness for probabilistic (soft) cluster algorithms, such as a Gaussian mixture model (GMM). 
The repository includes an implementation of the proposed generalization of balance and entropy fairness metrics. 

The repository also includes an implementation of a fairlet decomposition tailored to the GMM objective. This works by identifying fairlet members, which lie close in the space modeled by a GMM. This is achieved by minimizing model-weighted distances (MWDs) through a minimum clost flow (MCF) algorithm. 


## Experiments
To run the experiments use notebooks 'Bank', 'Diabetes' and 'Census'. Results are saved to 'results' directory and can inspected in 'Plots' notebook.

## Licenses

Our implementation is build on the python implementation of the minimum cost flow algorithm from the paper:
"Fair Clustering Through Fairlets" by Chierichetti et al. (NIPS 2017)
Github: https://github.com/guptakhil/fair-clustering-fairlets

Furthermore, we compare our results with the Euclidean k-median fairlet decomposition from the paper:
"Scalable Fair Clustering" by Backurs et al. (ICML 2019)
Github: https://github.com/talwagner/fair_clustering
The code from this work is included in this supplementary material under the name 'fairtree.py' to reproduce our experimental comparisons with the k-median decomposition.   

The licenses for both of these code works are included under the name "LICENSE_fairlets" and "LICENSE_fairtree".

## Dependencies

numpy version 1.20.1 \
scipy version 1.10.1 \
sklearn version 1.2.0 \
networkx version 2.5 \
pandas version 1.3.3 \
matplotlib version 3.3.2 
