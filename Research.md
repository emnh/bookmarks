# Research Related Reading

## Compression
 - [Compressing Sets and Multisets of Sequences](http://arxiv.org/pdf/1401.6410.pdf)
 - [Compressing multisets using tries](http://www.vincent-gripon.com/files/articles/2012-itw.pdf)
 - [Burrows-Wheeler transform](https://en.wikipedia.org/wiki/Burrows%E2%80%93Wheeler_transform)
 - [Move-to-front transform](https://en.wikipedia.org/wiki/Move-to-front_transform)
 - [Arithmetic Coding](https://en.wikipedia.org/wiki/Arithmetic_coding)

## Maximum Independent Set (MIS)
 - [All Maximal Independent Sets and Dynamic Dominance for Sparse Graphs](http://arxiv.org/pdf/cs/0407036v1.pdf)

Counting number of unions of neighbourhoods in a bipartite graph is equivalent to counting maximal independent sets in the graph : #MIS. It is the bottleneck in computing heuristics for boolean-width, a graph width parameter inspired by treewidth. #MIS is equivalent to counting maximal clique (just invert graph) and counting independent dominating sets. Searching by more names for the problem gives a larger set of search results.

 - [The Independent Domination Polynomial (2016)](https://arxiv.org/pdf/1602.08250.pdf)
 - [Wikipedia: #P-Complete](https://en.wikipedia.org/wiki/Sharp-P-complete)
   - From Sadia's Dr. Thesis: It is known that counting MISs is #P-hard even for planar bipartite graphs [50] and designing an approximation algorithm for this problem is also intricate [51, 52].
     - [50]: [The Complexity of Counting in Sparse, Regular, and Planar Graphs](http://epubs.siam.org/doi/abs/10.1137/S0097539797321602)
     - [51]: [J. Radhakrishnan M. M. Halldorsson. Improved approximation of independent sets in bounded-degree graphs via subgraph removal. Nordic Journal of Computing, 1:475–492, 1994.](https://pdfs.semanticscholar.org/87c3/3c65a183ecdcf362f1d42d28169b092afaad.pdf)
     - [52]: [T. Matsui. Approximation algorithms for maximum independent set problems and fractional coloring problems on unit disk graphs. Discrete and Computational Geometry, Springer Verlag, Lecture Notes in Computer Science, vol. 1763: 194–200, 2000.](https://link.springer.com/chapter/10.1007/978-3-540-46515-7_16)
   - Can we get inspiration to solve #MIS by a #P-complete problem which has an FPTAS? Perhaps DNF?
   - [The DNF Counting Problem (2004)](http://www.cs.cmu.edu/afs/cs/academic/class/15859-f04/www/scribes/lec8.pdf)
 - [Improved Inapproximability Results for Counting Independent Sets in the Hard-Core Model (2012)](https://arxiv.org/pdf/1105.5131.pdf)
 - [On Counting Cliques, Clique-covers and Independent sets in Random Graphs (2015)](https://arxiv.org/pdf/1411.6673.pdf)
 - [Dominating Set Counting in Graph Classes (2011)](http://dopal.cs.uec.ac.jp/okamotoy/PDF/2011/DS.pdf)
   - "On the other hand, we prove that counting the number of dominating sets (and minimum dominating sets) in split
graphs and chordal bipartite graphs is #P-complete".
 - [The Complexity of Counting Cuts and of Computing the Probability that a Graph is Connected (1983)](http://epubs.siam.org/doi/abs/10.1137/0212053)
 - [Counting Linear Extensions: Parameterizations by
Treewidth](http://drops.dagstuhl.de/opus/volltexte/2016/6390/pdf/LIPIcs-ESA-2016-39.pdf)
   - A #P-Complete problem that can be solved by FPT using threewidth.
 - [On the Analysis of Independent Sets via Multilevel Splitting (2016)](https://people.smp.uq.edu.au/RadislavVaisman/papers/IndependentSetsSplitting.pdf)
   - Approximation algorithm for #MIS.
   - [Talk](https://people.smp.uq.edu.au/RadislavVaisman/Talks/is-splitting.pdf)
 - [Knuth: Estimating the efficiency of backtrack programs](https://pdfs.semanticscholar.org/96b4/4e128bc9ef19160b6f6ccf39c4f71f04b96c.pdf)
 
## Miscellaneous Techniques
 - [Inclusion-Exclusion Principle](https://en.wikipedia.org/wiki/Inclusion%E2%80%93exclusion_principle)
 - [Inclusion–Exclusion Algorithms for Counting Set Partitions](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.98.1018&rep=rep1&type=pdf)
