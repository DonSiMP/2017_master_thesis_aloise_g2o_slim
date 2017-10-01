## Extended Measurements in Pose Graph Optimization [aka g2o_slim]
###### Irvin Aloise's master thesis, October 2017

#### Abstract
The goal of this Master’s Thesis is the design and development of a graph-optimization system tailored for SLAM pipelines. The work focuses on simplicity, accuracy and speed, reaching excellent results in each of the targeted fields.

In particular, this back-end aims attention at 3D pose-graphs and 3D Bundle Adjustment problems, producing outcomes comparable to current state-of-the-art systems like [g2o](https://github.com/RainerKuemmerle/g2o).

At its core there is a novel error function for SE(3) objects based on the concept of matrices’ chordal distance. This approach reduces the problem’s non-linearity bringing several benefits to the computation. The fastness of the system is due to a well-designed implementation that performs zero memory copy during the iterative part and that exploits SIMD instructions of modern CPUs and a smart use of the CPU cache.

Finally, the systems has been tested on both synthetic and real-world datasets and in both scenarios it succeeded in its purposes, being able to produce results comparable to state-of-the-art systems in only 5 thousands lines of code.
