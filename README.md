# Coursework Portfolio

Here’s some of my coursework from Computer Science + Mathematics at Harvey Mudd College. It covers data structures, performance, testing, and numerical models, which also come up in my application projects.

**Languages and tools:** C++, Python, NumPy, pandas, Matplotlib, Git, Make

## C++ data structures (CS70)

I worked on these projects with a partner: Jamie for the first three and Noah for the last two. We worked from course-provided starter code and specifications.

| Project | Work covered | Technical topics |
| --- | --- | --- |
| Dynamic train | A dynamically allocated C++ train structure and accompanying exercises | Object lifetime, pointers, ownership, and debugging |
| Lists and vectors | Integer list and vector implementations, tests, and performance comparisons | Container interfaces, iteration, allocation, and access costs |
| Tree-based string set | A string-set implementation and spell-checking client | Search-tree organization, insertion, membership, and testing |
| Generic tree set | A templated set, iterator interfaces, tests, and a client program | Templates, reusable interfaces, traversal, and const-correctness |
| Hash set | A hash-based set, hashing functions, tests, and a spell-checking client | Hashing, collisions, container behavior, and edge cases |

The original histories are preserved in private forks on my account. They retain the original authors, co-authors, dates, and course notices. The source solutions are not included here because CS70 requires instructor permission before course materials can be shared outside the class.

### Design questions I can discuss

- **Lists versus vectors:** Similar interfaces can hide different memory layouts and access costs. Vectors store elements together and support fast indexed access. Linked structures have different traversal and allocation costs.
- **Trees versus hash tables:** The right choice depends on whether the client needs ordered traversal or fast average-case membership checks. Tree height and hash collisions can have a large effect on performance.
- **Ownership:** C++ containers need clear rules for who owns each allocation and what happens when an object is copied or destroyed.
- **Testing:** Empty containers, duplicate insertions, iteration boundaries, and copy independence deserve targeted tests. A spell-checking client also exercises how the container behaves outside a small unit test.

## Mathematical machine learning (Math 129)

My Math 129 repository includes Python implementations, written assignments, plots, and project reports. The programming work extends course-provided starter files.

| Topic | Work and artifacts |
| --- | --- |
| Linear and regularized regression | Weight estimation, predictions, RMSE evaluation, and comparisons across regularization strengths |
| Numerical optimization | Gradient-descent work and plots of convergence and parameter behavior |
| Sparse modeling | Lasso-related programming and visualization |
| Clustering | K-means assignment and centroid updates, objective tracking, repeated initializations, and visualizations |
| Technical communication | Written homework, a midterm project report and presentation, and a term-project proposal |

### Modeling questions I can discuss

- **Regularization:** Changing the penalty affects coefficient size and validation error. Training error alone doesn’t show how well a model generalizes.
- **Optimization:** Learning rate, data scale, and stopping rules affect convergence. The path to a result matters too.
- **K-means:** Different starting centers can lead to different local solutions, so it helps to try several initializations. The implementation also needs to handle empty clusters.
- **Choosing k:** Within-cluster squared error usually decreases as the number of clusters grows. Choosing the smallest raw error across k is not enough; an elbow analysis or another selection criterion is needed.

The Math 129 source remains in the course organization, where personal forking is disabled. This public overview does not redistribute its starter code, assignment solutions, or datasets.

## Attribution and scope

I wrote these summaries and discussion notes to give people a way to browse my coursework while keeping course solutions private. The original repositories and private archives keep the source history. Any claims about speed, accuracy, or passing tests need a reproducible result to back them up.

For application projects with public code and setup instructions, see my [main profile](https://github.com/WCopelandProg).
