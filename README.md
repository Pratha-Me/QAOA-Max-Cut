# QAOA-Max-Cut

I solved the most studied problem of Combinatorial optimization, namely, MaxCut by using QAOA. In the python notebook, I have gone through a light literature review and then built the codes. I have solved a simple case of a graph (Four Vertices and Four Edges). The results are accurate in both of the cases. The report is kept inside the "reports" folder. There's an exported report, a pdf file named "max-cut.pdf".

The solution to the max-cut problem is identical to that of the [Antiferromagnetic](https://www.sciencedirect.com/topics/engineering/antiferromagnetic-material) [Ising model](http://micro.stanford.edu/~caiwei/me334/Chap12_Ising_Model_v04.pdf). Interestingly, there's only one change needed to solve [Ferromagnetic](https://www.sciencedirect.com/topics/materials-science/ferromagnetism) Ising model. The cost function needs to be positive. That means the code changes from `cost -= 1` to `cost += 1`. You almost missed the trick, didn't you?😜. The former will reduce the superpositioned states to |0101> and |1010> and the latter to |0000> and |1111>. 

I have enlisted all references at the end of the notebook. To generate this report, the two primary resources I studied are bulleted below.

1. Guerrero, N., 2020. Solving Combinatorial Optimization Problems using the Quantum Approximation Optimization Algorithm. [online] Scholar.afit.edu. Available at: <https://scholar.afit.edu/cgi/viewcontent.cgi?article=4264&context=etd>.

2. Qiskit.org. n.d. Solving combinatorial optimization problems using QAOA. [online] Available at: <https://qiskit.org/textbook/ch-applications/qaoa.html> [Accessed 16 September 2021].
