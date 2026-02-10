# 💻 Machine Learning

A personal endevaour to strengthen my understanding of python, it's various libraries, and their application in data analysis, data visualisation, and machine learning algorithms!

# Numpy

A fundamental package for scientific computing with Python.

###  Methods, attributes and their purpose 💡

|   **Methods & Attributes**    | **Purpose** |
| :----------: | :--------- |
| `array()`  | Create an array, parameters include but are not limited to `array(object, dtype, n...)`.  |
| `arange()` | Return evenly spaced values within a given interval. |
| `zeros()`  | Return a new array of given shape and type, filled with zeros.  |
|  `ones()`  | Return a new array of given shape and type, filled with ones.     |
| `linspace()` | Return evenly spaced numbers over a specified interval. |
| `eye`    | Create an identity matrix. |
| `random()` | Create an array of the given shape and populate it with random samples from a uniform distribution over `[0, 1)`.|
| `max()` | Returns maximum value found in an array |
| `min()` | Return the minimum value found in the array. |
| `argmax()` | Return the position of the maximum value. |
| `argmin()` | Return the position of the minimum value |
| `dtype()` | Return the object data type. |

# Pandas

A powerful data analysis and manipulation tool. This open source library has equipped me with the necessary skills to handle tabular and statistical data.

# Matplotlib

A comprehensive library for creating static, animated, and interactive visualisations in Python. An intuitive library due to my extensive use of MATLAB throughout university. 

# Seaborn

Seaborn is a python library based off of matplotlib. It is a high-level interface the generates statistical graphs when prompted with a dataset.

### **Method -** `kdeplot()`

### What is `kdeplot()`?

`kdeplot()` plots a univariate or bivariate distribution using **Kernel Density Estimation (KDE)**.

### <span style="color:blue">**What is a Kernel?**</span>

A **kernel** **is a weighting function**. Each measurement has a **zone of influence**. 

<span style="color:darkgreen">**Key Insight:**</span> A kernel says "this data point infleucnes not just its exact location, but also nearby locations on the x-axis, with influence decreasing as you move away.

### <span style="color:blue">**How KDE Works**</span>

**Kernel Density Estimation = Sum of all kernels**
For each data point in a dataset:

1. Place a kernel centered at that point
2. Add up all the kernels
3. Normalise the total area = 1 (makes it a proper probability density)

### <span style="color:blue">**What Does Bandwidth Control?**</span>

The **bandwidth** controls the width of each kernel:

- **Small bandwidth** --> Narrow kernels --> Wiggly, detailed curve. (might overfit)
- **Large bandwidth** --> Wide kernels --> Smooth curve. (might miss features)

The bandwidth effectively dictates the resolution of an estimate - A bias-variance tradeoff.
