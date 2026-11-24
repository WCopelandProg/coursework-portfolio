# Coursework Portfolio

Selected coursework from my Computer Science + Mathematics degree at Harvey Mudd College. This overview covers the programming and mathematical work behind my application projects: implementing data structures, reasoning about performance, testing edge cases, and analyzing numerical models.

**Languages and tools:** C++, Python, NumPy, pandas, Matplotlib, Git, Make

## C++ data structures — CS70

These projects were completed through pair programming. The first three below were developed with Jamie, and the last two with Noah. The course supplied starter code and specifications; the work was collaborative, not a claim of sole authorship.

| Project | Work covered | Technical topics |
| --- | --- | --- |
| Dynamic train | A dynamically allocated C++ train structure and accompanying exercises | Object lifetime, pointers, ownership, and debugging |
| Lists and vectors | Integer list and vector implementations, tests, and performance comparisons | Container interfaces, iteration, allocation, and access costs |
| Tree-based string set | A string-set implementation and spell-checking client | Search-tree organization, insertion, membership, and testing |
| Generic tree set | A templated set, iterator interfaces, tests, and a client program | Templates, reusable interfaces, traversal, and const-correctness |
| Hash set | A hash-based set, hashing functions, tests, and a spell-checking client | Hashing, collisions, container behavior, and edge cases |

The original histories are preserved in private forks on my account. They retain the original authors, co-authors, dates, and course notices. The source solutions are not included here because CS70 requires instructor permission before course materials can be shared outside the class.

### Design questions I can discuss

- **Lists versus vectors:** Why does an interface that looks similar hide very different memory layouts and access costs? A vector provides contiguous storage and efficient indexed access. A linked structure makes different tradeoffs around traversal and allocation.
- **Trees versus hash tables:** What operations does the client need? Ordered traversal and average-case membership speed lead to different choices. Tree height and hash collisions can dominate the performance of an otherwise simple interface.
- **Ownership:** Which object owns an allocation, and what should copying or destroying that object do? Making these rules explicit is essential when implementing containers in C++.
- **Testing:** Empty containers, duplicate insertions, iteration boundaries, and copy independence deserve targeted tests. A spell-checking client also exercises how the container behaves outside a small unit test.

## Mathematical machine learning — Math 129

My Math 129 repository includes Python implementations, written assignments, plots, and project reports. The programming work extends course-provided starter files.

| Topic | Work and artifacts |
| --- | --- |
| Linear and regularized regression | Weight estimation, predictions, RMSE evaluation, and comparisons across regularization strengths |
| Numerical optimization | Gradient-descent work and plots of convergence and parameter behavior |
| Sparse modeling | Lasso-related programming and visualization |
| Clustering | K-means assignment and centroid updates, objective tracking, repeated initializations, and visualizations |
| Technical communication | Written homework, a midterm project report and presentation, and a term-project proposal |

### Modeling questions I can discuss

- **Regularization:** How does changing the penalty alter coefficient size and validation error? Training error alone does not establish whether a model generalizes.
- **Optimization:** How do the learning rate, data scale, and stopping rule affect convergence? The trajectory matters as well as the final output.
- **K-means:** Why run more than one initialization? Different starting centers can lead to different local solutions. Empty clusters also need deliberate handling.
- **Choosing k:** Within-cluster squared error usually decreases as the number of clusters grows. Choosing the smallest raw error across k is not enough; an elbow analysis or another selection criterion is needed.

The Math 129 source remains in the course organization, where personal forking is disabled. This public overview does not redistribute its starter code, assignment solutions, or datasets.

## Attribution and scope

This repository is a public guide to my coursework, not a public release of the course solutions. It contains newly written summaries and discussion notes. Source history remains intact in the original repositories and private archives. No performance, accuracy, or test-pass claims are made without a corresponding reproducible result.

For application projects with public code and setup instructions, see my [main profile](https://github.com/WCopelandProg).
