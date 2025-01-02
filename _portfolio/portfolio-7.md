---
title: "Parallel Depth First Search for Directed Acyclic Graphs"
excerpt: "Implemented a parallel version of the popular Depth First Search algorithm which is by nature non-serializable, written entirely in CUDA and showed significant performance improvement over the serial version over large graphs."
collection: portfolio
---

Depth-First Search (DFS) is a common algorithm, often used as a building block for topological sort, connectivity and planarity testing, among many other applications. We implemented the work-efficient parallel algorithm for the DFS traversal of directed acyclic graphs (DAGs) and reported the speedup of this parallel algorithm (in comparison with the serial implementation).
<br/><img style='margin: auto; padding: 50px; display: block; width: 80% !important; max-width: 700px !important;' src='/images/Parallel_DFS.jpg'>

[[PDF]](https://viraj96.github.io/files/portfolio-7/report.pdf) [[Code]](https://github.com/divyanshu-talwar/Parallel-DFS)
