# data

Two parts data used in our paper about Lpnet algorithm.

* `Random matrix`<br>
10000 distance matrixes for 30 taxa which use random numbers between 0 and 1 from the uniform distribution as pairwise distances.
And then, we add a smallest constant to all distances to guarantee the triangle inequality in every distance matrix.
We provide 10000 distance matrixes in this folder.

* `Simulation sequences`<br>
We randomly generate 10000 trees for 30 taxa by using the function `sim.taxa` from the R package `TreeSimGM`[1].
We let the parameter `waiting time until speciation` for `sim.taxa` be exponentially distributed and normalize the maximum pairwise distance to 1 for every simulation tree.
Then we use the software `Dawg`[2] to simulate DNA sequences of length 10000bp from the simulation trees under `Jukes-Cantor` model.
We previde origin simulation trees, distance matrixes, and simulation sequences in this folder.

## Reference

[1][Hagen, O. and Stadler, T. 2018. TreeSimGM: Simulating phylogenetic trees under general Bellman-Harris models with lineage-specific shifts of speciation and extinction in R. Methods in ecology and evolution, 9(3): 754{760.](https://besjournals.onlinelibrary.wiley.com/doi/full/10.1111/2041-210X.12917)<br>
[2][Cartwright, R. A. 2005. DNA assembly with gaps (Dawg): simulating sequence evolution. Bioinformatics, 21(Suppl 3): iii31{iii38.](https://academic.oup.com/bioinformatics/article/21/Suppl_3/iii31/216620)<br>
